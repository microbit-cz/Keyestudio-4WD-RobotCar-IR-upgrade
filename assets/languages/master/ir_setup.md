[4_channel_IR]: https://www.aliexpress.com/item/32910726663.html "Four Way 4 Channel Infrared Detector Tracking Line Obstacle Avoidance Sensor Module Diy Smart Car Robot Module Board For Arduino"
[insert]: https://www.aliexpress.com/item/1005003582355741.html "M2 M2.5 M3 M4 M5 M6 Brass Hot Melt Insert Knurled Nut Thread Heat Molding Double Twill Injection Embedment Nut For 3D Printer"
[screws]: https://www.aliexpress.com/item/1005005098799689.html "Screw Set KM2 2.5 KM3Machine Laptop Screws Flat Head Phillips Drive Accessories for Repair Computer Electronic Laptop Screws Kit"
[lego_pieces]: https://www.aliexpress.com/item/1005004975645306.html "Bolt Pin with Friction Peg Cross Axle Building Block Bricks Connector Technical 32002 MOC Parts Assemble Particles Toy"
[wire]: https://www.aliexpress.com/item/1005002906304265.html "Led Wire Cable 22AWG 2Pin/3Pin/4Pin/5Pin/6pin For WS2812B WS2811 5050 2835 5730 Led Strip Light 5m/10m/20m/50m/100m"
[dupont]: https://www.aliexpress.com/item/1005002646300836.html "620pcs Dupont Connector 2.54mm, Dupont Cable Jumper Wire Pin Header Housing Kit, Male Crimp Pins+Female Pin Terminal Connector"
[insert_nut]: nut_insertion.md
[cables]: crimping_cables.md
[models]: models_download.md

# Tutorial - 4 way IR sensor addition

<table>
  <thead>
    <tr>
      <th>Parts List</th>
      <th>Reference Photo</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <ul>
         <li>1x <strong><a href="https://www.aliexpress.com/item/32910726663.html">4 Channel Infrared Sensor Module</a></strong></li>
         <li>8x <strong>Lego Pin</strong> type <a href="https://www.aliexpress.com/item/1005004975645306.html">32002</a></li>
         <li>6x <strong>Insert nut</strong> type <a href="https://www.aliexpress.com/item/1005004629314742.html">M3x4x4.2</a></li>
         <li>6x <strong>Screw</strong> type <a href="https://www.aliexpress.com/item/1005005098799689.html">M3x4mm</a></li>
         <li><strong><a href="models_download.md">Models</a></strong>
            <ul>
                <li>1x Front holder</li>
                <li>2x side holder - top piece</li>
                <li>2x side holder - bottom piece</li>
                <li>1x back lid</li>
            </ul>
         </li>
         <li><strong><a href="crimping_cables.md">Cables</a></strong>
            <ul>
                <li>2x 3pin dupont 20cm</li>
                <li>2x 3pin dupont 15cm</li>
                <li>1x 1pin dupont 8cm</li>
                <li>1x 2pin dupont 8cm</li>
                <li>1x 3pin dupont 5cm</li>
            </ul>
         </li>
        </ul>
      </td>
      <td><img src="/assets/img/IR_reference.jpg" alt="Reference Photo" width="400"></td>
    </tr>
  </tbody>
</table>

all parts were bought on Aliexpress on 29.5.2023 and cost **14.61$** without shipping:

- [Four Way 4 Channel Infrared Detector Tracking Line Obstacle Avoidance Sensor Module Diy Smart Car Robot Module Board For Arduino][4_channel_IR] - **0.97$**
- [Screw Set KM2 2.5 KM3Machine Laptop Screws Flat Head Phillips Drive Accessories for Repair Computer Electronic Laptop Screws Kit][screws] - choice: _250PCS SET_ - **1.03$**
- [Bolt Pin with Friction Peg Cross Axle Building Block Bricks Connector Technical 32002 MOC Parts Assemble Particles Toy][lego_pieces] - choice: _50pcs_ - **2.52$**
- [M2 M2.5 M3 M4 M5 M6 Brass Hot Melt Insert Knurled Nut Thread Heat Molding Double Twill Injection Embedment Nut For 3D Printer][insert_nut] - choice: _M3(OD4.2mm)_ , _Length 3mm 50pcs_ - **0.85$**
- [Led Wire Cable 22AWG 2Pin/3Pin/4Pin/5Pin/6pin For WS2812B WS2811 5050 2835 5730 Led Strip Light 5m/10m/20m/50m/100m][wire] - choice: _10m_ - **5.80$**
- [620pcs Dupont Connector 2.54mm, Dupont Cable Jumper Wire Pin Header Housing Kit, Male Crimp Pins+Female Pin Terminal Connector][dupont] - **3.44$**

---

# Embedding Models

Before Embeding [models][models] onto the car create the needed [cables][cables] and insert all needed [insertion nuts][insert_nut].

When embedding the models onto the car, it is important to make sure that everything is secured properly and all cables are connected correctly. Start with the back lid. Connect the cables to the appropriate pins on the module.

Make sure all cables are tidy and out of the way of any moving parts. Once all models are embedded onto the car, test the IR sensors to ensure they are working properly. With all four sensors in place, the car should be able to detect obstacles in all directions.

---

## Back Lid

**Parts:**

- 1x Back Lid
- 2x insertion nuts
- 2x screws
- 1x 3pin dupont 5cm
- 1x 2pin dupont 8cm
- 1x 1pin dupont 8cm
- 1x [4 Channel Infrared Sensor Module][4_channel_IR]

<table>
  <tr>
    <td valign="top">Step 1: <a href="nut_insertion.md">Insert the 2 insertion nuts into the model</a></td>
    <td valign="top"><img src="/assets/img/tutorial/back/step_1.jpg" alt="step1"  height="220"></td>
  </tr>
  <tr>
    <td valign="top">Step 2: Screw the IR module in</td>
    <td valign="top"><img src="/assets/img/tutorial/back/step_2.jpg" alt="step2"  height="220"></td>
  </tr>
  <tr>
    <td valign="top">Step 3: Connect the <a href="crimping_cables.md">Cables</a> 
    <ul>
        <li>3pin dupont cable (5cm) to ports:
            <ul>
                <li>5V - VCC</li>
                <li>G - GND</li>
                <li>P7 - OUT1</li>
            </ul>
        </li>
        <li>2pin dupont cable(8cm) to ports:
            <ul>
                <li>P12 - OUT3</li>
                <li>P13 - OUT4</li>
            </ul>
        </li>
        <li>1pin dupont cable (8cm) to ports:
            <ul>
                <li>P0 - OUT2</li>
            </ul>
        </li>
    </ul>
    </td>
    <td valign="top"><img src="/assets/img/tutorial/back/step_3.jpg" alt="step3"  height="220"></td>
    <td valign="top"><img src="/assets/img/tutorial/back/step_3.png" alt="step3"  height="220"></td>
  </tr>
</table>

---

## Front Piece

**Parts:**

- 1x Front holder
- 4x LEGO Pin type 32002
- 2x insertion nuts
- 2x screws
- 2x 3pin dupont 20cm
- 2x IR sensors from [4 Channel Infrared Sensor Module][4_channel_IR]

<table>
  <tr>
    <td valign="top">Step 1: <a href="nut_insertion.md">Insert the 2 insertion nuts into the model</a></td>
    <td valign="top"><img src="/assets/img/tutorial/front/step_1.jpg" alt="step1"  height="220"></td>
  </tr>
  <tr>
    <td valign="top">Step 2: Insert 1 LEGO pin into each corner of the front LEGO plate</td>
    <td valign="top"><img src="/assets/img/tutorial/front/step_2.jpg" alt="step2"  height="220"></td>
  </tr>
  <tr>
    <td valign="top">Step 3: Place the model on the lego pins</td>
    <td valign="top"><img src="/assets/img/tutorial/front/step_3.jpg" alt="step3"  height="220"></td>
  </tr>
  <tr>
    <td valign="top">Step 4: Screw the IR sensors into the insertion nuts</td>
    <td valign="top"><img src="/assets/img/tutorial/front/step_4.jpg" alt="step4"  height="220"></td>
  </tr>
  <tr>
    <td valign="top">Step 5: Connect the <a href="crimping_cables.md">Cables</a></td>
    <td valign="top"><img src="/assets/img/tutorial/front/step_5.jpg" alt="step5"  height="220"></td>
    <td valign="top"><img src="/assets/img/tutorial/front/cables.jpg" alt="step5"  height="220"></td>
  </tr>
  <tr>
    <td valign="top">Step 6: Place the ultrasonic sensor on top</td>
    <td valign="top"><img src="/assets/img/tutorial/front/step_6.jpg" alt="step6"  height="220"></td>
  </tr>
</table>

---

## Side Piece

**Parts:**

- 2x side holder - top piece
- 2x side holder - bottom piece
- 4x LEGO Pin type 32002
- 2x insertion nuts
- 2x screws
- 2x 3pin dupont 15cm
- 2x IR sensors from [4 Channel Infrared Sensor Module][4_channel_IR]

<table>
  <tr>
    <td valign="top">Step 1: <a href="nut_insertion.md">Insert the 2 insertion nuts into the models</a></td>
    <td valign="top"><img src="/assets/img/tutorial/side/step_1.jpg" alt="step1"  height="220"></td>
  </tr>
  <tr>
    <td valign="top">Step 2: Insert LEGO pins on the top of the LEGO plate</td>
    <td valign="top"><img src="/assets/img/tutorial/side/step_2.jpg" alt="step2"  height="220"></td>
  </tr>
  <tr>
    <td valign="top">Step 3: Place the bottom piece on the lego pieces</td>
    <td valign="top"><img src="/assets/img/tutorial/side/step_3.jpg" alt="step3"  height="220"></td>
  </tr>
  <tr>
    <td valign="top">Step 4: Place the top piece on the lego pins</td>
    <td valign="top"><img src="/assets/img/tutorial/side/step_4.jpg" alt="step4"  height="220"></td>
  </tr>
  <tr>
    <td valign="top">Step 5: Connect the <a href="crimping_cables.md">Cables</a></td>
    <td valign="top"><img src="/assets/img/tutorial/side/step_5.1.jpg" alt="step5"  height="220"></td>
    <td valign="top"><img src="/assets/img/tutorial/side/step_5.2.jpg" alt="step5"  height="220"></td>
    <td valign="top"><img src="/assets/img/tutorial/side/cables.jpg" alt="step5"  height="220"></td>
  </tr>
</table>
