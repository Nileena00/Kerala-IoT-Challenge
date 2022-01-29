# Kerala-IoT-Challenge
>**Kerala IoT Challenge 2021** is a program launched by **Foxlab Markerspace** in association with **GTech-Group Of Technology Companies** using the platform **mulearn**. The aim of this program is to bring 100 experts in IoT. It has 4 levels - includes challenges and projects. 
### About Me
>Hey Folks! I'm Nileena, student of College of Engineering, Chengannur(Electronics and Communications).This challenge will help me to learn more about IoT and to apply it in everyday life.
## Level 1
>Level 1 is  a 15 hours challenge contains 12 experiments and 2 assignments. This level gives basic knowledge about basic electronics, arduino programming. For level 1 challenge we are using Arduino UNO and its software Arduino IDE 1.8.15. You can Download & Install the Arduino IDE from  https://www.arduino.cc/en/software
>![Screenshot (105)](https://user-images.githubusercontent.com/97266374/151187925-9eb12f6a-221a-47b8-85e7-2314d960b934.png)
### Exp 1 : Hello World LED Blinking
>To blink the Led with a duration of 1 second.
#### **Components Required**
>Arduino Uno Board - 
>USB Cable - 
>LED (Any Color) x 1 Nos - 
>1 KOHM Resistor X 1 Nos - 
>BreadboardJumper Wires (Male to Male ) X 2 Nos
#### **Circuit Diagram**
>![image](https://user-images.githubusercontent.com/97266374/151189597-2f6e6784-7915-4c27-a0f3-7a244b4643e9.png)
![20220126_210026](https://user-images.githubusercontent.com/97266374/151194914-5efbfc42-b79f-44d7-8f45-c3d698885cc1.jpg)
#### **Code**
<pre>
<font color="#00979c">int</font> <font color="#000000">lp</font><font color="#434f54">=</font><font color="#000000">12</font><font color="#000000">;</font>
<font color="#00979c">void</font> <font color="#5e6d03">setup</font><font color="#000000">(</font><font color="#000000">)</font> <font color="#000000">{</font>
 &nbsp;<font color="#d35400">pinMode</font><font color="#000000">(</font><font color="#000000">lp</font><font color="#434f54">,</font> <font color="#00979c">OUTPUT</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font>

<font color="#00979c">void</font> <font color="#5e6d03">loop</font><font color="#000000">(</font><font color="#000000">)</font> <font color="#000000">{</font>
<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">lp</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">delay</font><font color="#000000">(</font><font color="#000000">1000</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">lp</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">delay</font><font color="#000000">(</font><font color="#000000">1000</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font>

</pre>
#### **Output**
>The LED is blinking for every 1 second
https://user-images.githubusercontent.com/97266374/151195012-cd43b14a-8094-4caa-a453-bbaabd8bb766.mp4

### Exp 2 : Traffic Light
>In this traffic lights experiment, we use 3 LEDs with different colors rather than 1 LED
#### **Components Required**
>Arduino Board x1 - 
USB Cable x1 - 
RED M5 LED x1 - 
YELLOW M5 LED x1 - 
GREEN M5 LED x1 - 
1KΩ Resistor x3 - 
BreadBoard x1 - 
Jumper Wire xseveral
#### **Circuit Diagram**
![image](https://user-images.githubusercontent.com/97266374/151289126-751833b6-5674-40bd-9ab2-be4bbd6658e7.png)
>![20220127_093850](https://user-images.githubusercontent.com/97266374/151291739-88fcd47a-5681-47fe-a224-aebf0377d45d.jpg)

#### **Code**
<pre>
<font color="#00979c">int</font> <font color="#000000">red</font> <font color="#434f54">=</font><font color="#000000">10</font><font color="#000000">;</font> 
<font color="#00979c">int</font> <font color="#000000">yellow</font> <font color="#434f54">=</font><font color="#000000">11</font><font color="#000000">;</font> 
<font color="#00979c">int</font> <font color="#000000">green</font> <font color="#434f54">=</font><font color="#000000">12</font><font color="#000000">;</font>
<font color="#00979c">void</font> <font color="#5e6d03">setup</font><font color="#000000">(</font><font color="#000000">)</font>
<font color="#000000">{</font>
<font color="#d35400">pinMode</font><font color="#000000">(</font><font color="#000000">red</font><font color="#434f54">,</font> <font color="#00979c">OUTPUT</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">pinMode</font><font color="#000000">(</font><font color="#000000">yellow</font><font color="#434f54">,</font> <font color="#00979c">OUTPUT</font><font color="#000000">)</font><font color="#000000">;</font> 
<font color="#d35400">pinMode</font><font color="#000000">(</font><font color="#000000">green</font><font color="#434f54">,</font> <font color="#00979c">OUTPUT</font><font color="#000000">)</font><font color="#000000">;</font> 
<font color="#000000">}</font>
<font color="#00979c">void</font> <font color="#5e6d03">loop</font><font color="#000000">(</font><font color="#000000">)</font>
<font color="#000000">{</font>
<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">green</font><font color="#434f54">,</font> <font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">delay</font><font color="#000000">(</font><font color="#000000">5000</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">green</font><font color="#434f54">,</font> <font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font> 

<font color="#5e6d03">for</font><font color="#000000">(</font><font color="#00979c">int</font> <font color="#000000">i</font><font color="#434f54">=</font><font color="#000000">0</font><font color="#000000">;</font><font color="#000000">i</font><font color="#434f54">&lt;</font><font color="#000000">3</font><font color="#000000">;</font><font color="#000000">i</font><font color="#434f54">++</font><font color="#000000">)</font>
<font color="#000000">{</font>
<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">yellow</font><font color="#434f54">,</font> <font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">delay</font><font color="#000000">(</font><font color="#000000">500</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">yellow</font><font color="#434f54">,</font> <font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">delay</font><font color="#000000">(</font><font color="#000000">500</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font> 

<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">red</font><font color="#434f54">,</font> <font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">delay</font><font color="#000000">(</font><font color="#000000">5000</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">red</font><font color="#434f54">,</font> <font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font>

</pre>
#### **Output**
Three LEDs are blinking like a traffic light with proper duration.
https://user-images.githubusercontent.com/97266374/151291779-0e19eadd-0216-495d-889f-d4c3cfa5425b.mp4

### Exp 3 : LED Chasing Effect
>In this experiment, we compile a program to simulate LED chasing effect.
#### **Components Required**
Led x5 - 
Arduino board x1 - 
1KΩ resistor x5 - 
Breadboard x1 - 
USB cablex1 - 
Breadboard wire x12
#### **Circuit Diagram**
![image](https://user-images.githubusercontent.com/97266374/151296304-517b757e-40d2-4e3c-a99e-8c77e817f361.png)
![20220127_110645](https://user-images.githubusercontent.com/97266374/151298746-e2bf835f-982a-41e2-b255-b0ede23d186e.jpg)
#### **Code**
<pre>
<font color="#00979c">int</font> <font color="#000000">start</font><font color="#434f54">=</font><font color="#000000">2</font><font color="#000000">;</font>
<font color="#00979c">int</font> <font color="#000000">num</font><font color="#434f54">=</font><font color="#000000">5</font><font color="#000000">;</font>
<font color="#00979c">void</font> <font color="#5e6d03">setup</font><font color="#000000">(</font><font color="#000000">)</font> <font color="#000000">{</font>
 &nbsp;<font color="#5e6d03">for</font><font color="#000000">(</font><font color="#00979c">int</font> <font color="#000000">i</font><font color="#434f54">=</font><font color="#000000">start</font><font color="#000000">;</font><font color="#000000">i</font><font color="#434f54">&lt;</font><font color="#000000">start</font><font color="#434f54">+</font><font color="#000000">num</font><font color="#000000">;</font><font color="#000000">i</font><font color="#434f54">++</font><font color="#000000">)</font>
 &nbsp;<font color="#d35400">pinMode</font><font color="#000000">(</font><font color="#000000">i</font><font color="#434f54">,</font><font color="#00979c">OUTPUT</font><font color="#000000">)</font><font color="#000000">;</font>

<font color="#000000">}</font>

<font color="#00979c">void</font> <font color="#5e6d03">loop</font><font color="#000000">(</font><font color="#000000">)</font> <font color="#000000">{</font>
 &nbsp;<font color="#5e6d03">for</font><font color="#000000">(</font><font color="#00979c">int</font> <font color="#000000">i</font><font color="#434f54">=</font><font color="#000000">start</font><font color="#000000">;</font><font color="#000000">i</font><font color="#434f54">&lt;</font><font color="#000000">start</font><font color="#434f54">+</font><font color="#000000">num</font><font color="#000000">;</font><font color="#000000">i</font><font color="#434f54">++</font><font color="#000000">)</font>
 &nbsp;<font color="#000000">{</font><font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">i</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;&nbsp;<font color="#d35400">delay</font><font color="#000000">(</font><font color="#000000">200</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#000000">}</font>
 &nbsp;<font color="#5e6d03">for</font><font color="#000000">(</font><font color="#00979c">int</font> <font color="#000000">i</font><font color="#434f54">=</font><font color="#000000">start</font><font color="#000000">;</font><font color="#000000">i</font><font color="#434f54">&lt;</font><font color="#000000">start</font><font color="#434f54">+</font><font color="#000000">num</font><font color="#000000">;</font><font color="#000000">i</font><font color="#434f54">++</font><font color="#000000">)</font>
 &nbsp;<font color="#000000">{</font><font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">i</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;&nbsp;<font color="#d35400">delay</font><font color="#000000">(</font><font color="#000000">200</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#000000">}</font>
<font color="#000000">}</font>

</pre>
#### **Output**
LEDs are blinking by the prrogrammed pattern.
https://user-images.githubusercontent.com/97266374/151298668-1d4783e5-6ed6-41dd-a761-5ad7c28c652c.mp4

### Exp 4 : Button Controlled LED
To controll the LED by a button switch
#### Components Required
>Arduino Uno
Button Switch x1 - 
RED M5 LED x1 - 
1KΩ Resistor x1 - 
10KΩ Resistor x1 - 
Breadboard x1 - 
Jumper wires x6  - 
USB Cable x1
#### Circuit Diagram
![image](https://user-images.githubusercontent.com/97266374/151299621-b08d93ce-7072-4e29-aa94-8bb169aed561.png)
![20220127_114123](https://user-images.githubusercontent.com/97266374/151302356-b78924d6-e3e0-420e-a95b-edbeb3af8dee.jpg)
#### Code
<pre>
<font color="#00979c">int</font> <font color="#000000">led</font><font color="#434f54">=</font><font color="#000000">11</font><font color="#000000">;</font>
<font color="#00979c">int</font> <font color="#000000">button</font><font color="#434f54">=</font><font color="#000000">7</font><font color="#000000">;</font>
<font color="#00979c">int</font> <font color="#000000">value</font><font color="#000000">;</font>
<font color="#00979c">void</font> <font color="#5e6d03">setup</font><font color="#000000">(</font><font color="#000000">)</font> <font color="#000000">{</font>
 &nbsp;<font color="#d35400">pinMode</font><font color="#000000">(</font><font color="#000000">button</font><font color="#434f54">,</font><font color="#00979c">INPUT</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">pinMode</font><font color="#000000">(</font><font color="#000000">led</font><font color="#434f54">,</font><font color="#00979c">OUTPUT</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font>

<font color="#00979c">void</font> <font color="#5e6d03">loop</font><font color="#000000">(</font><font color="#000000">)</font> <font color="#000000">{</font>
 &nbsp;<font color="#000000">value</font><font color="#434f54">=</font><font color="#d35400">digitalRead</font><font color="#000000">(</font><font color="#000000">button</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#5e6d03">if</font><font color="#000000">(</font><font color="#000000">value</font><font color="#434f54">==</font><font color="#00979c">LOW</font><font color="#000000">)</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">led</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#5e6d03">if</font><font color="#000000">(</font><font color="#000000">value</font><font color="#434f54">==</font><font color="#00979c">HIGH</font><font color="#000000">)</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">led</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font>

</pre>
#### Output
The LED is on whenever the button is pressed.
https://user-images.githubusercontent.com/97266374/151302429-b197b027-33d1-494a-bc0e-c6a84694866e.mp4

### Exp 5 : Buzzer
This experiment familarize with buzzer
#### Components Required
Arduino Uno - 
Buzzer x1 - 
Breadboard x1 - 
Breadboard Jumper Wire x2 - 
USB cable x1
#### Circuit Diagram
![image](https://user-images.githubusercontent.com/97266374/151302859-1659451c-6660-414d-bda1-8798da5fe78e.png)
![20220127_115255](https://user-images.githubusercontent.com/97266374/151303560-0e76e6e3-5ca8-4bc9-8cf3-5eb308c380e0.jpg)
#### Code
<pre>
<font color="#00979c">int</font> <font color="#000000">buz</font><font color="#434f54">=</font><font color="#000000">8</font><font color="#000000">;</font>
<font color="#00979c">void</font> <font color="#5e6d03">setup</font><font color="#000000">(</font><font color="#000000">)</font> <font color="#000000">{</font>
 &nbsp;<font color="#d35400">pinMode</font><font color="#000000">(</font><font color="#000000">buz</font><font color="#434f54">,</font><font color="#00979c">OUTPUT</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font>

<font color="#00979c">void</font> <font color="#5e6d03">loop</font><font color="#000000">(</font><font color="#000000">)</font> <font color="#000000">{</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">buz</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font> 
<font color="#000000">}</font>

</pre>
#### Output
The buzzer produces sound.
https://user-images.githubusercontent.com/97266374/151303510-aafd6f9f-d263-4527-a3e4-a745cab99c26.mp4

### Exp 6 : RGB LED 
To used a RGB LED and making diifferent colours.
#### Components Required
Arduino Uno - 
USB Cable x1 - 
RGB LED x1 - 
Resistor x3 - 
Jumper Wires x5
#### Circuit Diagram
![image](https://user-images.githubusercontent.com/97266374/151305670-249e08f0-ee9b-456f-88f3-2bed8468cb73.png)
![20220127_123147](https://user-images.githubusercontent.com/97266374/151308277-c47199d4-3533-48e1-9216-dfec0ab05969.jpg)
#### Code
<pre>
<font color="#00979c">int</font> <font color="#000000">redpin</font> <font color="#434f54">=</font> <font color="#000000">11</font><font color="#000000">;</font>
<font color="#00979c">int</font> <font color="#000000">bluepin</font> <font color="#434f54">=</font><font color="#000000">10</font><font color="#000000">;</font>
<font color="#00979c">int</font> <font color="#000000">greenpin</font> <font color="#434f54">=</font><font color="#000000">9</font><font color="#000000">;</font>
<font color="#00979c">int</font> <font color="#000000">val</font><font color="#000000">;</font>
<font color="#00979c">void</font> <font color="#5e6d03">setup</font><font color="#000000">(</font><font color="#000000">)</font> <font color="#000000">{</font>
 &nbsp;<font color="#d35400">pinMode</font><font color="#000000">(</font><font color="#000000">redpin</font><font color="#434f54">,</font> <font color="#00979c">OUTPUT</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">pinMode</font><font color="#000000">(</font><font color="#000000">bluepin</font><font color="#434f54">,</font> <font color="#00979c">OUTPUT</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">pinMode</font><font color="#000000">(</font><font color="#000000">greenpin</font><font color="#434f54">,</font> <font color="#00979c">OUTPUT</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font>
<font color="#00979c">void</font> <font color="#5e6d03">loop</font><font color="#000000">(</font><font color="#000000">)</font> 
<font color="#000000">{</font>
<font color="#5e6d03">for</font><font color="#000000">(</font><font color="#000000">val</font><font color="#434f54">=</font><font color="#000000">255</font><font color="#000000">;</font> <font color="#000000">val</font><font color="#434f54">&gt;</font><font color="#000000">0</font><font color="#000000">;</font> <font color="#000000">val</font><font color="#434f54">--</font><font color="#000000">)</font>
 &nbsp;<font color="#000000">{</font>
 &nbsp;&nbsp;<font color="#d35400">analogWrite</font><font color="#000000">(</font><font color="#000000">11</font><font color="#434f54">,</font> <font color="#000000">val</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;&nbsp;<font color="#d35400">analogWrite</font><font color="#000000">(</font><font color="#000000">10</font><font color="#434f54">,</font> <font color="#000000">255</font><font color="#434f54">-</font><font color="#000000">val</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;&nbsp;<font color="#d35400">analogWrite</font><font color="#000000">(</font><font color="#000000">9</font><font color="#434f54">,</font> <font color="#000000">128</font><font color="#434f54">-</font><font color="#000000">val</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;&nbsp;<font color="#d35400">delay</font><font color="#000000">(</font><font color="#000000">1</font><font color="#000000">)</font><font color="#000000">;</font> 
 &nbsp;<font color="#000000">}</font> 
<font color="#000000">}</font>

</pre>
#### Output
The RGB LED starts to blink within the range of 0 to 255.
https://user-images.githubusercontent.com/97266374/151308331-4938d857-6048-4c2d-957e-ae9718b31b0f.mp4

### Exp 7 : LDR Light Sensor
>The intensity of LED light is gradually increasing as the darkness increases. It uses photodiode.
#### Components Required
>Arduino Uno Board - 
Photo Resistor - 
Red M5 LED - 
10KΩ Resistor x1 - 
1KΩ Resistor x1 - 
Breadboard - 
Jumper Wire x5 - 
USB cable
#### Circuit Diagram
![Screenshot_20220128-104035_Chrome](https://user-images.githubusercontent.com/97266374/151491015-af305ee1-9164-4196-9a42-411f2ddc045b.jpg)
![20220128_093345](https://user-images.githubusercontent.com/97266374/151491025-567516e9-f2d9-4040-bddb-cca1d5585dc9.jpg)
#### Code
<pre>
<font color="#00979c">int</font> <font color="#000000">diode</font><font color="#434f54">=</font><font color="#000000">0</font><font color="#000000">;</font>
<font color="#00979c">int</font> <font color="#000000">led</font><font color="#434f54">=</font><font color="#000000">11</font><font color="#000000">;</font>
<font color="#00979c">int</font> <font color="#000000">value</font><font color="#434f54">=</font><font color="#000000">0</font><font color="#000000">;</font>
<font color="#00979c">void</font> <font color="#5e6d03">setup</font><font color="#000000">(</font><font color="#000000">)</font>
<font color="#000000">{</font>
<font color="#d35400">pinMode</font><font color="#000000">(</font><font color="#000000">diode</font><font color="#434f54">,</font><font color="#00979c">INPUT</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">pinMode</font><font color="#000000">(</font><font color="#000000">led</font><font color="#434f54">,</font><font color="#00979c">OUTPUT</font><font color="#000000">)</font><font color="#000000">;</font>
<b><font color="#d35400">Serial</font></b><font color="#434f54">.</font><font color="#d35400">begin</font><font color="#000000">(</font><font color="#000000">9600</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font>
<font color="#00979c">void</font> <font color="#5e6d03">loop</font><font color="#000000">(</font><font color="#000000">)</font>
<font color="#000000">{</font>
<font color="#000000">value</font><font color="#434f54">=</font><font color="#d35400">analogRead</font><font color="#000000">(</font><font color="#000000">diode</font><font color="#000000">)</font><font color="#000000">;</font>
<b><font color="#d35400">Serial</font></b><font color="#434f54">.</font><font color="#d35400">println</font><font color="#000000">(</font><font color="#000000">value</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#5e6d03">if</font><font color="#000000">(</font><font color="#000000">value</font><font color="#434f54">&gt;</font><font color="#000000">600</font><font color="#000000">)</font>
<font color="#d35400">analogWrite</font><font color="#000000">(</font><font color="#000000">led</font><font color="#434f54">,</font><font color="#000000">value</font><font color="#434f54">&#47;</font><font color="#000000">4</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#5e6d03">else</font>
<font color="#d35400">analogWrite</font><font color="#000000">(</font><font color="#000000">led</font><font color="#434f54">,</font><font color="#000000">value</font><font color="#434f54">&#47;</font><font color="#000000">40</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">delay</font><font color="#000000">(</font><font color="#000000">10</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font>

</pre>
#### Output
The LED brightness increases with increase in darkness
https://user-images.githubusercontent.com/97266374/151495564-c573c75a-3752-461f-bb8f-cf511c76fd10.mp4

### Exp 8 : Flame Sensor
>To beep  buzzer when there is a flame. We are using Infrared Receiver (IR )for detecting Flame.
#### Components Required
Arduino Uno Board - 
Flame Sensor - 
Buzzer - 
10K Resistor - 
Jumper Wire x6 - 
USB cable
#### Circuit Diagram
![Screenshot_20220128-122706_Chrome](https://user-images.githubusercontent.com/97266374/151501686-7ef5d745-172c-4ce2-9725-46af4650f1fa.jpg)
![20220128_122358](https://user-images.githubusercontent.com/97266374/151501605-cdc5b318-56ad-4c19-bc6e-181c8804680d.jpg)
#### Code
<pre>
<font color="#00979c">int</font> <font color="#000000">IR</font><font color="#434f54">=</font><font color="#000000">0</font><font color="#000000">;</font>
<font color="#00979c">int</font> <font color="#000000">Buz</font><font color="#434f54">=</font><font color="#000000">9</font><font color="#000000">;</font>
<font color="#00979c">int</font> <font color="#000000">value</font><font color="#434f54">=</font><font color="#000000">0</font><font color="#000000">;</font>
 <font color="#00979c">void</font> <font color="#5e6d03">setup</font><font color="#000000">(</font><font color="#000000">)</font> 
<font color="#000000">{</font>
 &nbsp;<font color="#d35400">pinMode</font><font color="#000000">(</font><font color="#000000">Buz</font><font color="#434f54">,</font><font color="#00979c">OUTPUT</font><font color="#000000">)</font><font color="#000000">;</font>
 <font color="#d35400">pinMode</font><font color="#000000">(</font><font color="#000000">IR</font><font color="#434f54">,</font><font color="#00979c">INPUT</font><font color="#000000">)</font><font color="#000000">;</font>
 <b><font color="#d35400">Serial</font></b><font color="#434f54">.</font><font color="#d35400">begin</font><font color="#000000">(</font><font color="#000000">9600</font><font color="#000000">)</font><font color="#000000">;</font>
 <font color="#000000">}</font> 
<font color="#00979c">void</font> <font color="#5e6d03">loop</font><font color="#000000">(</font><font color="#000000">)</font> 
<font color="#000000">{</font> 
 &nbsp;<font color="#000000">value</font><font color="#434f54">=</font><font color="#d35400">analogRead</font><font color="#000000">(</font><font color="#000000">IR</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<b><font color="#d35400">Serial</font></b><font color="#434f54">.</font><font color="#d35400">println</font><font color="#000000">(</font><font color="#000000">value</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#5e6d03">if</font><font color="#000000">(</font><font color="#000000">value</font><font color="#434f54">&gt;=</font><font color="#000000">600</font><font color="#000000">)</font>
 &nbsp;<font color="#000000">{</font> &nbsp;
 &nbsp;&nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">Buz</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font> 
 &nbsp;&nbsp;<font color="#000000">}</font><font color="#5e6d03">else</font> 
 &nbsp;&nbsp;<font color="#000000">{</font> &nbsp;
 &nbsp;&nbsp;&nbsp;&nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">Buz</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font> 
 &nbsp;&nbsp;&nbsp;<font color="#000000">}</font>
 &nbsp;&nbsp;<font color="#d35400">delay</font><font color="#000000">(</font><font color="#000000">500</font><font color="#000000">)</font><font color="#000000">;</font> 
<font color="#000000">}</font>

</pre>
#### Output
>The buzzer produce sound whenever there is a flame present near the IR module.
https://user-images.githubusercontent.com/97266374/151501529-f1353393-95f8-4dcd-a30d-20aa8caa7491.mp4

### Exp 9 : LM35 Temperature Sensor
To obtain and print the current temperature using LM35
>#### Components Required
>Arduino Uno  Board x1 - 
LM35 x1 - 
Breadboard x1 - 
Breadboard Jumper Wire x5 - 
USB cable
### Circuit Diagram
![Screenshot_20220128-130850_Chrome](https://user-images.githubusercontent.com/97266374/151507061-7cecde88-f58b-40b5-8917-e4fa4070c861.jpg)
![20220128_130639](https://user-images.githubusercontent.com/97266374/151507084-64560312-6fe6-4c6b-8939-2fc03244b86e.jpg)
### Code
<pre>
<font color="#00979c">int</font> <font color="#000000">lm35</font><font color="#434f54">=</font><font color="#000000">0</font><font color="#000000">;</font>
<font color="#00979c">int</font> <font color="#000000">value</font><font color="#434f54">=</font><font color="#000000">0</font><font color="#000000">;</font>
 <font color="#00979c">void</font> <font color="#5e6d03">setup</font><font color="#000000">(</font><font color="#000000">)</font> 
<font color="#000000">{</font>
 <font color="#d35400">pinMode</font><font color="#000000">(</font><font color="#000000">lm35</font><font color="#434f54">,</font><font color="#00979c">INPUT</font><font color="#000000">)</font><font color="#000000">;</font>
 <b><font color="#d35400">Serial</font></b><font color="#434f54">.</font><font color="#d35400">begin</font><font color="#000000">(</font><font color="#000000">9600</font><font color="#000000">)</font><font color="#000000">;</font>
 <font color="#000000">}</font> 
<font color="#00979c">void</font> <font color="#5e6d03">loop</font><font color="#000000">(</font><font color="#000000">)</font> 
<font color="#000000">{</font> 
 &nbsp;<font color="#000000">value</font><font color="#434f54">=</font><font color="#d35400">analogRead</font><font color="#000000">(</font><font color="#000000">lm35</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#00979c">float</font> <font color="#000000">data</font><font color="#434f54">=</font><font color="#000000">(</font><font color="#000000">125</font><font color="#434f54">*</font><font color="#000000">value</font><font color="#000000">)</font><font color="#434f54">&gt;&gt;</font><font color="#000000">8</font><font color="#000000">;</font>
 &nbsp;<b><font color="#d35400">Serial</font></b><font color="#434f54">.</font><font color="#d35400">print</font><font color="#000000">(</font><font color="#005c5f">&#34;temp= &#34;</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<b><font color="#d35400">Serial</font></b><font color="#434f54">.</font><font color="#d35400">println</font><font color="#000000">(</font><font color="#000000">data</font><font color="#000000">)</font><font color="#000000">;</font> 
 &nbsp;<font color="#d35400">delay</font><font color="#000000">(</font><font color="#000000">1000</font><font color="#000000">)</font><font color="#000000">;</font> 
<font color="#000000">}</font>

</pre>
#### Output
The temperature in degree Celcius is displayed on Serial Monitor.
https://user-images.githubusercontent.com/97266374/151506980-6d7344f1-1e31-4498-8bae-5b3659478a3b.mp4

### Exp 10:IR Remote Control Using TSOP
>To controll LED by TV remote(using IR reciever)
#### Components Required
>Arduino Uno Board - 
Infrared Remote Controller - 
Infrared Receiver - 
LED x5 - 
1KΩResistor x5 - 
Breadboard Wire - 
USB cable
#### Circuit Diagram![Screenshot_20220128-190935_Chrome](https://user-images.githubusercontent.com/97266374/151556718-8be61c4f-7172-4406-9e04-27499dc34f54.jpg)![20220128_185358](https://user-images.githubusercontent.com/97266374/151556783-6e06c4fa-90f7-4bad-baff-0260b7cebc5f.jpg)
#### Code
<pre>
<font color="#5e6d03">#include</font> <font color="#434f54">&lt;</font><font color="#000000">IRremote</font><font color="#434f54">.</font><font color="#000000">h</font><font color="#434f54">&gt;</font>
<font color="#00979c">int</font> <font color="#000000">RECV_PIN</font> <font color="#434f54">=</font> <font color="#000000">11</font><font color="#000000">;</font>
<font color="#00979c">int</font> <font color="#000000">led1</font><font color="#434f54">=</font><font color="#000000">2</font><font color="#000000">;</font>
<font color="#00979c">int</font> <font color="#000000">led2</font><font color="#434f54">=</font><font color="#000000">3</font><font color="#000000">;</font>
<font color="#00979c">int</font> <font color="#000000">led3</font><font color="#434f54">=</font><font color="#000000">4</font><font color="#000000">;</font>
<font color="#00979c">int</font> <font color="#000000">led4</font><font color="#434f54">=</font><font color="#000000">5</font><font color="#000000">;</font>
<font color="#00979c">int</font> <font color="#000000">led5</font><font color="#434f54">=</font><font color="#000000">6</font><font color="#000000">;</font>
<b><font color="#d35400">IRrecv</font></b> <font color="#000000">irrecv</font><font color="#000000">(</font><font color="#000000">RECV_PIN</font><font color="#000000">)</font><font color="#000000">;</font>
<b><font color="#d35400">decode_results</font></b> <font color="#000000">results</font><font color="#000000">;</font>

<font color="#00979c">void</font> <font color="#5e6d03">setup</font><font color="#000000">(</font><font color="#000000">)</font>
<font color="#000000">{</font>
 &nbsp;<b><font color="#d35400">Serial</font></b><font color="#434f54">.</font><font color="#d35400">begin</font><font color="#000000">(</font><font color="#000000">9600</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#000000">irrecv</font><font color="#434f54">.</font><font color="#d35400">enableIRIn</font><font color="#000000">(</font><font color="#000000">)</font><font color="#000000">;</font> <font color="#434f54">&#47;&#47; Start the receiver</font>
 &nbsp;<font color="#d35400">pinMode</font><font color="#000000">(</font><font color="#000000">led1</font><font color="#434f54">,</font><font color="#00979c">OUTPUT</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">pinMode</font><font color="#000000">(</font><font color="#000000">led2</font><font color="#434f54">,</font><font color="#00979c">OUTPUT</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">pinMode</font><font color="#000000">(</font><font color="#000000">led3</font><font color="#434f54">,</font><font color="#00979c">OUTPUT</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">pinMode</font><font color="#000000">(</font><font color="#000000">led4</font><font color="#434f54">,</font><font color="#00979c">OUTPUT</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">pinMode</font><font color="#000000">(</font><font color="#000000">led5</font><font color="#434f54">,</font><font color="#00979c">OUTPUT</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font>

<font color="#00979c">void</font> <font color="#5e6d03">loop</font><font color="#000000">(</font><font color="#000000">)</font>
<font color="#000000">{</font>
 &nbsp;<font color="#5e6d03">if</font> <font color="#000000">(</font><font color="#000000">irrecv</font><font color="#434f54">.</font><font color="#d35400">decode</font><font color="#000000">(</font><font color="#434f54">&amp;</font><font color="#000000">results</font><font color="#000000">)</font><font color="#000000">)</font>
 &nbsp;&nbsp;&nbsp;<font color="#000000">{</font>
 &nbsp;&nbsp;&nbsp;&nbsp;<b><font color="#d35400">Serial</font></b><font color="#434f54">.</font><font color="#d35400">println</font><font color="#000000">(</font><font color="#000000">results</font><font color="#434f54">.</font><font color="#000000">value</font><font color="#434f54">,</font> <font color="#00979c">HEX</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;&nbsp;&nbsp;&nbsp;<font color="#5e6d03">switch</font><font color="#000000">(</font><font color="#000000">results</font><font color="#434f54">.</font><font color="#000000">value</font><font color="#000000">)</font><font color="#000000">{</font>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<font color="#5e6d03">case</font> <font color="#000000">16</font><font color="#434f54">:</font><font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">led1</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<font color="#d35400">delay</font><font color="#000000">(</font><font color="#000000">1000</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">led1</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<font color="#5e6d03">break</font><font color="#000000">;</font>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<font color="#5e6d03">case</font> <font color="#000000">2064</font><font color="#434f54">:</font><font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">led2</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<font color="#d35400">delay</font><font color="#000000">(</font><font color="#000000">1000</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">led2</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<font color="#5e6d03">break</font><font color="#000000">;</font>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<font color="#5e6d03">case</font> <font color="#000000">1040</font><font color="#434f54">:</font><font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">led3</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<font color="#d35400">delay</font><font color="#000000">(</font><font color="#000000">1000</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">led3</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<font color="#5e6d03">break</font><font color="#000000">;</font>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<font color="#5e6d03">case</font> <font color="#000000">3088</font><font color="#434f54">:</font><font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">led4</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<font color="#d35400">delay</font><font color="#000000">(</font><font color="#000000">1000</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">led4</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<font color="#5e6d03">break</font><font color="#000000">;</font>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<font color="#5e6d03">case</font> <font color="#000000">528</font><font color="#434f54">:</font><font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">led5</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<font color="#d35400">delay</font><font color="#000000">(</font><font color="#000000">1000</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">led5</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<font color="#5e6d03">break</font><font color="#000000">;</font><font color="#000000">}</font>
 &nbsp;&nbsp;&nbsp;&nbsp;<font color="#000000">irrecv</font><font color="#434f54">.</font><font color="#d35400">resume</font><font color="#000000">(</font><font color="#000000">)</font><font color="#000000">;</font> <font color="#434f54">&#47;&#47; Receive the next value</font>
 &nbsp;&nbsp;&nbsp;<font color="#000000">}</font><font color="#d35400">delay</font><font color="#000000">(</font><font color="#000000">10</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font>
</pre>
#### Output
>LEDs are blinking by using the TV remote.
https://user-images.githubusercontent.com/97266374/151556645-4813e73e-5bf0-48c6-9876-8e5e358c09a6.mp4
### Exp 11 :Potentiometer analog Value Reading
>In this experiment we are reading value(Analog Value) from a Potentiometer
#### Components Required
Arduino Uno Board - 
10K Potentiometer -  
Breadboard - 
Breadboard Jumper Wire x3 - 
USB cable x1
#### Circuit Diagram
![image](https://user-images.githubusercontent.com/97266374/151654051-ddaeeb84-3140-4528-818c-b222817d5c5c.png)![20220128_201241](https://user-images.githubusercontent.com/97266374/151654129-0431ee87-e22d-4856-9ac8-b94636df808b.jpg)
#### Code
<pre>
<font color="#00979c">int</font> <font color="#000000">pot</font><font color="#434f54">=</font><font color="#000000">0</font><font color="#000000">;</font>
<font color="#00979c">void</font> <font color="#5e6d03">setup</font><font color="#000000">(</font><font color="#000000">)</font>
<font color="#000000">{</font>
<font color="#d35400">pinMode</font><font color="#000000">(</font><font color="#000000">pot</font><font color="#434f54">,</font><font color="#00979c">OUTPUT</font><font color="#000000">)</font><font color="#000000">;</font>
<b><font color="#d35400">Serial</font></b><font color="#434f54">.</font><font color="#d35400">begin</font><font color="#000000">(</font><font color="#000000">9600</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font>
<font color="#00979c">void</font> <font color="#5e6d03">loop</font><font color="#000000">(</font><font color="#000000">)</font>
<font color="#000000">{</font>
<font color="#00979c">int</font> <font color="#000000">val</font><font color="#434f54">=</font><font color="#d35400">analogRead</font><font color="#000000">(</font><font color="#000000">pot</font><font color="#000000">)</font><font color="#000000">;</font> 
<b><font color="#d35400">Serial</font></b><font color="#434f54">.</font><font color="#d35400">println</font><font color="#000000">(</font><font color="#000000">val</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">delay</font><font color="#000000">(</font><font color="#000000">1000</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font>

</pre>
#### Output
>The analog values of the potentiometer is displayed on the Serial Monitor.
https://user-images.githubusercontent.com/97266374/151654145-df832359-985c-4144-8a2f-a94b1ea85d9b.mp4
### Exp 12 : 7 Segment Display
> To display numbers on 7 segment display.
#### Components Required
Arduino Uno Board
1-digit LED Segment Display - 
1KΩ Resistor - 
Breadboard - 
Breadboard Jumper Wires - 
USB cable
#### Circuit Diagram
![image](https://user-images.githubusercontent.com/97266374/151656100-ec5b0b4c-56ee-4bf8-a2a6-8935dba6e432.png)![20220129_150440](https://user-images.githubusercontent.com/97266374/151656418-962dc4fe-5266-420d-a92b-759a99d45dc2.jpg)
#### Code
<pre>
<font color="#00979c">int</font> <font color="#000000">a</font><font color="#434f54">=</font><font color="#000000">2</font><font color="#000000">;</font>
<font color="#00979c">int</font> <font color="#000000">b</font><font color="#434f54">=</font><font color="#000000">3</font><font color="#000000">;</font>
<font color="#00979c">int</font> <font color="#000000">c</font><font color="#434f54">=</font><font color="#000000">4</font><font color="#000000">;</font>
<font color="#00979c">int</font> <font color="#000000">d</font><font color="#434f54">=</font><font color="#000000">5</font><font color="#000000">;</font>
<font color="#00979c">int</font> <font color="#000000">e</font><font color="#434f54">=</font><font color="#000000">6</font><font color="#000000">;</font>
<font color="#00979c">int</font> <font color="#000000">f</font><font color="#434f54">=</font><font color="#000000">7</font><font color="#000000">;</font>
<font color="#00979c">int</font> <font color="#000000">g</font><font color="#434f54">=</font><font color="#000000">8</font><font color="#000000">;</font>
<font color="#00979c">int</font> <font color="#000000">h</font><font color="#434f54">=</font><font color="#000000">9</font><font color="#000000">;</font>
<font color="#00979c">void</font> <font color="#000000">digit0</font><font color="#000000">(</font><font color="#00979c">void</font><font color="#000000">)</font>
<font color="#000000">{</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">a</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">b</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">c</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">d</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">e</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">f</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">g</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">h</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font>
<font color="#00979c">void</font> <font color="#000000">digit1</font><font color="#000000">(</font><font color="#00979c">void</font><font color="#000000">)</font>
<font color="#000000">{</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">a</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">b</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">c</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">d</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">e</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">f</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">g</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">h</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font><font color="#00979c">void</font> <font color="#000000">digit2</font><font color="#000000">(</font><font color="#00979c">void</font><font color="#000000">)</font>
<font color="#000000">{</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">a</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">b</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">c</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">d</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">e</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">f</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">g</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">h</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font><font color="#00979c">void</font> <font color="#000000">digit3</font><font color="#000000">(</font><font color="#00979c">void</font><font color="#000000">)</font>
<font color="#000000">{</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">a</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">b</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">c</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">d</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">e</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">f</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">g</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">h</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font><font color="#00979c">void</font> <font color="#000000">digit4</font><font color="#000000">(</font><font color="#00979c">void</font><font color="#000000">)</font>
<font color="#000000">{</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">a</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">b</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">c</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">d</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">e</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">f</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">g</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">h</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font><font color="#00979c">void</font> <font color="#000000">digit5</font><font color="#000000">(</font><font color="#00979c">void</font><font color="#000000">)</font>
<font color="#000000">{</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">a</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">b</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">c</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">d</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">e</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">f</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">g</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">h</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font><font color="#00979c">void</font> <font color="#000000">digit6</font><font color="#000000">(</font><font color="#00979c">void</font><font color="#000000">)</font>
<font color="#000000">{</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">a</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">b</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">c</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">d</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">e</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">f</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">g</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">h</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font><font color="#00979c">void</font> <font color="#000000">digit7</font><font color="#000000">(</font><font color="#00979c">void</font><font color="#000000">)</font>
<font color="#000000">{</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">a</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">b</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">c</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">d</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">e</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">f</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">g</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">h</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font><font color="#00979c">void</font> <font color="#000000">digit8</font><font color="#000000">(</font><font color="#00979c">void</font><font color="#000000">)</font>
<font color="#000000">{</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">a</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">b</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">c</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">d</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">e</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">f</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">g</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">h</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font><font color="#00979c">void</font> <font color="#000000">digit9</font><font color="#000000">(</font><font color="#00979c">void</font><font color="#000000">)</font>
<font color="#000000">{</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">a</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">b</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">c</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">d</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">e</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">f</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">g</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">h</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font>
 <font color="#00979c">void</font> <font color="#5e6d03">setup</font><font color="#000000">(</font><font color="#000000">)</font>
<font color="#000000">{</font>
<font color="#00979c">int</font> <font color="#000000">i</font><font color="#000000">;</font>
<font color="#5e6d03">for</font><font color="#000000">(</font><font color="#000000">i</font><font color="#434f54">=</font><font color="#000000">2</font><font color="#000000">;</font><font color="#000000">i</font><font color="#434f54">&lt;</font><font color="#000000">10</font><font color="#000000">;</font><font color="#000000">i</font><font color="#434f54">++</font><font color="#000000">)</font>
<font color="#d35400">pinMode</font><font color="#000000">(</font><font color="#000000">i</font><font color="#434f54">,</font><font color="#00979c">OUTPUT</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font> 
<font color="#00979c">void</font> <font color="#5e6d03">loop</font><font color="#000000">(</font><font color="#000000">)</font>
<font color="#000000">{</font>
<font color="#000000">digit0</font><font color="#000000">(</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">delay</font><font color="#000000">(</font><font color="#000000">1000</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">digit1</font><font color="#000000">(</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">delay</font><font color="#000000">(</font><font color="#000000">1000</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">digit2</font><font color="#000000">(</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">delay</font><font color="#000000">(</font><font color="#000000">1000</font><font color="#000000">)</font><font color="#000000">;</font> 
<font color="#000000">digit3</font><font color="#000000">(</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">delay</font><font color="#000000">(</font><font color="#000000">1000</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">digit4</font><font color="#000000">(</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">delay</font><font color="#000000">(</font><font color="#000000">1000</font><font color="#000000">)</font><font color="#000000">;</font> 
<font color="#000000">digit5</font><font color="#000000">(</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">delay</font><font color="#000000">(</font><font color="#000000">1000</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">digit6</font><font color="#000000">(</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">delay</font><font color="#000000">(</font><font color="#000000">1000</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">digit7</font><font color="#000000">(</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">delay</font><font color="#000000">(</font><font color="#000000">1000</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">digit8</font><font color="#000000">(</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">delay</font><font color="#000000">(</font><font color="#000000">1000</font><font color="#000000">)</font><font color="#000000">;</font> 
<font color="#000000">digit9</font><font color="#000000">(</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">delay</font><font color="#000000">(</font><font color="#000000">1000</font><font color="#000000">)</font><font color="#000000">;</font> 
<font color="#000000">}</font>

</pre>
#### Output 
>Digits from 0 to 9 are diaplayed on the 7 segment display.
https://user-images.githubusercontent.com/97266374/151656391-e3719767-7486-42a9-beaa-ef252d2fd486.mp4

## Assignment
### Experiment 2
Create a Digital Dice using 7 Segment Display and Push Button
#### Components Required
Arduino Board - breadboard - 1Kohm x8 resistors - 10Kohm resistor - jumper wires - USB Cable - & segment display - Push Button
#### Circuit Diagram

#### Code
<pre>
<font color="#00979c">int</font> <font color="#000000">a</font><font color="#434f54">=</font><font color="#000000">2</font><font color="#000000">;</font>
<font color="#00979c">int</font> <font color="#000000">b</font><font color="#434f54">=</font><font color="#000000">3</font><font color="#000000">;</font>
<font color="#00979c">int</font> <font color="#000000">c</font><font color="#434f54">=</font><font color="#000000">4</font><font color="#000000">;</font>
<font color="#00979c">int</font> <font color="#000000">d</font><font color="#434f54">=</font><font color="#000000">5</font><font color="#000000">;</font>
<font color="#00979c">int</font> <font color="#000000">e</font><font color="#434f54">=</font><font color="#000000">6</font><font color="#000000">;</font>
<font color="#00979c">int</font> <font color="#000000">f</font><font color="#434f54">=</font><font color="#000000">7</font><font color="#000000">;</font>
<font color="#00979c">int</font> <font color="#000000">g</font><font color="#434f54">=</font><font color="#000000">8</font><font color="#000000">;</font>
<font color="#00979c">int</font> <font color="#000000">h</font><font color="#434f54">=</font><font color="#000000">9</font><font color="#000000">;</font>
<font color="#00979c">int</font> <font color="#000000">button</font><font color="#434f54">=</font><font color="#000000">10</font><font color="#000000">;</font>
<font color="#00979c">void</font> <font color="#000000">digit1</font><font color="#000000">(</font><font color="#00979c">void</font><font color="#000000">)</font>
<font color="#000000">{</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">a</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">b</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">c</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">d</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">e</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">f</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">g</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">h</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font><font color="#00979c">void</font> <font color="#000000">digit2</font><font color="#000000">(</font><font color="#00979c">void</font><font color="#000000">)</font>
<font color="#000000">{</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">a</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">b</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">c</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">d</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">e</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">f</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">g</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">h</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font><font color="#00979c">void</font> <font color="#000000">digit3</font><font color="#000000">(</font><font color="#00979c">void</font><font color="#000000">)</font>
<font color="#000000">{</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">a</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">b</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">c</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">d</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">e</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">f</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">g</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">h</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font><font color="#00979c">void</font> <font color="#000000">digit4</font><font color="#000000">(</font><font color="#00979c">void</font><font color="#000000">)</font>
<font color="#000000">{</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">a</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">b</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">c</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">d</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">e</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">f</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">g</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">h</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font><font color="#00979c">void</font> <font color="#000000">digit5</font><font color="#000000">(</font><font color="#00979c">void</font><font color="#000000">)</font>
<font color="#000000">{</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">a</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">b</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">c</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">d</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">e</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">f</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">g</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">h</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font><font color="#00979c">void</font> <font color="#000000">digit6</font><font color="#000000">(</font><font color="#00979c">void</font><font color="#000000">)</font>
<font color="#000000">{</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">a</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">b</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">c</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">d</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">e</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">f</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">g</font><font color="#434f54">,</font><font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font><font color="#000000">(</font><font color="#000000">h</font><font color="#434f54">,</font><font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font>
<font color="#00979c">void</font> <font color="#000000">digit0</font><font color="#000000">(</font><font color="#00979c">void</font><font color="#000000">)</font>
<font color="#000000">{</font>
 &nbsp;<font color="#d35400">digitalWrite</font> <font color="#000000">(</font><font color="#000000">a</font><font color="#434f54">,</font> <font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font> <font color="#000000">(</font><font color="#000000">b</font><font color="#434f54">,</font> <font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font> <font color="#000000">(</font><font color="#000000">c</font><font color="#434f54">,</font> <font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font> <font color="#000000">(</font><font color="#000000">d</font><font color="#434f54">,</font> <font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font> <font color="#000000">(</font><font color="#000000">e</font><font color="#434f54">,</font> <font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font> <font color="#000000">(</font><font color="#000000">f</font><font color="#434f54">,</font> <font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font> <font color="#000000">(</font><font color="#000000">g</font><font color="#434f54">,</font> <font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
 &nbsp;<font color="#d35400">digitalWrite</font> <font color="#000000">(</font><font color="#000000">h</font><font color="#434f54">,</font> <font color="#00979c">HIGH</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font>
<font color="#00979c">long</font> <font color="#000000">num</font><font color="#000000">;</font>
<font color="#00979c">int</font> <font color="#000000">buttonstate</font><font color="#000000">;</font>

<font color="#00979c">void</font> <font color="#5e6d03">setup</font><font color="#000000">(</font><font color="#000000">)</font><font color="#000000">{</font>
<font color="#d35400">pinMode</font><font color="#000000">(</font><font color="#000000">a</font><font color="#434f54">,</font> <font color="#00979c">OUTPUT</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">pinMode</font><font color="#000000">(</font><font color="#000000">b</font><font color="#434f54">,</font> <font color="#00979c">OUTPUT</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">pinMode</font><font color="#000000">(</font><font color="#000000">c</font><font color="#434f54">,</font> <font color="#00979c">OUTPUT</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">pinMode</font><font color="#000000">(</font><font color="#000000">d</font><font color="#434f54">,</font> <font color="#00979c">OUTPUT</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">pinMode</font><font color="#000000">(</font><font color="#000000">e</font><font color="#434f54">,</font> <font color="#00979c">OUTPUT</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">pinMode</font><font color="#000000">(</font><font color="#000000">f</font><font color="#434f54">,</font> <font color="#00979c">OUTPUT</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">pinMode</font><font color="#000000">(</font><font color="#000000">g</font><font color="#434f54">,</font> <font color="#00979c">OUTPUT</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">pinMode</font><font color="#000000">(</font><font color="#000000">h</font><font color="#434f54">,</font> <font color="#00979c">OUTPUT</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">pinMode</font><font color="#000000">(</font><font color="#000000">button</font><font color="#434f54">,</font><font color="#00979c">INPUT</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">randomSeed</font><font color="#000000">(</font><font color="#d35400">analogRead</font><font color="#000000">(</font><font color="#000000">0</font><font color="#000000">)</font><font color="#000000">)</font><font color="#000000">;</font> 
<font color="#000000">}</font>

<font color="#00979c">void</font> <font color="#5e6d03">loop</font><font color="#000000">(</font><font color="#000000">)</font><font color="#000000">{</font>
<font color="#000000">buttonstate</font> <font color="#434f54">=</font> <font color="#d35400">digitalRead</font><font color="#000000">(</font><font color="#000000">button</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#5e6d03">if</font><font color="#000000">(</font><font color="#000000">buttonstate</font> <font color="#434f54">==</font> <font color="#00979c">LOW</font><font color="#000000">)</font><font color="#000000">{</font>
<font color="#000000">num</font> <font color="#434f54">=</font> <font color="#d35400">random</font><font color="#000000">(</font><font color="#000000">1</font><font color="#434f54">,</font><font color="#000000">7</font><font color="#000000">)</font><font color="#000000">;</font> 
<font color="#5e6d03">if</font> <font color="#000000">(</font><font color="#000000">num</font> <font color="#434f54">==</font> <font color="#000000">1</font><font color="#000000">)</font><font color="#000000">{</font>
<font color="#000000">digit1</font><font color="#000000">(</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">delay</font><font color="#000000">(</font><font color="#000000">2000</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">digit0</font><font color="#000000">(</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font>
<font color="#5e6d03">if</font> <font color="#000000">(</font><font color="#000000">num</font> <font color="#434f54">==</font> <font color="#000000">2</font><font color="#000000">)</font><font color="#000000">{</font>
<font color="#000000">digit2</font><font color="#000000">(</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">delay</font><font color="#000000">(</font><font color="#000000">2000</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">digit0</font><font color="#000000">(</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font>
<font color="#5e6d03">if</font> <font color="#000000">(</font><font color="#000000">num</font> <font color="#434f54">==</font> <font color="#000000">3</font><font color="#000000">)</font><font color="#000000">{</font>
<font color="#000000">digit3</font><font color="#000000">(</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">delay</font><font color="#000000">(</font><font color="#000000">2000</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">digit0</font><font color="#000000">(</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font>
<font color="#5e6d03">if</font> <font color="#000000">(</font><font color="#000000">num</font> <font color="#434f54">==</font> <font color="#000000">4</font><font color="#000000">)</font><font color="#000000">{</font>
<font color="#000000">digit4</font><font color="#000000">(</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">delay</font><font color="#000000">(</font><font color="#000000">2000</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">digit0</font><font color="#000000">(</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font>
<font color="#5e6d03">if</font> <font color="#000000">(</font><font color="#000000">num</font> <font color="#434f54">==</font> <font color="#000000">5</font><font color="#000000">)</font><font color="#000000">{</font>
<font color="#000000">digit5</font><font color="#000000">(</font><font color="#000000">)</font><font color="#000000">;</font> &nbsp;
<font color="#d35400">delay</font><font color="#000000">(</font><font color="#000000">2000</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">digit0</font><font color="#000000">(</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font>
<font color="#5e6d03">if</font> <font color="#000000">(</font><font color="#000000">num</font> <font color="#434f54">==</font> <font color="#000000">6</font><font color="#000000">)</font><font color="#000000">{</font>
<font color="#000000">digit6</font><font color="#000000">(</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#d35400">delay</font><font color="#000000">(</font><font color="#000000">2000</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">digit0</font><font color="#000000">(</font><font color="#000000">)</font><font color="#000000">;</font>
<font color="#000000">}</font>
<font color="#000000">}</font>
<font color="#000000">}</font>

</pre>
