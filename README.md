[IR_MD]: /assets/languages/master/ir_setup.md
[models_MD]: /assets/languages/master/models_download.md
[crimping_MD]: /assets/languages/master/crimping_cables.md
[nuts_MD]: /assets/languages/master/nut_insertion.md
[charge_MD]: /assets/languages/master/charging_setup.md
[czechLanguage_MD]: /assets/languages/czech/README.cs.md
[englishLanguage_MD]: /README.md
[productFoto]: /assets/img/welcome.jpg

# Wall Detection and Integrated Charging addition for KS4031 Keyestudio 4WD Mecanum Robot Car

<kbd>[<img title="Czech" alt="Czech" src="/assets/img/icons/czech.svg" width="22">][czechLanguage_MD]</kbd> <kbd>[<img title="English" alt="English" src="/assets/img/icons/english.svg" width="22">][englishLanguage_MD]</kbd>

![Welcome!][productFoto]

The **[wall detection][IR_MD]** feature uses sensors to detect the presence of obstacles in 180° radius such as walls and other objects in the car's path, allowing the car to automatically stop or change its direction to avoid collisions. This feature can be particularly useful in situations where the car is operating in a confined space or navigating through a complex environment such as Maze.

The **[integrated charging][charge_MD]** through USB-C can save time and improve convenience by allowing users to quickly and easily recharge the car without the need for additional equipment or cables.

## Documentation

- **[Download Models][models_MD]**
- [How to set-up wall detection][IR_MD]
- [How to set-up integrated charging][charge_MD]
- [Nut insertion][nuts_MD]
- [Cable crimping][crimping_MD]

---

## Functionality test

```js
pins.setPull(DigitalPin.P0, PinPullMode.PullNone);
pins.setPull(DigitalPin.P7, PinPullMode.PullNone);
pins.setPull(DigitalPin.P12, PinPullMode.PullNone);
pins.setPull(DigitalPin.P13, PinPullMode.PullNone);

while (true) {
  let front_P = pins.digitalReadPin(DigitalPin.P12);
  let front_L = pins.digitalReadPin(DigitalPin.P7);
  let left = pins.digitalReadPin(DigitalPin.P0);
  let right = pins.digitalReadPin(DigitalPin.P13);

  console.log("front_P: " + front_P);
  console.log("front_L: " + front_L);
  console.log("left: " + left);
  console.log("right: " + right);
  pause(100);
}
```

The given code snippet assigns the digital readings from the IR sensors to respective variables: front_P, front_L, left, and right. The console.log statements display the values of each sensor to the Console.

---
