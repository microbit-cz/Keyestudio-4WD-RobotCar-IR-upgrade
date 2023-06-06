[IR_MD]: /assets/languages/czech/ir_setup.md
[models_MD]: /assets/languages/czech/models_download.md
[crimping_MD]: /assets/languages/czech/crimping_cables.md
[nuts_MD]: /assets/languages/czech/nut_insertion.md
[charge_MD]: /assets/languages/czech/charging_setup.md
[czechLanguage_MD]: README.cs.md
[englishLanguage_MD]: /README.md
[productFoto]: /assets/img/welcome.jpg

# Detekce na zdi a integrované nabíjení pro robotické auto KS4031 Keyestudio 4WD Mecanum

<kbd>[<img title="Czech" alt="Czech" src="/assets/img/icons/czech.svg" width="22">][czechLanguage_MD]</kbd> <kbd>[<img title="English" alt="English" src="/assets/img/icons/english.svg" width="22">][englishLanguage_MD]</kbd>

![Welcome!][productFoto]

Funkce **[detekce stěn][IR_MD]** využívá senzory k detekci přítomnosti překážek v okruhu 180°, jako jsou stěny a další objekty v dráze vozu, a umožňuje vozu automaticky zastavit nebo změnit směr jízdy, aby se vyhnul kolizi. Tato funkce může být užitečná zejména v situacích, kdy se vůz pohybuje v omezeném prostoru nebo projíždí složitým prostředím, jako je například Bludiště.

**[Integrované nabíjení][charge_MD]** přes USB-C může ušetřit čas a zvýšit pohodlí, protože umožňuje uživatelům rychle a snadno dobíjet auto bez potřeby dalšího vybavení nebo kabelů.

## Dokumentace

- **[Modely ke stažení][models_MD]**
- [Jak nastavit detekci stěn][IR_MD]
- [Jak nastavit integrované nabíjení][charge_MD]
- [Vsázení matic][nuts_MD]
- [Krimpování kabelů][crimping_MD]

---

## Test funkčnosti

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

Uvedený úryvek kódu přiřadí digitální údaje z infračervených senzorů příslušným proměnným: front_P, front_L, left a right. Příkazy console.log zobrazí hodnoty jednotlivých senzorů do konzoly

---