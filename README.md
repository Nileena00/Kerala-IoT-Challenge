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



