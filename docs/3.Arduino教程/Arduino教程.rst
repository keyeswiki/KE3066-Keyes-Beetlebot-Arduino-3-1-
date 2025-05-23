Arduino教程
===========

开发环境设置
------------

\ **注意：**
扩展板上标注的G、GND表示电源负极，可连接传感器的G、GND、—等负极接口；标注的V、VCC为电源正极（此扩展板上的电源为5V），可连接传感器的V、VCC、+
等5V电源接口。

--------------

安装开发软件和驱动
~~~~~~~~~~~~~~~~~~

安装Arduino IDE（Windows）
^^^^^^^^^^^^^^^^^^^^^^^^^^

我们先到Arduino官方的网站：\ https://www.arduino.cc/en/software/

下载最新版本的arduino开发软件，Arduino 软件有很多版本，有wodows,mac
linux系统的（如下图），而且还有过去老的版本，你只需要下载一个适合系统的版本即可。

|img|

--------------

这里我们以Windows系统的为例给大家介绍下载和安装的步骤。Windows系统的也有两个版本，一个版本是安装版的，一个是下载版的不用安装，直接下载文件到电脑，解压缩就可以用了。

|image1|

一般情况下，我们点击JUST
DOWNLOAD就可以下载了，当然，如果你愿意，你可以选择小小的赞助一下，以帮助伟大的Arduino
开源事业。

--------------

安装Arduino IDE（Mac）
^^^^^^^^^^^^^^^^^^^^^^

不同的系统，需要下载不同的Arduino
IDE，下载方式和5.1.1章节类似。选择如下图。

|image2|

--------------

安装开发板驱动文件
^^^^^^^^^^^^^^^^^^

**在Windows系统电脑详细使用方法**

安装Arduino
IDE后，我们就开始安装驱动。将控制板用USB线连接在电脑上后，如果是Windows10系统电脑，电脑会自动安装驱动。如果是其他系统电脑，如Windows7系统电脑，需要手动安装驱动。

控制板的USB转串口芯片为CH340我们需要安装这芯片的驱动，驱动为usb_ch341_3.1.2009.06。我们在对应的资料位置中提供有驱动文件。

|image3|

第一次将控制板连接电脑时，点击计算机--属性--设备管理器，显示如下图。

|image4|

--------------

点击USB Serial后，点击“更新驱动程序”，开始安装驱动，如下图。

|image5|

--------------

进入下图，选择浏览我的电脑以查找驱动程序。

|image6|

--------------

在电脑中找到usb_ch341_3.1.2009.06文件夹。

|image7|

--------------

安装驱动完成，出现下图点击关闭，之后就会出现串口号了。

|image8|

--------------

这样驱动就装好了。点击计算机--属性--设备管理器，我们可看见如下图。

|image9|

--------------

**在 MAC 系统电脑详细使用方法**

请参考以下链接:

https://wiki.keyestudio.com/Download_CH340_Driver_on_MAC_System

|image10|

控制板的USB转串口芯片为CH340我们需要安装这芯片的驱动，我们在对应的资料位置中也提供有驱动文件。

|Img|

--------------

Arduino IDE设置和工具栏介绍
^^^^^^^^^^^^^^^^^^^^^^^^^^^

**在 Windows 系统电脑详细使用方法**

装好了开发板的驱动，我们下面了解Arduino软件的使用，首先我们打开Arduino
IDE软件。

|image11|

--------------

选择正确的Arduino板，与连接到计算机的电路板相匹配。转到Tools→Board，选择Arduino
NANO。

|image12|

--------------

然后再选择正确的COM口（安装驱动成功后，可看到对应COM口），这样就算连接成功了。

|image13|

--------------

**在MAC系统电脑详细使用方法**

在 Arduino IDE设置时，方法和Windows
系统类似，只是设置COM口时不同，如下图。

|image14|

--------------

**启动你的第一个程序**

上面我们学习了怎么下载软件和安装开发板的驱动，那下面我们就开始正式开始第一个程序，打开文件选择例子，选择第一个文件BASIC里面的BLINK程序。

|image15|

--------------

按照前面方法设置板和COM口，IDE右下角显示对应板和COM口。点击左上角的“√”图标开始编译程序，检查错误，也可以点击“→”一键编译并上传到开发板。

|image16|

--------------

上传成功如下图。

|image17|

程序上传成功，板载的LED灯亮一秒钟，灭一秒钟，恭喜你的第一个程序完成了。Arduino编程语言可以分为三个主要部分：函数、值（变量和常量）和结构。具体参考请查看Arduino官网教程:
https://www.arduino.cc/reference/en/

--------------

安装库文件
~~~~~~~~~~

在开始课程之前我们还需要安装课程里面代码需要的Arduino库文件。

**什么是arduino库文件 ?**

库是代码的集合，使您可以轻松地连接到传感器、显示器、模块等。

例如，内置的LiquidCrystal库使与字符LCD显示器的通话变得容易，Internet上有数百个其他库可供下载。参考中列出了内置库和手动添加的库。

--------------

**如何安装库文件?**

我们在对应文件资料路径中提供有本套件Arduino教程所需的所有库文件。如下所示：

|image18|

在这里，我们将为您介绍最简单的添加库的方法。首先，依次点击右上角的
**项目** > **导入库** > **添加.Zip 库...** 。

|image19|

--------------

再选择文件中，找到自己需要的库压缩包.zip格式，点击确定即可添加成功，添加成功后消息栏会显示“Library
installed”。这里是以“Adafruit_NeoPixel”库文件为例，其他的库文件添加方法一样，就不多重复。

|image20|

|image21|

更多教程与产品，请访问本公司官网: http://www.keyes-robot.com/

--------------

小车原生态安装步骤
------------------

在安装过程中，会有烧录代码的过程，请先安装软件部分，如果已经完成，接下来就开始实物的安装吧。一共分为20个小步骤，可分为椴木板安装和开发板接线两大类，还请拿出100%的精神，集中注意力，尽情享受动手创造的快乐吧！

--------------

|image22|

步骤 1

--------------

1.1

|image23|

--------------

1.2

|image24|

--------------

1.3

完成

|image25|

--------------

步骤 2

--------------

2.1

|image26|

--------------

2.2

|image27|

--------------

2.3

|image28|

--------------

步骤 3

--------------

3.1

|image29|

--------------

3.2

|image30|

--------------

3.3

|image31|

--------------

步骤 4

--------------

4.1

|image32|

--------------

4.2

|image33|

--------------

4.3

|image34|

--------------

步骤 5

--------------

5.1

|image35|

--------------

5.2

======== ================
模块     接口
======== ================
左边电机 （L） 2.54mm端子
右边电机 （R） 2.54mm端子
======== ================

**接线时，请注意区分线材颜色，传感器S接黄色，V接红色，G接黑色**

|image36|

--------------

5.3

将8*8点阵，通过杜邦线连接PCB底板。

======== ======================================
所需线材 4P 杜邦母对母连拼 100mm （黑红蓝绿线）
======== ======================================
======== ======================================

|image37|

8*8点阵接线表：

=========== ===========
8*8点阵模块 PCB底板
=========== ===========
G（黑色）   G（黑色）
5V（红色）  5V（红色）
SDA（蓝色） SDA（蓝色）
SCL（绿色） SCL（绿色）
=========== ===========

然后将电机、8*8点阵屏用连接线，连接上下两块 PCB板，如下。

|image38|

--------------

5.4

|image39|

--------------

5.5

|image40|

--------------

步骤 6

--------------

6.1

|image41|

--------------

6.2

|image42|

--------------

6.3

|image43|

--------------

步骤 7

--------------

7.1

|image44|

--------------

7.2

|image45|

--------------

7.3

|image46|

--------------

步骤 8

--------------

8.1

|image47|

--------------

8.2

|image48|

--------------

8.3

|image49|

--------------

步骤 9

--------------

9.1

|image50|

--------------

9.2

|image51|

--------------

**安装舵机前，舵机角度调节到90度，通过烧录代码进行调节，通过arduino编译器进行。**

- 用舵机连接到小车的扩展板，连接扩展板上的引脚S1（D9）。

|image52|

- 我们提供的示例代码的路径如下：

|image53|

.. code:: C

   /*
    * 名称   : 180_Servo_Angle_initialization
    * 功能   : 舵机旋转角度0 -> 180 -> 90
    * 作者   : http://www.keyes-robot.com/ 
   */
   #include <Servo.h>

   Servo myservo;  //创建舵机对象来控制舵机

   int servoPin = 9;  // 定义舵机引脚D5

   void setup() {
     myservo.attach(servoPin);  //选择舵机引脚D9
     myservo.write(0); //旋转到0度
     delay(1000); //延迟1s
     myservo.write(180); //旋转到180度
     delay(1000); //延迟1s
     myservo.write(90); //旋转到90度
     delay(1000); //延迟1s
   }

   void loop() {
   }

- 用\ **Arduino
  IDE**\ 打开\ **180_Servo_Angle_initialization.ino**\ ，并上传至NANO开发板。

  |image54|

- 舵机将会调整到90度。

--------------

9.3

**开始安装舵机**

|image55|

--------------

9.4

|image56|

--------------

9.5

|image57|

--------------

步骤 10

--------------

10.1

|image58|

--------------

10.2

|image59|

--------------

10.3

|image60|

--------------

10.4

**此步骤需要使用杜邦线，连接超声波传感器。**

============ =====================
模块         线材
============ =====================
超声波传感器 4PIN **（黑红蓝绿）**
============ =====================

|image61|

- 先接超声波模块，\ **接线时，请注意区分线材颜色，Vcc接红色，Trig接蓝色，Echo接绿色，Gnd接黑色,**

  请务必要接线正确，否则发生短路，会烧坏超声波传感器！！

  |image62|

  --------------

  超声波线另一端，接小车扩展板上。

  |image63|

  --------------

  |image64|

  --------------

10.5

**此步骤需要使用杜邦线，连接两个光敏传感器。**

========== ====
模块       线材
========== ====
光敏传感器 3PIN
========== ====

|image65|

- 先连接光敏传感器，请注意，\ **黄色线连接S，红色线连接V，黑色线连接G**\ 。

  |image66|

  --------------

- 再把传感器连接到小车扩展板，请注意，\ **黄色线连接S，红色线连接V，黑色线连接G**\ 。

  |image67|

  --------------

  |image68|

--------------

步骤 11

--------------

11.1

**所需零件**

|image69|

--------------

11.2

|image70|

--------------

11.3

|image71|

--------------

11.4

|image72|

--------------

步骤 12

--------------

12.1

使用缠绕管，把线全部整理起来。

|image73|

--------------

|image74|

--------------

完成

|image75|

--------------

项目教程
--------

Project 01: LED Blinking
~~~~~~~~~~~~~~~~~~~~~~~~

**实验简介**

在前面的准备工作中，知道我们Arduino
Nano主板上有个板载LED(L)，而且我们已经知道这个LED是连接在Arduino
Nano主板上的D13，在本实验中，我们让这个LED闪烁起来。LED闪烁对于学习Arduino的爱好者而言，是最基础的实验项目，也是新手必须经历的一个练习。

--------------

**元件知识**

**板载LED：**
LED是一种被称为“发光二极管”的半导体，是一种由半导体材料(硅、硒、锗等)制成的电子器件。它的控制方法非常简单，通过控制Arduino
Nano主板上IO口（D13）的高低电平，来使LED灯亮灭。

|image76|

--------------

**实验代码**

.. code:: c++

   /*
     Project 01 LED Blinking
     Turns an LED on for one second, then off for one second, repeatedly.
   */
   int ledPin=13; //Define LED pin to D13
   // the setup function runs once when you press reset or power the board

   void setup() 
   {
     // initialize digital pin LED_BUILTIN as an output.
     pinMode(ledPin, OUTPUT);
   }

   // the loop function runs over and over again forever
   void loop() 
   {
     digitalWrite(ledPin, HIGH);   // turn the LED on (HIGH is the voltage level)
     delay(1000);                       // wait for a second
     digitalWrite(ledPin, LOW);    // turn the LED off by making the voltage LOW
     delay(1000);                       // wait for a second
   }

--------------

**实验现象**

将实验代码上传至Arduino Nano主板上，利用USB线上电后，Arduino
Nano主板上的板载LED就闪烁起来。

Project 02: 6812 RGB
~~~~~~~~~~~~~~~~~~~~

|image77|

**实验简介**

小车扩展板上有4个RGB LED，RGB
LED属于简单的发光模块，可以通过调节色彩调出不同颜色的灯效，可广泛应用于建筑物、桥梁、道路、花园、庭院、地板等领域的装饰照明与会场布置、圣诞节、万圣节、情人节、复活节、国庆节等节日期间烘托气氛等场景。在本实验中，使小车扩展板上的4个RGB实现各种灯光效果。

--------------

**元件知识**

**SK6812RGB：** 小车扩展板上有4个RGB
LED，从原理图中可以看出，这4个RGBLED都是串联起来的，在电压电流充足的情况下可以接几百个RGB
LED，都可以用一根信号线控制任意一个RGB
LED，并且让它显示任意一种颜色。每一颗RGBLED都是一个独立的像素点，每个像素点都是由R、G、B三基色颜色组成，可实现256级亮度显示，完成16777216种颜色的全真色彩显示，同时像素点内部包含了智能数字接口数据锁存信号整形放大驱动电路，还内置信号整形电路，有效保证了像素点光的颜色高度一致。

|image78|

--------------

**实验代码**

.. code:: c++

   //*************************************************************************************
   /*
     Project 02 SK6812 RGB
     4 RGBs for various lighting effects.
   */
   #include <Adafruit_NeoPixel.h>

   #define PIN A3

   // Parameter 1 = number of pixels in strip
   // Parameter 2 = Arduino pin number (most are valid)
   // Parameter 3 = pixel type flags, add together as needed:
   //   NEO_KHZ800  800 KHz bitstream (most NeoPixel products w/WS2812 LEDs)
   //   NEO_KHZ400  400 KHz (classic 'v1' (not v2) FLORA pixels, WS2811 drivers)
   //   NEO_GRB     Pixels are wired for GRB bitstream (most NeoPixel products)
   //   NEO_RGB     Pixels are wired for RGB bitstream (v1 FLORA pixels, not v2)
   Adafruit_NeoPixel strip = Adafruit_NeoPixel(4, PIN, NEO_GRB + NEO_KHZ800);

   // IMPORTANT: To reduce NeoPixel burnout risk, add 1000 uF capacitor across
   // pixel power leads, add 300 - 500 Ohm resistor on first pixel's data input
   // and minimize distance between Arduino and first pixel.  Avoid connecting
   // on a live circuit...if you must, connect GND first.

   void setup() {
     strip.begin();
     strip.show(); // Initialize all pixels to 'off'
   }

   void loop() {
     // Some example procedures showing how to display to the pixels:
     colorWipe(strip.Color(255, 0, 0), 50); // Red
     colorWipe(strip.Color(0, 255, 0), 50); // Green
     colorWipe(strip.Color(0, 0, 255), 50); // Blue
     // Send a theater pixel chase in...
     theaterChase(strip.Color(127, 127, 127), 50); // White
     theaterChase(strip.Color(127,   0,   0), 50); // Red
     theaterChase(strip.Color(  0,   0, 127), 50); // Blue

     rainbow(20);
     rainbowCycle(20);
     theaterChaseRainbow(50);
   }

   // Fill the dots one after the other with a color
   void colorWipe(uint32_t c, uint8_t wait) {
     for(uint16_t i=0; i<strip.numPixels(); i++) {
         strip.setPixelColor(i, c);
         strip.show();
         delay(wait);
     }
   }

   void rainbow(uint8_t wait) {
     uint16_t i, j;

     for(j=0; j<256; j++) {
       for(i=0; i<strip.numPixels(); i++) {
         strip.setPixelColor(i, Wheel((i+j) & 255));
       }
       strip.show();
       delay(wait);
     }
   }

   // Slightly different, this makes the rainbow equally distributed throughout
   void rainbowCycle(uint8_t wait) {
     uint16_t i, j;

     for(j=0; j<256*5; j++) { // 5 cycles of all colors on wheel
       for(i=0; i< strip.numPixels(); i++) {
         strip.setPixelColor(i, Wheel(((i * 256 / strip.numPixels()) + j) & 255));
       }
       strip.show();
       delay(wait);
     }
   }

   //Theatre-style crawling lights.
   void theaterChase(uint32_t c, uint8_t wait) {
     for (int j=0; j<10; j++) {  //do 10 cycles of chasing
       for (int q=0; q < 3; q++) {
         for (int i=0; i < strip.numPixels(); i=i+3) {
           strip.setPixelColor(i+q, c);    //turn every third pixel on
         }
         strip.show();
        
         delay(wait);
        
         for (int i=0; i < strip.numPixels(); i=i+3) {
           strip.setPixelColor(i+q, 0);        //turn every third pixel off
         }
       }
     }
   }

   //Theatre-style crawling lights with rainbow effect
   void theaterChaseRainbow(uint8_t wait) {
     for (int j=0; j < 256; j++) {     // cycle all 256 colors in the wheel
       for (int q=0; q < 3; q++) {
           for (int i=0; i < strip.numPixels(); i=i+3) {
             strip.setPixelColor(i+q, Wheel( (i+j) % 255));    //turn every third pixel on
           }
           strip.show();
          
           delay(wait);
          
           for (int i=0; i < strip.numPixels(); i=i+3) {
             strip.setPixelColor(i+q, 0);        //turn every third pixel off
           }
       }
     }
   }

   // Input a value 0 to 255 to get a color value.
   // The colours are a transition r - g - b - back to r.
   uint32_t Wheel(byte WheelPos) {
     if(WheelPos < 85) {
      return strip.Color(WheelPos * 3, 255 - WheelPos * 3, 0);
     } else if(WheelPos < 170) {
      WheelPos -= 85;
      return strip.Color(255 - WheelPos * 3, 0, WheelPos * 3);
     } else {
      WheelPos -= 170;
      return strip.Color(0, WheelPos * 3, 255 - WheelPos * 3);
     }
   }
   //*************************************************************************************

**实验现象**

将实验代码上传至Arduino Nano主板上，利用USB线上电后，小车PCB板上的4个RGB
LED实现各种灯光效果。

Project 03: 演奏音乐
~~~~~~~~~~~~~~~~~~~~

**实验简介**

小车扩展板上有个喇叭功放元件，它常用来播放音乐，作为一些音乐播放设备的外接扩音设备。

在本实验中，我们利用喇叭功放元件来播放一首音乐。

--------------

**元件知识**

**\*喇叭功放元件：\***
喇叭功放元件（原理相当于无源蜂鸣器），其内部不带震荡电路，控制时需要在元件正极输入不同频率的方波，负极接地，从而控制喇叭功放元件响起不同频率的声音。

--------------

**实验代码：**

.. code:: c++

   //*********************************************************************************
   /*
   Project 03 Buzzer
   Buzzer plays music
   */
   #define NOTE_B0  31
   #define NOTE_C1  33
   #define NOTE_CS1 35
   #define NOTE_D1  37
   #define NOTE_DS1 39
   #define NOTE_E1  41
   #define NOTE_F1  44
   #define NOTE_FS1 46
   #define NOTE_G1  49
   #define NOTE_GS1 52
   #define NOTE_A1  55
   #define NOTE_AS1 58
   #define NOTE_B1  62
   #define NOTE_C2  65
   #define NOTE_CS2 69
   #define NOTE_D2  73
   #define NOTE_DS2 78
   #define NOTE_E2  82
   #define NOTE_F2  87
   #define NOTE_FS2 93
   #define NOTE_G2  98
   #define NOTE_GS2 104
   #define NOTE_A2  110
   #define NOTE_AS2 117
   #define NOTE_B2  123
   #define NOTE_C3  131
   #define NOTE_CS3 139
   #define NOTE_D3  147
   #define NOTE_DS3 156
   #define NOTE_E3  165
   #define NOTE_F3  175
   #define NOTE_FS3 185
   #define NOTE_G3  196
   #define NOTE_GS3 208
   #define NOTE_A3  220
   #define NOTE_AS3 233
   #define NOTE_B3  247
   #define NOTE_C4  262
   #define NOTE_CS4 277
   #define NOTE_D4  294
   #define NOTE_DS4 311
   #define NOTE_E4  330
   #define NOTE_F4  349
   #define NOTE_FS4 370
   #define NOTE_G4  392
   #define NOTE_GS4 415
   #define NOTE_A4  440
   #define NOTE_AS4 466
   #define NOTE_B4  494
   #define NOTE_C5  523
   #define NOTE_CS5 554
   #define NOTE_D5  587
   #define NOTE_DS5 622
   #define NOTE_E5  659
   #define NOTE_F5  698
   #define NOTE_FS5 740
   #define NOTE_G5  784
   #define NOTE_GS5 831
   #define NOTE_A5  880
   #define NOTE_AS5 932
   #define NOTE_B5  988
   #define NOTE_C6  1047
   #define NOTE_CS6 1109
   #define NOTE_D6  1175
   #define NOTE_DS6 1245
   #define NOTE_E6  1319
   #define NOTE_F6  1397
   #define NOTE_FS6 1480
   #define NOTE_G6  1568
   #define NOTE_GS6 1661
   #define NOTE_A6  1760
   #define NOTE_AS6 1865
   #define NOTE_B6  1976
   #define NOTE_C7  2093
   #define NOTE_CS7 2217
   #define NOTE_D7  2349
   #define NOTE_DS7 2489
   #define NOTE_E7  2637
   #define NOTE_F7  2794
   #define NOTE_FS7 2960
   #define NOTE_G7  3136
   #define NOTE_GS7 3322
   #define NOTE_A7  3520
   #define NOTE_AS7 3729
   #define NOTE_B7  3951
   #define NOTE_C8  4186
   #define NOTE_CS8 4435
   #define NOTE_D8  4699
   #define NOTE_DS8 4978
   #define REST 0
   int tempo=114; // change this to make the song slower or faster
   int buzzer = 3;// initializes  digital I/O PIN to control the buzzer
   // notes of the moledy followed by the duration
   // a 4 means a quarter note, 8 an eighteenth , 16 sixteenth, so on
   //  !!negative numbers are used to represent dotted notes
   //  so -4 means a dotted quarter note, that is, a quarter plus an eighteenth
   int melody[] = {
     NOTE_E4,4,  NOTE_E4,4,  NOTE_F4,4,  NOTE_G4,4,//1
     NOTE_G4,4,  NOTE_F4,4,  NOTE_E4,4,  NOTE_D4,4,
     NOTE_C4,4,  NOTE_C4,4,  NOTE_D4,4,  NOTE_E4,4,
     NOTE_E4,-4, NOTE_D4,8,  NOTE_D4,2,
     NOTE_E4,4,  NOTE_E4,4,  NOTE_F4,4,  NOTE_G4,4,//4
     NOTE_G4,4,  NOTE_F4,4,  NOTE_E4,4,  NOTE_D4,4,
     NOTE_C4,4,  NOTE_C4,4,  NOTE_D4,4,  NOTE_E4,4,
     NOTE_D4,-4,  NOTE_C4,8,  NOTE_C4,2,
     NOTE_D4,4,  NOTE_D4,4,  NOTE_E4,4,  NOTE_C4,4,//8
     NOTE_D4,4,  NOTE_E4,8,  NOTE_F4,8,  NOTE_E4,4, NOTE_C4,4,
     NOTE_D4,4,  NOTE_E4,8,  NOTE_F4,8,  NOTE_E4,4, NOTE_D4,4,
     NOTE_C4,4,  NOTE_D4,4,  NOTE_G3,2,
     NOTE_E4,4,  NOTE_E4,4,  NOTE_F4,4,  NOTE_G4,4,//12
     NOTE_G4,4,  NOTE_F4,4,  NOTE_E4,4,  NOTE_D4,4,
     NOTE_C4,4,  NOTE_C4,4,  NOTE_D4,4,  NOTE_E4,4,
     NOTE_D4,-4,  NOTE_C4,8,  NOTE_C4,2
   };
   // sizeof gives the number of bytes, each int value is composed of two bytes (16 bits)
   // there are two values per note (pitch and duration), so for each note there are four bytes
   int notes=sizeof(melody)/sizeof(melody[0])/2; 
   // this calculates the duration of a whole note in ms (60s/tempo)*4 beats
   int wholenote = (60000 * 4) / tempo;
   int divider = 0, noteDuration = 0;
   void setup() {
     // iterate over the notes of the melody
     // remember, the array is twice the number of notes (notes + durations)
     for (int thisNote = 0; thisNote < notes * 2; thisNote = thisNote + 2) {
       // calculates the duration of each note
       divider = melody[thisNote + 1];
       if (divider > 0) {
       noteDuration = (wholenote) / divider; // regular note, just proceed
       } else if (divider < 0) {
         // dotted notes are represented with negative durations!!
         noteDuration = (wholenote) / abs(divider);
         noteDuration *= 1.5; // increases the duration in half for dotted notes
       }
       // we only play the note for 90% of the duration, leaving 10% as a pause
       tone(buzzer, melody[thisNote], noteDuration*0.9);
     // Wait for the specief duration before playing the next note
       delay(noteDuration);
       noTone(buzzer);  //  stop the waveform generation before the next note
     }
   }
   void loop() {
   // if you want to repeat the song forever, 
   // just paste the setup code here instead.
   }
   //*********************************************************************************

--------------

**实验现象**

将实验代码上传至Arduino
Nano主板上，利用USB线上电后，小车PCB板上的喇叭功放元件就开始播放一首音乐。

Project 04: 8*8点阵
~~~~~~~~~~~~~~~~~~~

**实验简介：**

|image-20230701141308990|

8*8
点阵屏通过LED(发光二极管）组成，以灯珠亮灭来显示文字、图片、动画、视频等，8*8
点阵显示屏制作简单，安装方便，被广泛应用于各种公共场合，如汽车报站器、广告屏、银行窗口屏、叫号屏以及停车系统等等。在本实验中，将使用8*8
点阵屏来显示图案。

--------------

**元件知识**

**8*8点阵屏：**
LED点阵屏按照LED发光颜色可分为单色、双色、三色灯等，可显示红、黄、绿甚至是真彩色。根据LED的数量又分为4×4、8×8、16×16等不同类型。这里我们通过单色8×8点阵屏来了解其原理。

不同点阵屏封装不同，8×8点阵屏由8行8列共64个LED灯组成，其内部结构如下图：

|image79|

每个LED放置在行线和列线的交叉点上，当对应的某一行电平拉高，某一列电拉低，则对应交叉点的LED就会点亮。8×8点阵屏有16个管脚，将有丝印的一边朝下，逆时针编号为1-8，9-16。

|image80|

其对应内部管脚定义如下如所示：

|image81|

比如我们要点亮第一行第一列LED灯，则对应将点阵屏的第9脚拉高，第13脚拉低，其他LED控制以此类推即可。

HT16K33：8X8点阵驱动模块：上面介绍了8\ *8点阵的原理，想控制8*\ 8点阵需要多达16个单片机的引脚。这样既浪费资源也浪费时间。这里用了一个驱动点阵屏的芯片：HT16K33。HT16K33是一款内存映射和多功能LED控制器驱动芯片。利用HT16K33芯片驱动1个8*8点阵，只需要利用单片机的I2C通信端口控制点阵，大大的节约了单片机资源。下图是HT16K33
芯片工作原理图。

|image82|

我们基于以上原理设计了一个8X8点阵驱动模块，从上图我们可以看出，我们只要通过I2C
通讯利用单片机的2个引脚就可以很好的控制点阵显示。

**8X8点阵模块的参数：**

- 工作电压: 5V

- 额定输入频率: 400KHZ

- 输入功率: 2.5W

- 输入电流: 500mA

**取模工具的使用说明：**

点阵和驱动的原理都已经介绍完了，那点阵上显示的内容是怎么来的呢，有没有比较简便的方法？这里给大家介绍一款点阵取模工具，这块工具使用的是在线版，链接：\ http://dotmatrixtool.com/#

现在就一起看看怎么使用吧。

①打开链接如下图：

|image83|

②我们的点阵是8*8的，所以调整高度为8，宽度为8，如下图：

|image84|

③在****Byte order***\* 这里选择****Row major***\* 这个模式

|image85|

④将图案生成16进制的数据

如下图，按鼠标左键选中，右键取消，画好自己想要的图案，点击****Generate***\*，就会生成我们所需要的十六进制的数据了,

|image86|

这个生成的十六进制的代码（0x00, 0x66, 0x00, 0x00, 0x18, 0x42, 0x3c,
0x00）就是我们需要显示的内容，我们先保存好，等一下需要放到程序里面。

**实验接线**

======= =========
8*8点阵 小车PCB板
======= =========
G       G
5V      5V
SDA     SDA
SCL     SCL
======= =========

**实验代码**

.. code:: c++

   //*************************************************************************************
   /*
    Project 04 8*8 Dot Matrix
    8*8 dot matrix screen to display patterns
   */ 
   #include <ks_Matrix.h>
   Matrix myMatrix(A4,A5);    //set pins to communication pins
   // define an array
   uint8_t LedArray1[8]={0x00, 0x66, 0x00, 0x00, 0x18, 0x42, 0x3c, 0x00};  
   uint8_t  LEDArray[8]; //define an array(by modulus tool) without initial value

   void setup(){
     myMatrix.begin(0x70);  //communication address
     myMatrix.clear();    //clear matrix
   }

   void loop(){
     for(int i=0; i<8; i++)  // there is eight data, loop for eight times
     {
   LEDArray[i]=LedArray1[i];  //Call the emoticon array data in the subroutine LEDArray
   for(int j=7; j>=0; j--)  //Every data(byte) has 8 bit, therefore, loop for eight times
       {
         if((LEDArray[i]&0x01)>0) //judge if the last bit of data is greater than 0
         {
           myMatrix.drawPixel(j, i,1);  //light up the corresponding point
         }
         else  //otherwise
         {
           myMatrix.drawPixel(j, i,0);  //turn off the corresponding point
         }
         LEDArray[i] = LEDArray[i]>>1;  //LEDArray[i] moves right for one bit to judge the previous one bit
       }
     }
     myMatrix.writeDisplay();  // dot matrix shows
   }
   //*****************************************

**实验现象**

将实验代码上传至Arduino
Nano主板上，利用USB线上电后，小车前的8*8点阵屏显示“笑脸”图案。

|img-20230531141128|

Project 05: 舵机转动
~~~~~~~~~~~~~~~~~~~~

**实验简介：**

小车上有两个舵机，这里以接在引脚D9的舵机为例，舵机是一种可以非常精确地旋转的电机。目前已广泛应用于玩具车、遥控直升机、飞机、机器人等领域。在这个项目中，我们将使用Nano主板控制舵机转动。

**元件知识：**

|image87|

**\*舵机：\***
舵机是一种位置伺服的驱动器，主要是由外壳、电路板、无核心马达、齿轮与位置检测器所构成。其工作原理是由接收机或者单片机发出信号给舵机，其内部有一个基准电路，产生周期为20ms，宽度为1.5ms
的基准信号，将获得的直流偏置电压与电位器的电压比较，获得电压差输出。经由电路板上的IC
判断转动方向，再驱动无核心马达开始转动，透过减速齿轮将动力传至摆臂，同时由位置检测器送回信号，判断是否已经到达定位。适用于那些需要角度不断变化并可以保持的控制系统。当电机转速一定时，通过级联减速齿轮带动电位器旋转，使得电压差为0，电机停止转动。一般舵机旋转的角度范围是0度到180
度。

控制舵机的脉冲周期为20ms，脉冲宽度为0.5ms ~ 2.5ms，对应位置为-90°~
+90°。下面是以一个180°角的舵机为例：

|image88|

伺服电机有多种规格，但它们都有三根连接线，分别是棕色、红色、橙色(不同品牌可能有不同的颜色)。棕色为GND，红色为电源正极，橙色为信号线。

|image89|

**实验接线：**

====== =========
舵机   小车PCB板
====== =========
棕线   G
红线   5V
橙黄线 S1（D9）
====== =========

**实验代码**

.. code:: c++

   //*********************************************************************************
   /*
   Project 05 Servo Rotation
   the plastic arm of the servo will rotate at an angle of 0°, 45°, 90°, 135°, and 180°,repeatly.
   */
   #include <Servo.h>
   Servo myservo;// define the name of the servo
   void setup()
   {
   myservo.attach(9);// select the pin of the servo(9)
   }
   void loop()
   {
     myservo.write(0);// set the rotation angle of the motor
     delay(500);
     myservo.write(45);// set the rotation angle of the motor
     delay(500);
     myservo.write(90);// set the rotation angle of the motor
     delay(500);
     myservo.write(135);// set the rotation angle of the motor
     delay(500);
     myservo.write(180);// set the rotation angle of the motor
     delay(500);
   }
   //*********************************************************************************

**实验现象**

将实验代码上传至Arduino
Nano主板，利用USB线上电后，舵机塑料臂将以0°、45°、90°、135°、180°的角度转动。循环进行！！

Project 06: 电机驱动和调速
~~~~~~~~~~~~~~~~~~~~~~~~~~

**实验简介：**

驱动电机的方法有很多，我们这个小车用到的是最常用的DRV8833电机驱动芯片，该芯片为玩具、打印机及其它电机一体化应用提供了一款双通道桥式电动驱动器解决方案。

在本实验中，我们使用扩展板上的DRV8833电机驱动芯片驱动小车的两个直流电机，通过编写代码实现小车分别向前，向后，向左，向右行走的效果。

**元件知识：**

**DRV8833电机驱动芯片：**
具有电流控制功能的双H桥电机驱动器，可以驱动两个直流电机、一个双极步进电机、电磁阀或其他电感负载。每个H桥的输出驱动器块由N沟道功率MOSFET组成，配置为H桥以驱动电机绕组。每个H桥包括调节或限制绕组电流的电路。

带有故障输出引脚的内部停机功能是用于过大电流保护、短路保护、欠压锁定和超温。还提供了低功耗睡眠模式。我们来看一下DRV8833电机驱动芯片驱动两个直流电机的电路图和示意图：

|image90|

|image91|

**规格参数：**

逻辑部分输入电压：DC 5V

驱动部分输入电压：DC 5V

逻辑部分工作电流：<30mA

驱动部分工作电流：<2A

最大耗散功率：10W（T=80℃）

电机转速：5V 200 rpm / min

电机驱动形式：双路H桥驱动

控制信号输入电平：高电平2.3V<Vin<5V ，低电平-0.3V<Vin<1.5V

工作温度：-25~130℃

**驱动小车运行原理**\ ：

根据上面电机驱动板的电路图和示意图，我们知道左电机的方向引脚在D4，调速引脚在D6；右电机的方向引脚在D2，调速引脚在D5，按照以下表格的运动逻辑，就可以知道如何通过控制数字口，PWM口控制2个电机转动，从而实现智能小车的行走。其中PWM值范围为0-255，设置数字越大，电机转动越快。

==== ==== ========= ====== ==== ========= ======
功能 D4   D6（PWM） 左电机 D2   D5（PWM） 右电机
==== ==== ========= ====== ==== ========= ======
前进 LOW  200       正转   LOW  200       正转
后退 HIGH 50        反转   HIGH 50        反转
左转 HIGH 200       反转   LOW  200       正转
右转 LOW  200       正转   HIGH 200       反转
停止 LOW  0         停止   LOW  0         停止
==== ==== ========= ====== ==== ========= ======

**实验代码**

.. code:: c++

   //*************************************************************************************
   /*
    Project 06 Motor drive and speed regulation
    Motor moves forward, backward, left and right
   */ 
   const int left_ctrl = 4;//定义左电机方向控制引脚D4
   const int left_pwm = 6;//定义左电机速度控制引脚D6
   const int right_ctrl = 2;//定义右电机方向控制引脚D2
   const int right_pwm = 5;//定义右电机速度控制引脚D5

   void setup()
   {
     pinMode(left_ctrl,OUTPUT);//设置左电机方向控制引脚为输出
     pinMode(left_pwm,OUTPUT);//设置左电机pwm控制速度引脚为输出
     pinMode(right_ctrl,OUTPUT);//设置右电机方向控制引脚为输出
     pinMode(right_pwm,OUTPUT);//设置右电机pwm控制速度引脚为输出
   }

   void loop()
   { 
     //front
     digitalWrite(left_ctrl,LOW); //左电机方向控制引脚低电平
     analogWrite(left_pwm,200); //左电机PWM控制速度200
     digitalWrite(right_ctrl,LOW); //右电机方向控制引脚低电平
     analogWrite(right_pwm,200); //右电机PWM控制速度200
     delay(2000);//延时2秒
     
     //back
     digitalWrite(left_ctrl,HIGH); //左电机方向控制引脚高电平
     analogWrite(left_pwm,50); //左电机PWM控制速度50
     digitalWrite(right_ctrl,HIGH); //右电机方向控制引脚高电平
     analogWrite(right_pwm,50); //右电机PWM控制速度50
     delay(2000);//延时2秒
     
     //left
     digitalWrite(left_ctrl,HIGH); //左电机方向控制引脚高电平
     analogWrite(left_pwm,55); //左电机PWM控制速度55
     digitalWrite(right_ctrl,LOW); //右电机方向控制引脚低电平
     analogWrite(right_pwm,200); //右电机PWM控制速度200
     delay(2000);//延时2秒
     
     //right
     digitalWrite(left_ctrl,LOW); //左电机方向控制引脚低电平
     analogWrite(left_pwm,200); //左电机PWM控制速度200
     digitalWrite(right_ctrl,HIGH); //右电机方向控制引脚高电平
     analogWrite(right_pwm,55); //右电机PWM控制速度55
     delay(2000);//延时2秒
     
     //stop
     digitalWrite(left_ctrl,LOW);//左电机方向控制引脚低电平
     analogWrite(left_pwm,0);//左电机PWM控制速度0
     digitalWrite(right_ctrl,LOW);//右电机方向控制引脚低电平
     analogWrite(right_pwm,0);//右电机PWM控制速度0
     delay(2000);//延时2秒
   }
   //*************************************************************************************

**实验现象**

将实验代码上传到Arduino
Nano主板，小车安上电池，并且将电源开关拨到ON端，上电后，小车前进2秒，后退2秒，左转2秒，右转2秒，停止2秒，循环。

**调速说明**

|image92|\ HIGH相当于PWM值255，50是PWM值，是可以调整的。此代码中的差值是200，上下差值越大，电机转速越快，我们可以通过调整PWM值达到调节电机转速。如果将50调为0，上下差值就变成255，电机转速达到最大；如果将50调为255时，上下差值就变成0，电机转速为0，电机就不转动了。上下差值为正值时，电机反转。

|image93|\ LOW相当于PWM值0，200是PWM值，是可以调整的。此代码中的差值是200，上下差值越大，电机转速越快，我们可以通过调整PWM值达到调节电机转速。如果将200调为100，上下差值就变成100，电机转速减慢；如果将200调为255时，上下差值就变成255，电机转速达到最大；如果将200调为0时，上下差值变为0，电机就不转动了。上下差值为负值时，电机正转。

Project 07：超声波测距
~~~~~~~~~~~~~~~~~~~~~~

小车上有个超声波传感器，超声波传感器是一种非常实惠的距离传感器，它可以检测前方是否存在障碍物，并且检测出传感器与障碍物的详细距离。它的原理和蝙蝠飞行的原理一样，就是超声波传感器发送出一种频率很高的超声波信号，通常正常人耳朵的听力的声波范围是20Hz~20kHz，人类无法听到。这些超声波的信号若是碰到障碍物，就会立刻反射回来，在接收到返回的信息之后，通过判断发射信号和接收信号的时间差，计算出传感器和障碍物的距离。超声波传感器主要用于各种机器人项目中的物体躲避和测距，也常被用于水位传感，甚至作为一个停车传感器。在本章中，我们将学习超声波传感器测距原理及应用。

**实验简介**

在本实验中，我们使用超声波传感器来测量距离，并将数据打印在串口监视器上。

**元件知识**

**\*HC-SR04超声波传感器：\***
像蝙蝠一样使用声纳来确定与物体的距离，它提供了精准的非接触范围检测，高精度和稳定的读数。它的操作不受阳光或黑色材料的影响，就像精密的照相机(在声学上像布料这样比较软的材料很难被探测到)。它带有超声波发射器和接收器。

|image94|

在超声波传感器的前面是两个金属圆筒，这些是转换器。转换器将机械能转换成电信号。在超声波传感器中，有发射转换器和接收转换器。发射转换器将电信号转换为超声波脉冲，接收转换器将反射的超声波脉冲转换回电信号。如果你看超声波传感器的背面，你会看到的发射转换器后面有一个IC。这是控制发射转换器的IC。在接收转换器后面也有一个IC，这是一个四运算放大器，它将接收转换器产生的信号放大成足以传输到Arduino的信号。

**\*时序图：\***

下面图示是HC-SR04的时序图，为了开始测量，SR04的Trig必须接受至少10us的高(5V)脉冲，这将启动传感器将发射出8个周期的40kHz的超声波脉冲，并等待反射的超声波脉冲。当传感器从接收器检测到超声波时，它将设置回波引脚为高(5V)和延迟一个周期(宽度)，与距离成比例。为了获得距离，测量Echo引脚的宽度。

|image95|

时间=回波脉冲宽度，单位为us(微秒)

距离（厘米）=时间/ 58

距离(英寸)=时间/ 148

|image96|

HC-SR04超声波传感器有四个引脚：Vcc、Trig、Echo和GND。Vcc引脚提供产生超声波脉冲的电源，接Vcc/+5V。GND引脚接地/GND。Trig引脚是Arduino发送信号来启动超声波脉冲的地方。Echo引脚是超声波传感器向Arduino控制板发送关于超声波脉冲行程持续时间的信息的地方。

**实验接线：**

============ =========
超声波传感器 小车PCB板
============ =========
Vcc          5V
Trig         S2（D8）
Echo         S1（D7）
Gnd          G
============ =========

**实验代码**

超声波传感器的Trig引脚是由Arduino
Nano主板的IO口D8控制，Echo引脚是由Arduino Nano主板的IO口D7控制。

.. code:: c++

   //**********************************************************************************
   /*
   Project 07 Ultrasonic Ranging
   Ultrasonic detection of distance from objects
   */
   const int trig = 8;  //Define trig pin to D8
   const int echo = 7;  //Define echo pin to D7
   int duration = 0;   
   int distance = 0; //Define a variable to receive distance
   void setup() 
   {
     pinMode(trig , OUTPUT); // Define the trig pin as the output mode 
     pinMode(echo , INPUT); // Define the echo pin as the input mode
     Serial.begin(9600); // Set baud rate to 9600
   }
   void loop()
   {
     digitalWrite(trig , HIGH);//the sensor is triggered by a high pulse of 1000 microseconds or more
     delayMicroseconds(1000);
     digitalWrite(trig , LOW); // Give a short low level in advance to ensure a clean high pulse
     duration = pulseIn(echo , HIGH);
     distance = (duration/2) / 28.5 ; //Convert to distance
     Serial.print(distance); // Print the distance in centimeters
     Serial.println("cm");
   }
   //**********************************************************************************

**实验现象**

将实验代码上传到Arduino
Nano主板，利用USB线上电后，再打开串口监视器，设置波特率为9600，当把一个物体放在超声波传感器前面移动时(远近)，它会检测到物体的距离，该值将显示在串口监视器上。

|image97|

Project 08: 跟随我
~~~~~~~~~~~~~~~~~~

**实验简介：**

|img-20230518083845|

在上面实验中，我们已经了解了8*8点阵、电机驱动和调速、超声波传感器、舵机等硬件知识，那么在本实验中，我们将结合它们打造一款跟随小车!
在电路设计过程中，我们可以利用超声波传感器来检测小车与前方物体的距离。通过测量距离控制电机的旋转，从而控制小车的运动状态，使小车跟随物体运动。

**工作原理：**

===== ========================= ================
检测  检测前方物体的距离        距离（单位：cm）
===== ========================= ================
条件1 距离＜8                   
状态  小车后退（设置PWM 为100） 
条件2 8≤距离<13                 
状态  小车停止                  
条件3 13≤距离<35                
状态  小车前进（设置PWM 为100） 
条件3 距离≥35                   
状态  小车停止                  
===== ========================= ================

**流程图：**

|image98|

**实验代码**

.. code:: c++

   //*************************************************************************************
   /*
   Project 08: follow me
   Car follows the object
   */ 
   const int left_ctrl = 4;//定义左电机方向控制引脚D4
   const int left_pwm = 6;//定义左电机速度控制引脚D6
   const int right_ctrl = 2;//定义右电机方向控制引脚D2
   const int right_pwm = 5;//定义右电机速度控制引脚D5
   #include "SR04.h" //定义超声波模块函数库
   #define TRIG_PIN 8// 定义超声波的信号输入在D8
   #define ECHO_PIN 7//定义超声波的信号输出在D7
   SR04 sr04 = SR04(ECHO_PIN,TRIG_PIN);
   long distance;
   const int servopin = 9;//定义舵机的脚位在D9
   int myangle;
   int pulsewidth;

   void setup() {
     pinMode(left_ctrl,OUTPUT);//设置左电机方向控制引脚为输出
     pinMode(left_pwm,OUTPUT);//设置左电机pwm控制速度引脚为输出
     pinMode(right_ctrl,OUTPUT);//设置右电机方向控制引脚为输出
     pinMode(right_pwm,OUTPUT);//设置右电机pwm控制速度引脚为输出
     pinMode(TRIG_PIN,OUTPUT);//设置TRIG_PIN为输出
     pinMode(ECHO_PIN,INPUT);//设置ECHO_PIN为输入
     servopulse(servopin,90);//设置舵机初始角度为90
     delay(300);
   }

   void loop() {
     distance = sr04.Distance();//超声波测量的距离
     if(distance<8)//如果距离小于8
     {
       back();//后退
     }
     else if((distance>=8)&&(distance<13))//如果距离大于等于8，小于13
     {
       Stop();//停止
     }
     else if((distance>=13)&&(distance<35))//如果距离大于等于13，小于35
     {
       front();//跟随
     }
     else//如果以上都不是
     {
       Stop();//停止
     }
   }

   void servopulse(int servopin,int myangle)//舵机运行角度
   {
     for(int i=0; i<20; i++)
     {
       pulsewidth = (myangle*11)+500;
       digitalWrite(servopin,HIGH);
       delayMicroseconds(pulsewidth);
       digitalWrite(servopin,LOW);
       delay(20-pulsewidth/1000);
     }  
   }

   void front()//定义前进的状态
   {
     digitalWrite(left_ctrl,LOW); //左电机方向控制引脚低电平
     analogWrite(left_pwm,200); //左电机PWM控制速度200
     digitalWrite(right_ctrl,LOW); //右电机方向控制引脚低电平
     analogWrite(right_pwm,200); //右电机PWM控制速度200
   }
   void back()//定义后退的状态
   {
     digitalWrite(left_ctrl,HIGH); //左电机方向控制引脚高电平
     analogWrite(left_pwm,50); //左电机PWM控制速度50
     digitalWrite(right_ctrl,HIGH); //右电机方向控制引脚高电平
     analogWrite(right_pwm,50); //右电机PWM控制速度50
   }
   void Stop()//定义停止的状态
   {
     digitalWrite(left_ctrl,LOW);//左电机方向控制引脚低电平
     analogWrite(left_pwm,0);//左电机PWM控制速度0
     digitalWrite(right_ctrl,LOW);//右电机方向控制引脚低电平
     analogWrite(right_pwm,0);//右电机PWM控制速度0
   }
   //*************************************************************************************

**实验现象**

将实验代码上传到Arduino
Nano主板，小车安上电池，并且将电源开关拨到ON端，上电后，小车可以随着前方障碍物的移动而移动（只能在一条线直上，不能转弯）。

Project 09: 躲避障碍物
~~~~~~~~~~~~~~~~~~~~~~

**实验简介：**

|img-20230518083634|

在上一实验中，我们制作了一个超声波跟随小车。实际上，利用同样硬件，我只需要更改一个测试代码就可以将跟随小车变为避障小车。那超声波避障小车，是怎么实现的呢？当然也是通过超声波传感器的测距来实现的。通过超声波传感器检测机器人前方障碍物，然后根据这一个数据获得机器人运动方向。

**工作原理：**

====================== ======================================
初始设定               8*8点阵清屏
====================== ======================================
设置舵机90°            
循环进行               检测前方障碍物的距离：距离（单位: cm）
条件 1                 状态
0<距离＜10             小车停止
8*8点阵显示“停止”图案  
设置舵机 180°          离障碍物的距离：a1（单位：cm）
设置舵机0°             离障碍物的距离：a2（单位：cm）
条件2                  状态
a1＜a2                 小车向右转（设置PWM为 200）
8*8点阵显示“向右” 图案 
设置舵机 90°           
a1≥a2                  小车向左转（设置PWM为 200）
8*8点阵显示“向左” 图案 
设置舵机 90°           
距离≥10                8*8点阵显示“向前” 图案
前进（设置PWM为200）   
====================== ======================================

**流程图：**

|image99|

**实验代码**

.. code:: c++

   //*************************************************************************************
   /*
   Project 09: avoid obstacles
   */  
   #include <ks_Matrix.h>
   Matrix myMatrix(A4,A5);//定义点阵的引脚在A4,A5
   //数组，用于储存图案的数据，可以自己算也可以从取摸工具中得到
   uint8_t matrix_front[8]={0x18,0x24,0x42,0x99,0x24,0x42,0x81,0x00};
   uint8_t matrix_back[8]={0x00,0x81,0x42,0x24,0x99,0x42,0x24,0x18};
   uint8_t matrix_left[8]={0x12,0x24,0x48,0x90,0x90,0x48,0x24,0x12};
   uint8_t matrix_right[8]={0x48,0x24,0x12,0x09,0x09,0x12,0x24,0x48};
   uint8_t matrix_stop[8]={0x18,0x18,0x18,0x18,0x18,0x00,0x18,0x18};
   uint8_t  LEDArray[8];
   const int left_ctrl = 4;//定义左电机方向控制引脚D4
   const int left_pwm = 6;//定义左电机速度控制引脚D6
   const int right_ctrl = 2;//定义右电机方向控制引脚D2
   const int right_pwm = 5;//定义右电机速度控制引脚D5
   #include "SR04.h"//定义超声波模块函数库
   #define TRIG_PIN 8// 定义超声波的信号输入在D8
   #define ECHO_PIN 7//定义超声波的信号输出在D7
   SR04 sr04 = SR04(ECHO_PIN,TRIG_PIN);
   long distance,a1,a2;//定义三个距离变量
   const int servopin = 9;//定义舵机的脚位在D9
   int myangle;
   int pulsewidth;
   int val;

   void setup() {
     pinMode(left_ctrl,OUTPUT);//设置左电机方向控制引脚为输出
     pinMode(left_pwm,OUTPUT);//设置左电机pwm控制速度引脚为输出
     pinMode(right_ctrl,OUTPUT);//设置右电机方向控制引脚为输出
     pinMode(right_pwm,OUTPUT);//设置右电机pwm控制速度引脚为输出
     pinMode(TRIG_PIN,OUTPUT);//设置TRIG_PIN为输出
     pinMode(ECHO_PIN,INPUT);//设置ECHO_PIN为输入
     servopulse(servopin,90);//设置舵机初始角度为90
     delay(300);
     myMatrix.begin(112);
     myMatrix.clear();
   }
    
   void loop()
    {
     avoid();//运行避障主程序
   }

   void avoid()
   {
     distance=sr04.Distance(); //获取超声波距离的值
     if((distance < 10)&&(distance != 0))//如果距离小于10且大于0
     {
       car_Stop();//停止
       myMatrix.clear();
       myMatrix.writeDisplay();//点阵显示停止图案
       matrix_display(matrix_stop);  //点阵显示停止图案
       delay(100);
       servopulse(servopin,180);//舵机转到180度
       delay(200);
       a1=sr04.Distance();//测量距离
       delay(100);
       servopulse(servopin,0);//再转到0度
       delay(200);
       a2=sr04.Distance();//测量距离
       delay(100);
       if(a1 > a2)//比较距离，如果左边大于右边
       {
         car_left();//向左转
         myMatrix.clear();
         myMatrix.writeDisplay();
         matrix_display(matrix_left);    //点阵显示向左图案
         servopulse(servopin,90);//舵机回到90度
         delay(200);
         myMatrix.clear();
         myMatrix.writeDisplay();
         matrix_display(matrix_front);   //点阵显示前进图案
       }
       else//如果右边大于左边
       {
         car_right();//向右转
         myMatrix.clear();
         myMatrix.writeDisplay();
         matrix_display(matrix_right);   //显示右转图案
         servopulse(servopin,90);//舵机回到90度
         delay(200);
         myMatrix.clear();
         myMatrix.writeDisplay();
         matrix_display(matrix_front);  //点阵显示前进图案
       }
     }
     else//如果以上都不是
     {
       car_front();//前进
       myMatrix.clear();
       myMatrix.writeDisplay();
       matrix_display(matrix_front);  //点阵显示前进图案
     }
   }

   void servopulse(int servopin,int myangle)//舵机运行角度
   {
     for(int i=0; i<20; i++)
     {
       pulsewidth = (myangle*11)+500;
       digitalWrite(servopin,HIGH);
       delayMicroseconds(pulsewidth);
       digitalWrite(servopin,LOW);
       delay(20-pulsewidth/1000);
     } 
   }

   void car_front()//定义前进的状态
   {
     digitalWrite(left_ctrl,LOW); //左电机方向控制引脚低电平
     analogWrite(left_pwm,200); //左电机PWM控制速度200
     digitalWrite(right_ctrl,LOW); //右电机方向控制引脚低电平
     analogWrite(right_pwm,200); //右电机PWM控制速度200
   }
   void car_back()//定义后退的状态
   {
     digitalWrite(left_ctrl,HIGH); //左电机方向控制引脚高电平
     analogWrite(left_pwm,50); //左电机PWM控制速度50
     digitalWrite(right_ctrl,HIGH); //右电机方向控制引脚高电平
     analogWrite(right_pwm,50); //右电机PWM控制速度50
   }
   void car_left()//定义左转的状态
   {
     digitalWrite(left_ctrl,HIGH); //左电机方向控制引脚高电平
     analogWrite(left_pwm,55); //左电机PWM控制速度55
     digitalWrite(right_ctrl,LOW); //右电机方向控制引脚低电平
     analogWrite(right_pwm,200); //右电机PWM控制速度200
   }
   void car_right()//定义右转的状态
   {
     digitalWrite(left_ctrl,LOW); //左电机方向控制引脚低电平
     analogWrite(left_pwm,200); //左电机PWM控制速度200
     digitalWrite(right_ctrl,HIGH); //右电机方向控制引脚高电平
     analogWrite(right_pwm,55); //右电机PWM控制速度55
   }
   void car_Stop()//定义停止的状态
   {
     digitalWrite(left_ctrl,LOW);//左电机方向控制引脚低电平
     analogWrite(left_pwm,0);//左电机PWM控制速度0
     digitalWrite(right_ctrl,LOW);//右电机方向控制引脚低电平
     analogWrite(right_pwm,0);//右电机PWM控制速度0
   }

   //点阵显示图案的函数
   void matrix_display(unsigned char matrix_value[])
   {
     for(int i=0; i<8; i++)
       {
         LEDArray[i]=matrix_value[i];
         for(int j=7; j>=0; j--)
         {
           if((LEDArray[i]&0x01)>0)
           myMatrix.drawPixel(j, i,1);
           LEDArray[i] = LEDArray[i]>>1;
         }
       } 
       myMatrix.writeDisplay();
   }
   //*************************************************************************************
        

**实验现象**

将实验代码上传到Arduino
Nano主板，小车安上电池，并且将电源开关拨到ON端，上电后，小车可以可以自动避障。

Project 10: 红外循迹读值
~~~~~~~~~~~~~~~~~~~~~~~~

**实验简介：**

在本实验中，我们使用ST188L3红外对管来检测黑白线，并将数据打印在串口监视器上。

**元件知识：**

**\*红外循迹：\***
红外循迹有1对ST188L3红外对管，ST188L3红外对管具有一个高发射功率红外发射二极管和一个高灵敏度红外接收管。当红外发射二极管发射红外信号，红外信号经白色物体反射后，被接收管接收，一旦接收管接收到信号，输出端将输出低电平（0）；当红外发射二极管发射红外信号，红外线信号被黑色物体吸收后，将输出高电平（1），从而实现了通过红外线检测信号的功能。

|image-20230701141513611|

警告：反射式光学传感器(包括红外循迹)应避免在阳光等有红外干扰的环境中使用。阳光中含有许多不可见光，如红外线和紫外线。在强光环境下，反射式光学传感器不能正常工作。

下表给出了小车上的红外循迹检测不同颜色物体的所有情况下的数值。其中检测到黑色物体或无物体代表1，检测到白色物体代表0。

== == ============
左 右 值（二进制）
== == ============
0  0  00
0  1  01
1  0  10
1  1  11
== == ============

**实验代码**

小车PCB板上的左边红外循迹是由Arduino
Nano主板的IO口D11控制，右边红外循迹是由Arduino Nano主板的IO口D10控制。

.. code:: c++

   //*************************************************************************************
   /*
   Project 10: Tracking sensor read value
   */ 
   int tracking_left = 11; //定义左红外循迹引脚D11
   int tracking_right = 10; //定义右红外循迹引脚D10
   int L_val,R_val; //定义左,右红外循迹两个变量

   void setup() {
    Serial.begin(9600); //设置波特率为9600
    pinMode(tracking_left, INPUT); //设置左红外循迹引脚为输入
    pinMode(tracking_right, INPUT); //设置右红外循迹引脚为输入
   }

   void loop() {
    L_val = digitalRead(tracking_left); //读取左红外循迹的值
    R_val = digitalRead(tracking_right); //读取右红外循迹的值
    Serial.print("L_val: "); //串口打印字符串L_val
    Serial.print(L_val); //串口打印L_val值
    Serial.print("    "); //串口打印空格
    Serial.print("R_val: "); //串口打印字符串R_val
    Serial.println(R_val); //串口打印R_val值
    delay(300); //延时0.3秒
   }
   //*************************************************************************************

**实验现象**

将实验代码上传到Arduino
Nano主板，利用USB线上电后，再打开串口监视器，设置波特率为9600，在小车的红外循迹下面放个黑色的东西，移动它，你会看到不同的指示灯亮起来，同时在串口监视器上看到红外循迹读取的值。旋转电位器可调节灵敏度，将指示灯调节至亮与不亮的临界点时，灵敏度最高。

|image-20230701114014751|

Project 11: 循线行走
~~~~~~~~~~~~~~~~~~~~

**实验简介**

|img-20230518082944|

在前面的项目中，我们详细的介绍了在上面实验中，我们已经了解了电机驱动和调速、红外循迹等硬件知识。在本实验中，小车会根据红外循迹传送的数值做出不同的动作。

**工作原理**

== == ============ ========
左 右 值（二进制） 动作
== == ============ ========
0  0  00           停止
0  1  01           向右转
1  0  10           向左转
1  1  11           向前移动
== == ============ ========

**流程图**

|image100|

**实验代码**

.. code:: c++

   //*************************************************************************************
   /*
   Project 11: Follow line to walk
   */
   const int left_ctrl = 4;//定义左电机方向控制引脚D4
   const int left_pwm = 6;//定义左电机速度控制引脚D5
   const int right_ctrl = 2;//定义右电机方向控制引脚D2
   const int right_pwm = 5;//定义右电机速度控制引脚D5
   int tracking_left = 11;//定义左红外循迹引脚D11
   int tracking_right = 10;//定义右红外循迹引脚D10
   int L_val,R_val;//定义左,右红外循迹两个变量
   const int servopin = 9;//定义舵机的脚位在D9
   int myangle;
   int pulsewidth;

   void setup() {
     pinMode(left_ctrl,OUTPUT);//设置左电机方向控制引脚为输出
     pinMode(left_pwm,OUTPUT);//设置左电机pwm控制速度引脚为输出
     pinMode(right_ctrl,OUTPUT);//设置右电机方向控制引脚为输出
     pinMode(right_pwm,OUTPUT);//设置右电机pwm控制速度引脚为输出
     pinMode(tracking_left, INPUT); //设置左红外循迹引脚为输入
     pinMode(tracking_right, INPUT); //设置右红外循迹引脚为输入
     servopulse(servopin,90);//设置舵机初始角度为90
     delay(300);
   }

   void loop() 
   {
     tracking(); //运行主程序
   }

   void tracking()
   {
     L_val = digitalRead(tracking_left);//读取左红外循迹的值
     R_val = digitalRead(tracking_right);//读取右红外循迹的值
     if((L_val == 1)&&(R_val == 1))//如果左,右红外循迹都读到黑线
     {
       front();//小车前进
     }
     else if((L_val == 1)&&(R_val == 0))//否则如果左红外循迹读到黑线，右红外循迹没有
     {
       left();//小车左转
     }
     else if((L_val == 0)&&(R_val == 1))//如果右红外循迹读到黑线，左红外循迹没有
     {
       right();//小车右转
     }
     else//如果左,右红外循迹都没有读到黑线
     {
       Stop();//小车停止
      }
   }

   void servopulse(int servopin,int myangle)//舵机运行角度
   {
     for(int i=0; i<20; i++)
     {
       pulsewidth = (myangle*11)+500;
       digitalWrite(servopin,HIGH);
       delayMicroseconds(pulsewidth);
       digitalWrite(servopin,LOW);
       delay(20-pulsewidth/1000);
     }  
   }

   void front()//定义前进的状态
   {
     digitalWrite(left_ctrl,LOW); //左电机方向控制引脚低电平
     analogWrite(left_pwm,100); //左电机PWM控制速度200
     digitalWrite(right_ctrl,LOW); //右电机方向控制引脚低电平
     analogWrite(right_pwm,100); //右电机PWM控制速度200
   }
   void left()//定义左转的状态
   {
     digitalWrite(left_ctrl,HIGH); //左电机方向控制引脚高电平
     analogWrite(left_pwm,200); //左电机PWM控制速度200
     digitalWrite(right_ctrl,LOW); //右电机方向控制引脚低电平
     analogWrite(right_pwm,50); //右电机PWM控制速度200
   }
   void right()//定义右转的状态
   {
     digitalWrite(left_ctrl,LOW); //左电机方向控制引脚低电平
     analogWrite(left_pwm,50); //左电机PWM控制速度200
     digitalWrite(right_ctrl,HIGH); //右电机方向控制引脚高电平
     analogWrite(right_pwm,200); //右电机PWM控制速度200
   }
   void Stop()//定义停止的状态
   {
     digitalWrite(left_ctrl,LOW);//左电机方向控制引脚低电平
     analogWrite(left_pwm,0);//左电机PWM控制速度0
     digitalWrite(right_ctrl,LOW);//右电机方向控制引脚低电平
     analogWrite(right_pwm,0);//右电机PWM控制速度0
   }
   //*************************************************************************************

**实验现象**

将实验代码上传到Arduino
Nano主板，小车安上电池，并且将电源开关拨到ON端，上电后，然后把小车放在循迹轨道（我们提供的）上，小车就开始根据红外循迹传送的数值做出不同的动作。

Project 12: 读取光敏传感器的值
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

我们都知道人类可以通过自己的眼睛在黑暗中寻找光源，那么机器人是怎样完成这项任务呢？让机器人完成这项任务首先需要给机器人安装上能看见光亮的眼睛，即光敏传感器，这样就能让机器人通过光源的强弱来寻找光源。

我们的小车上左右各装有1个光敏传感器，当外界环境光线的强、弱发生变化的时候，光敏传感器的电阻也跟随发生相应的改变，并把这种变化传输给小车上的Nano主板，Nano主板就像人的大脑一样可以判断和思考，指挥着小车寻找光线。两个光敏传感器不停的检测是否有光线，检测到光线后就判断左、右两边哪个方向的光线较强，最后就指挥小车向着光线强的方向前进。

**实验简介：**

在本实验中，我们将了解光敏传感器的工作原理。

**元件知识：**

**光敏传感器：**
它主要采用光敏电阻元件，该电阻元件电阻大小随着光照强度的变化而变化。传感器信号端连接单片机模拟口，当光线越强时，模拟口电压越大，即单片机的模拟值也大；反之，光照强度越弱时，模拟口电压越小，即单片机的模拟值也小。这样，就可以利用光敏传感器读取对应的模拟值来反映环境光线强度。

**实验接线：**

通过前面的安装接线知道，两个光敏传感器的信号脚位已经接到了Nano主板的A6和A7，下面我们就利用接到A6的光敏传感器来完成下面的实验，首先我们来读取模拟值。

============== =============
左边光敏传感器 小车PCB板
============== =============
G              G
V              V
S              S（A6或者A7）
============== =============

|img-20230508101729|\ |img-20230508101203|

--------------

**实验代码**

左边光敏传感器是由Arduino Nano主板的IO口A6控制。

.. code:: c++

   //*************************************************************************************
   /*
   Project 12:Read Photosensor Value
   */
   int sensorPin = A6;    // select the input pin for the photocell
   int sensorValue = 0;  // variable to store the value coming from the sensor
   void setup() {
     Serial.begin(9600);
   }
   void loop() {
     sensorValue = analogRead(sensorPin);  // read the value from the sensor:
     Serial.println(sensorValue);  //Serial port prints the value of photoresistor
     delay(500);
   }
   //*************************************************************************************

**实验现象**

将实验代码上传到Arduino
Nano主板，利用USB线上电后，再打开串口监视器，设置波特率为9600，当光线增强时，串口监视器显示的模拟值增大；反之，串口监视器显示的模拟值减小。

|image101|

Project 13: 寻光车
~~~~~~~~~~~~~~~~~~

**实验简介**

|img-20230518083512|

前面实验已经了解过光敏传感器的工作原理、电机驱动与调速，在本实验中，我们利用光敏传感器检测光线强弱来实现小车寻光效果，哪边光敏传感器接收到的光线较强，小车就往那边走。

**工作原理**

==================== ==================== ========
左光敏传感器的模拟值 右光敏传感器的模拟值 功能
==================== ==================== ========
大于500              大于500              向前移动
大于500              小于等于500          向左移动
小于等于500          大于500              向右移动
小于500              小于500              停止
==================== ==================== ========

**实验接线**

============== ========= ============== =========
左边光敏传感器 小车PCB板  右边光敏传感器 小车PCB板
============== ========= ============== =========
G              G          G              G
V              V          V              V
S              S（A6）    S              S（A7）
============== ========= ============== =========

**流程图**

|image102|

**实验代码**

左边光敏传感器是由Arduino
Nano主板的IO口A6控制，右边光敏传感器是由Arduino Nano主板的IO口A7控制。

.. code:: c++

   //*************************************************************************************
   /*
   Project 13:Light Following Car
   */ 
   const int light_L_Pin = A6;   //定义左光敏传感器引脚A6
   const int light_R_Pin = A7;   //定义右光敏传感器引脚A7
   const int left_ctrl = 4;//定义左电机方向控制引脚D4
   const int left_pwm = 6;//定义左电机速度控制引脚D6
   const int right_ctrl = 2;//定义右电机方向控制引脚D2
   const int right_pwm = 5;//定义右电机速度控制引脚D5
   int left_light; 
   int right_light;
   const int servopin = 9;//定义舵机的脚位在D9
   int myangle;
   int pulsewidth;

   void setup(){
     Serial.begin(9600);
     pinMode(light_L_Pin, INPUT); //设置左光敏传感器引脚为输入
     pinMode(light_R_Pin, INPUT); //设置右光敏传感器引脚为输入
     pinMode(left_ctrl,OUTPUT);//设置左电机方向控制引脚为输出
     pinMode(left_pwm,OUTPUT);//设置左电机pwm控制速度引脚为输出
     pinMode(right_ctrl,OUTPUT);//设置右电机方向控制引脚为输出
     pinMode(right_pwm,OUTPUT);//设置右电机pwm控制速度引脚为输出
     servopulse(servopin,90);//设置舵机初始角度为90
     delay(300);
   }

   void loop(){
     left_light = analogRead(light_L_Pin);//读取左光敏传感器的值
     right_light = analogRead(light_R_Pin);//读取右光敏传感器的值
     Serial.print("left_light_value = ");
     Serial.println(left_light);
     Serial.print("right_light_value = ");
     Serial.println(right_light);
     if (left_light > 500 && right_light > 500) //左,右光敏传感器测到的范围值
     {  
       Car_front(); //小车前进
     } 
     else if (left_light >500 && right_light <= 500)  //左,右光敏传感器测到的范围值
     {
       Car_left(); //小车左转
     } 
     else if (left_light <= 500 && right_light > 500) //左,右光敏传感器测到的范围值
     {
       Car_right(); //小车右转
     } 
     else  //除以上情况之外
     {
       Car_Stop(); //小车停止
     }
   }

   void servopulse(int servopin,int myangle)//舵机运行角度
   {
     for(int i=0; i<20; i++)
     {
       pulsewidth = (myangle*11)+500;
       digitalWrite(servopin,HIGH);
       delayMicroseconds(pulsewidth);
       digitalWrite(servopin,LOW);
       delay(20-pulsewidth/1000);
     }  
   }

   void Car_front()
   {
     digitalWrite(left_ctrl,LOW); //左电机方向控制引脚低电平
     analogWrite(left_pwm,200); //左电机PWM控制速度200
     digitalWrite(right_ctrl,LOW); //右电机方向控制引脚低电平
     analogWrite(right_pwm,200); //右电机PWM控制速度200
   }
   void Car_left()
   {
     digitalWrite(left_ctrl,HIGH); //左电机方向控制引脚高电平
     analogWrite(left_pwm,200); //左电机PWM控制速度200
     digitalWrite(right_ctrl,LOW); //右电机方向控制引脚低电平
     analogWrite(right_pwm,200); //右电机PWM控制速度200;
   }
   void Car_right()
   {
     digitalWrite(left_ctrl,LOW); //左电机方向控制引脚低电平
     analogWrite(left_pwm,200); //左电机PWM控制速度200
     digitalWrite(right_ctrl,HIGH); //右电机方向控制引脚高电平
     analogWrite(right_pwm,200); //右电机PWM控制速度200
   }
   void Car_Stop()
   {
     digitalWrite(left_ctrl,LOW);//左电机方向控制引脚低电平
     analogWrite(left_pwm,0);//左电机PWM控制速度0
     digitalWrite(right_ctrl,LOW);//右电机方向控制引脚低电平
     analogWrite(right_pwm,0);//右电机PWM控制速度0
   }
   //*************************************************************************************

**实验现象**

将实验代码上传至Arduino
Nano主板，小车安上电池，并且将电源开关拨到ON端，上电后，寻光车能够跟随着光移动。

Project 14: 红外遥控和接收
~~~~~~~~~~~~~~~~~~~~~~~~~~

红外遥控在日常生活中随处可见，它被用来控制各种家电，如电视、音响、录影机和卫星信号接收器。红外遥控是由红外发射和红外接收系统组成的，也就是一个红外遥控器、红外接收器和一个能解码的单片机组成的，小车上有个红外接收器。在本章中，将介绍红外遥控器和红外接收器，并制作一辆红外遥控小车。
\*\* 实验简介*\*

在本实验中，使用红外接收器和红外遥控器相结合，读取红外遥控器上的按键值并将按键值打印在串口监视器上。

**元件知识**

**\*红外(IR)遥控器：\***
是一种具有一定数量按钮的设备。按下不同的按钮会使位于遥控器前端的红外发射管以不同的编码发送红外信号。红外遥控技术应用广泛，如电视、空调等。因此，在当今科技发达社会，红外遥控技术使你切换电视节目和调节空调温度都很方便。

我们使用的遥控器如下所示：

该红外遥控器采用NEC编码，信号周期为110ms。

|image103|

**\*红外(IR)接收器：\***
它是一种元件，可以接收红外光，所以可以用它来检测红外遥控器发出的红外光信号。红外接收器解调接收到的红外光信号，并将其转换回二进制，然后将信息传递给微控制器。

**红外信号调制过程图：**

|image104|

**\*NEC红外通信协议：\***

**\*NEC 协议\***

据我所知，我在这里描述的协议是由NEC（现在的瑞萨）开发的。我在互联网上看到过非常类似的协议描述，那里的协议被称为日本格式。

我承认，我不知道到底是谁开发的。我所知道的是，它被用于我的晚期录像机，由三洋公司生产，以Fisher的名义销售。NEC生产了遥控IC。

这段描述取自我的录像机的维修手册。在那些日子里，服务手册上充满了有用的信息！

\*\ **特点\***

- 8位地址和8位命令长度。

- 可使用扩展模式，使地址大小加倍。

- 地址和命令传输两次，以保证可靠性。

- 脉冲距离调制。

- 载波频率为38kHz。

- 位时间为1.125ms或2.25ms。

**\*调制**\ \*

|image105|

NEC协议使用脉冲距离编码的比特。每个脉冲是一个560µs长的38kHz载波突发（约21个周期）。一个逻辑
"1 "需要2.25ms的传输时间，而一个逻辑 "0
"只有一半，为1.125ms。推荐的载波占空比是1/4或1/3

**\*协议\***

|image106|

上图显示了NEC协议的一个典型脉冲序列。在这个协议中，LSB首先被传送。在这种情况下，地址59和命令16被传送。一个信息由一个9ms的AGC脉冲开始，它被用来设置早期红外接收器的增益。这个AGC突发之后是一个4.5ms的空格，然后是地址和命令。地址和命令被传送两次。第二次所有的位都是反转的，可以用来验证所收到的信息。总的传输时间是恒定的，因为每个比特都以其倒置的长度重复传输。如果你对这种可靠性不感兴趣，你可以忽略倒置的值，或者你可以将地址和命令扩展到每个16位

请记住，为了能够确定最后一个比特的值，在信息的最后还必须有一个额外的560µs的突发。

|image107|

一个命令只传送一次，即使遥控器上的键一直按着。每隔110ms就会传输一个重复代码，只要按键不动。这个重复代码只是一个9ms的AGC脉冲，然后是一个2.25ms的空间和一个560µs的脉冲。

|image108|

**\*扩展的NEC协议\***

NEC协议被广泛使用，很快所有可能的地址都用完了。通过牺牲地址冗余，地址范围从256个可能的值扩展到大约65000个不同的值。这样，地址范围从8位扩展到16位，而不改变协议的任何其他属性。

通过这种方式扩展地址范围，总的信息时间不再是恒定的。现在它取决于消息中1和0的总数。如果你想保持总的消息时间不变，你就必须确保地址栏中1的数量是8（这自动意味着0的数量也是8）。这将使不同地址的最大数量减少到只有13000左右。

命令的冗余仍然被保留下来。因此，每个地址仍然可以处理256个不同的命令。

|image109|

**请记住，**
扩展协议的256个地址值是无效的，因为它们实际上是正常的NEC协议地址。只要低字节与高字节完全相反，就不是一个有效的扩展地址。

**实验代码**

.. code:: c++

   //**********************************************************************************
   /*
   Project 14:Infrared remote and receiver
   */
   #include <IRremote.h>
   int RECV_PIN = 12;
   IRrecv irrecv(RECV_PIN);
   decode_results results;
   void setup()
   {
     Serial.begin(9600);
     irrecv.enableIRIn(); // start receiving signals
   }
   void loop() {
     if (irrecv.decode(&results)) {
       Serial.println(results.value, HEX);
       irrecv.resume(); // receive the next value
     }
     delay(100);
   }
   //**********************************************************************************

**实验现象**

将实验代码上传到Arduino
Nano主板，利用USB线上电后，再打开串口监视器，设置波特率为9600，

|image110|

按下红外遥控器上的一个按钮，你会在串口显示器上看到一个代码。多次按下相同的按钮以确保你拥有该按钮的正确代码。如果看到FFFFFFFF，请忽略它。

|image111|

写下红外遥控器与每个按钮相关联的代码，因为你稍后将需要这些信息。

|image112|

Project 15: 红外遥控车
~~~~~~~~~~~~~~~~~~~~~~

**实验简介：**

|img-20230518082547|

在上面实验中，我们已经了解了8*8点阵、电机驱动和调速、红外接收器和红外遥控器等硬件知识，在本实验中，我们将使用红外遥控器和红外接收器来控制小车做一些动作。

**工作原理：**

==================== ======== ======
按键                 按键代码 功能
==================== ======== ======
|image113|           FF629D   前进
点阵屏显示“前进”图案          
|image114|           FFA857   后退
点阵屏显示“后退”图案          
|image115|           FF22DD   向左转
点阵屏显示“左转”图案          
|image116|           FFC23D   向右转
点阵屏显示“右转”图案          
|image117|           FF02FD   停止
点阵屏显示“停止”图案          
==================== ======== ======

**流程图：**

|image118|

**实验代码**

.. code:: c++

   //*************************************************************************************
   /*
   Project 15:Infrared remote control car
   */ 
   #include <ks_Matrix.h>
   Matrix myMatrix(A4,A5);//定义点阵的引脚在A4,A5
   //数组，用于储存图案的数据，可以自己算也可以从取摸工具中得到
   uint8_t matrix_front[8]={0x18,0x24,0x42,0x99,0x24,0x42,0x81,0x00};
   uint8_t matrix_back[8]={0x00,0x81,0x42,0x24,0x99,0x42,0x24,0x18};
   uint8_t matrix_left[8]={0x12,0x24,0x48,0x90,0x90,0x48,0x24,0x12};
   uint8_t matrix_right[8]={0x48,0x24,0x12,0x09,0x09,0x12,0x24,0x48};
   uint8_t matrix_stop[8]={0x18,0x18,0x18,0x18,0x18,0x00,0x18,0x18};
   uint8_t  LEDArray[8];
   const int left_ctrl = 4;//定义左电机方向控制引脚D4
   const int left_pwm = 6;//定义左电机速度控制引脚D6
   const int right_ctrl = 2;//定义右电机方向控制引脚D2
   const int right_pwm = 5;//定义右电机速度控制引脚D5
   #include <IRremote.h>//红外遥控函数库
   int RECV_PIN = 12;//定义红外接收的脚位在D12
   IRrecv irrecv(RECV_PIN);
   long irr_val;
   decode_results results;
   const int servopin = 9;//定义舵机的脚位在D9
   int myangle;
   int pulsewidth;

   void setup()
   {
     Serial.begin(9600);//打开串口，波特率9600
     pinMode(left_ctrl,OUTPUT);//设置左电机方向控制引脚为输出
     pinMode(left_pwm,OUTPUT);//设置左电机pwm控制速度引脚为输出
     pinMode(right_ctrl,OUTPUT);//设置右电机方向控制引脚为输出
     pinMode(right_pwm,OUTPUT);//设置右电机pwm控制速度引脚为输出
     pinMode(RECV_PIN,INPUT);//设置红外接收器引脚为输入
     // In case the interrupt driver crashes on setup, give a clue
     // to the user what's going on.
     Serial.println("Enabling IRin");
     irrecv.enableIRIn(); // 开始接收信号
     Serial.println("Enabled IRin");
     myMatrix.begin(112);
     myMatrix.clear();
     myMatrix.writeDisplay();
     servopulse(servopin,90);//设置舵机初始角度为90
     delay(300);
   }

   void loop()
    {
     if (irrecv.decode(&results)) 
    {
       irr_val = results.value;
       Serial.println(irr_val, HEX);//串口打印读取的红外遥控信号
       switch(irr_val)
       {
         case 0xFF629D : 
         car_front(); 
         myMatrix.clear();
         myMatrix.writeDisplay();
         matrix_display(matrix_front);  
         break;
         case 0xFFA857 : 
         car_back(); 
         myMatrix.clear();
         myMatrix.writeDisplay();
         matrix_display(matrix_back); 
         break;
         case 0xFF22DD : 
         car_left(); 
         myMatrix.clear();
         myMatrix.writeDisplay();
         matrix_display(matrix_left); 
         break; 
         case 0xFFC23D : 
         car_right();
         myMatrix.clear();
         myMatrix.writeDisplay();
         matrix_display(matrix_right); 
         break;
         case 0xFF02FD : 
         car_Stop();
         myMatrix.clear();
         myMatrix.writeDisplay();
         matrix_display(matrix_stop); 
         break;
       }
           irrecv.resume(); // 接收下一个值
     }
   }

   void servopulse(int servopin,int myangle)//舵机运行角度
   {
     for(int i=0; i<20; i++)
     {
       pulsewidth = (myangle*11)+500;
       digitalWrite(servopin,HIGH);
       delayMicroseconds(pulsewidth);
       digitalWrite(servopin,LOW);
       delay(20-pulsewidth/1000);
     }  
   }

   void car_front()//定义前进的状态
   {
     digitalWrite(left_ctrl,LOW); //左电机方向控制引脚低电平
     analogWrite(left_pwm,200); //左电机PWM控制速度200
     digitalWrite(right_ctrl,LOW); //右电机方向控制引脚低电平
     analogWrite(right_pwm,200); //右电机PWM控制速度200
   }
   void car_back()//定义后退的状态
   {
     digitalWrite(left_ctrl,HIGH); //左电机方向控制引脚高电平
     analogWrite(left_pwm,50); //左电机PWM控制速度50
     digitalWrite(right_ctrl,HIGH); //右电机方向控制引脚高电平
     analogWrite(right_pwm,50); //右电机PWM控制速度50
   }
   void car_left()//定义左转的状态
   {
     digitalWrite(left_ctrl,HIGH); //左电机方向控制引脚高电平
     analogWrite(left_pwm,200); //左电机PWM控制速度200
     digitalWrite(right_ctrl,LOW); //右电机方向控制引脚低电平
     analogWrite(right_pwm,200); //右电机PWM控制速度200
   }
   void car_right()//定义右转的状态
   {
     digitalWrite(left_ctrl,LOW); //左电机方向控制引脚低电平
     analogWrite(left_pwm,200); //左电机PWM控制速度200
     digitalWrite(right_ctrl,HIGH); //右电机方向控制引脚高电平
     analogWrite(right_pwm,200); //右电机PWM控制速度200
   }
   void car_Stop()//定义停止的状态
   {
     digitalWrite(left_ctrl,LOW);//左电机方向控制引脚低电平
     analogWrite(left_pwm,0);//左电机PWM控制速度0
     digitalWrite(right_ctrl,LOW);//右电机方向控制引脚低电平
     analogWrite(right_pwm,0);//右电机PWM控制速度0
   }

   //点阵显示图案的函数
   void matrix_display(unsigned char matrix_value[])
   {
     for(int i=0; i<8; i++)
       {
         LEDArray[i]=matrix_value[i];
         for(int j=7; j>=0; j--)
         {
           if((LEDArray[i]&0x01)>0)
           myMatrix.drawPixel(j, i,1);
           LEDArray[i] = LEDArray[i]>>1;
         }
       } 
       myMatrix.writeDisplay();
   }
   //*************************************************************************************

**实验现象**

上传实验代码至Arduino
Nano主板，小车安上电池，并且将电源开关拨到ON端，上电后，按下红外遥控器对应按键，小车跟着遥控器按下的按键做出相应的动作。

Project 16：WIFI 测试
~~~~~~~~~~~~~~~~~~~~~

在如今科技高速发展的时代，人们的生活质量越来越好，生活节奏越来越快，开始有人觉得复杂多样的智能化设备控制起来十分麻烦，通过手机统一控制智能化设备这种方法逐渐得到了人们的青睐。

这种方法是利用单片机通过wifi模块和Internet网络建立手机和智能化设备之间的连接以此来实现对智能化设备的远程控制。在本章实验中，我们结合Nano主板和ESP8266串口WIFI
ESP-01模块，通过Beetlebot APP向ESP8266串口WIFI
ESP-01模块发送指令，ESP8266串口WIFI
ESP-01模块接到指令后再将其发送给单片机，单片机再控制小车进行动作调整。

**实验简介：**

ESP8266串口WIFI ESP-01模块，它是一款超低功耗的UART-WiFi
透传模块，拥有业内极富竞争力的封装尺寸和超低能耗技术，专为移动设备和物联网应用设计，可将用户的物理设备连接到Wi-Fi
无线网络上，进行互联网或局域网通信，实现联网功能。

**实验元件：**

======================== =====================================
|image119|               |image120|
======================== =====================================
ESP8266串口WIFI ESP-01*1 USB转ESP-01S WIFI模块串口测试扩展板*1
======================== =====================================

**元件知识：**

|image121|

**\*USB转ESP-01S WIFI模块串口测试扩展板：\*** 适用于ESP-01S
WiFi模块，扩展板的拨动开关打到flash
boot端，直插于电脑USB口，用安信可串口调试助手测试AT指令。

扩展板的拨动开关打到Uart Download
端，直插于电脑USB口，ESP-01模块处于下载模式，通过安信可固件下载软件可下载固件到ESP-01模块中。

|image122|

**ESP8266串口 WIFIESP-01：** ESP8266串口WIFI
ESP-01是一款超低功耗的UART-WiFi 透传模块，ESP8266串口WIFI
ESP-01可广泛应用于智能电网、智能交通、智能家具、手持设备、工业控制等领域。

**产品特性**

\*\* 支持无线802.11 b/g/n 标准

\*\* 支持STA/AP/STA+AP 三种工作模式

\*\* 内置TCP/IP协议栈，支持多路TCP Client连接

\*\* 支持丰富的Socket AT指令

\*\* 支持UART/GPIO数据通信接口

\*\* 支持Smart Link 智能联网功能

\*\* 支持远程固件升级（OTA）

\*\* 内置32位MCU，可兼作应用处理器

\*\* 超低能耗，高集成度的 Wi-Fi 芯片，适合电池供电应用

\*\* 超宽工作温度范围：-40°C 至 +125°C

\*\* 3.3V 单电源供电

**模块基本参数**

- **模块**

  ========== =======
  型号       主芯片
  ========== =======
  ESP8266-01 ESP8266
  ========== =======

- **无线参数**

  +-------------+-------------+-------------+-------------+-------------+
  | *           | *           | *           | **接        | *           |
  | *无线标准** | *频率范围** | *发射功率** | 收灵敏度**  | *天线形式** |
  +=============+=============+=============+=============+=============+
  | IEEE        | 2.412G      | 802.11b:    | 802.11b:    | 外置：      |
  | 802.11b/g/n | Hz-2.484GHz | +16 +/-2dBm | -93 dBm     | 邮票孔接口  |
  |             |             | (@11Mbps)   | (@11Mbps    |             |
  |             |             |             | ,CCK)       |             |
  +-------------+-------------+-------------+-------------+-------------+
  |             |             | 802.11g:    | 802.11g:    | 外置：I-PEX |
  |             |             | +14 +/-2dBm | -85dBm      | 连接器、SMA |
  |             |             | (@54Mbps)   | (@54Mbps,   | 连接器      |
  |             |             |             | OFDM)       |             |
  +-------------+-------------+-------------+-------------+-------------+
  |             |             | 802.11n:    | 802.11n:    | 内          |
  |             |             | +13 +/-2dBm | -82dBm      | 置：板载PCB |
  |             |             | (@HT20,     | (@HT20,     | 天线        |
  |             |             | MCS7)       | MCS7)       |             |
  +-------------+-------------+-------------+-------------+-------------+

- **硬件参数**

  +------------------+--------------------------------------------------+
  | **硬件接口**     | UART，IIC，PWM，GPIO，ADC                        |
  +==================+==================================================+
  | **工作电压**     | 3.3V                                             |
  +------------------+--------------------------------------------------+
  | **GPIO驱动能力** | Max：15ma                                        |
  +------------------+--------------------------------------------------+
  | **工作电流**     | 持续发送下=>平均值：~70mA，峰值:                 |
  |                  | 200mA正常模式下=>平均: ~12mA，峰值:              |
  |                  | 200mA待机：<200uA，                              |
  +------------------+--------------------------------------------------+
  | **工作温度**     | -40℃~125℃                                        |
  +------------------+--------------------------------------------------+
  | **存储环境**     | 温度：<40℃，相对湿度：<90%R.H.                   |
  +------------------+--------------------------------------------------+
  | **尺寸**         | 板载PCB天线：14.3mm\ *24.8mm*\ 1mm；             |
  +------------------+--------------------------------------------------+

- **串口透传**.

  ============= ==============
  **传输速率**  **TCP Client**
  ============= ==============
  110-921600bps 5个
  ============= ==============

- **软件参数**

  +------------------+--------------------------------------------------+
  | **无线网络类型** | STA/AP/STA+AP                                    |
  +==================+==================================================+
  | **安全机制**     | WEP/WPA-PSK/WPA2-PSK                             |
  +------------------+--------------------------------------------------+
  | **加密类型**     | WEP64/WEP128/TKIP/AES                            |
  +------------------+--------------------------------------------------+
  | **固件升级**     | 本地串口，OTA远程升级                            |
  +------------------+--------------------------------------------------+
  | **网络协议**     | IPv4, TCP/UDP/FTP/HTTP                           |
  +------------------+--------------------------------------------------+
  | **用户配置**     | AT+指令集, Web 页面 Android/iOS 终端, Smart Link |
  |                  | 智能配置APP                                      |
  +------------------+--------------------------------------------------+

**硬件介绍：**

ESP8266硬件接口丰富，可支持UART，IIC，PWM，GPIO，ADC等，适用于各种物联网应用场合。

+----------+------------------+--------------------------------------+
| **引脚** | **功能**         | **说明**                             |
+==========+==================+======================================+
| 1        | URXD             | 1）UART_RXD，接收；2）General        |
|          |                  | Purpose Input/Output：GPIO3；        |
+----------+------------------+--------------------------------------+
| 2        | UTXD             | 1）UART_TXD，发送；2）General        |
|          |                  | Purpose Input/Ou                     |
|          |                  | tput：GPIO1；3）开机时禁止下拉；     |
+----------+------------------+--------------------------------------+
| 5        | RESET（GPIO 16） | 外部Reset信号                        |
|          |                  | ，低电平复位，高电平工作（默认高）； |
+----------+------------------+--------------------------------------+
| 6        | GND              | GND                                  |
+----------+------------------+--------------------------------------+
| 8        | VCC              | 3.3V，模块供电；                     |
+----------+------------------+--------------------------------------+
| 9        | ANT              | WiFi Antenna                         |
+----------+------------------+--------------------------------------+
| 11       | GPIO0            | 1）默认WiFi                          |
|          |                  | Status：WiFi工作状                   |
|          |                  | 态指示灯控制信号；2）工作模式选择：  |
|          |                  | 悬空：Flash Boot，工作模式；         |
|          |                  | 下拉：UART Download，下载模式；      |
+----------+------------------+--------------------------------------+
| 12       | ADC              | ADC，输入范围：0V-1V；               |
+----------+------------------+--------------------------------------+
| 13       | GPIO15           | 下拉：工作模式；                     |
+----------+------------------+--------------------------------------+
| 14       | CH_PD            | 1）                                  |
|          |                  | 高电平工作；2）低电平模块供电关掉；  |
+----------+------------------+--------------------------------------+
| 15       | GPIO2            | 1）开机上电时必须为高电              |
|          |                  | 平，禁止硬件下拉；2）内部默认已拉高  |
+----------+------------------+--------------------------------------+

**功耗**

====================================== ====== ==== ====== ====
模式                                   最小值 通常 最大值 单位
====================================== ====== ==== ====== ====
传送802.11b，CCK 1Mbps，Pout=+19.5dBm         215         mA
传送802.11b，CCK 11Mbps，Pout=+18.5dBm        197         mA
传送802.11g，OFDM54 Mbps，Pout=+16dBm         145         mA
传送802.11n，MCS7，Pout=+14dBm                135         mA
接收802.11b，包长1024字节，-80dBm             100         mA
接收802.11g，包长1024字节，-70dBm             100         mA
接收802.11n，包长1024字节，-65dBm             102         mA
系统待机模式                                  70          mA
关机                                          0.5         μA
====================================== ====== ==== ====== ====

下列功耗数据是基于3.3V的电源、25°的环境温度下测得。

1.所有测量均在天线接口处完成。

2.所有发射数据是基于 90% 的占空比，在持续发射的模式下测得的。

射频指标：

以下数据是在室内温度下，电压为3.3V时测得。

============================== ========== ======== ========== ========
**描述**                       **最小值** **通常** **最大值** **单位**
============================== ========== ======== ========== ========
输入频率                       2412                2484       MHz
输入电阻                                  50                  Ω
输入反射                                           -10        dB
72.2Mbps下，PA的输出功率       14         15       16         dBm
802.11b模式下，PA的输出功率    17.5       18.5     19.5       dBm
**灵敏度**                                                    
CCK 1Mbps                                 -98                 dBm
CCK 11Mbps                                -91                 dBm
6Mbps(1/2BPSK)                            -93                 dBm
54Mbps(3/4 64-QAM)                        -75                 dBm
HT20，MCS7（65Mbps，72.2Mbps）            -71                 dBm
**邻频抑制**                                                  
OFDM，6Mbps                               37                  dB
OFDM，54Mbps                              21                  dB
HT20，MCS0                                37                  dB
HT20，MCS7                                20                  dB
============================== ========== ======== ========== ========

**注：** 1. 72.2Mbps是在802.11n模式下，MCS=7，GI=200uS时测得；

2. 802.11b模式下最高可达+19.5dBm的输出功率。

**功能描述**

**\*A.主要功能\***

ESP8266可以实现的主要功能包括：串口透传，PWM 调控，GPIO控制。

※串口透传：数据传输，传输的可靠性好，最大的传输速率为：460800bps。

※PWM 调控：灯光调节，三色LED 调节，电机调速等。

※GPIO控制：控制开关，继电器等。

**\*B.工作模式\***

ESP8266模块支持STA/AP/STA+AP 三种工作模式。

❊STA
模式：ESP8266模块通过路由器连接互联网，手机或电脑通过互联网实现对设备的远程控制。

|image123|

❊AP
模式：ESP8266模块作为热点，实现手机或电脑直接与模块通信，实现局域网无线控制。

❊STA+AP
模式：两种模式的共存模式，即可以通过互联网控制可实现无缝切换，方便操作。

|image124|

**\*C.应用领域\***

✭✮串口CH340 转Wi-Fi；

✭✮工业透传DTU；

✭✮Wi-Fi 远程监控/控制；

✭✮玩具领域；

✭✮彩色LED 控制；

✭✮消防、安防智能一体化管理；

✭✮智能卡终端，无线POS 机，Wi-Fi 摄像头，手持设备等

将WIFI模块串口测试扩展板插入电脑的USB口：

A. 将ESP8266串口WIFI ESP-01模块正确方向插入USB转ESP-01S
WIFI模块串口测试扩展板上。

|image125|

B. 先将USB转ESP-01S
WIFI模块串口测试扩展板上的拨码开关拨到UartDownload端，再将USB转ESP-01S
WIFI模块串口测试扩展板插入电脑的USB口。

|image126|

**Arduino搭建Esp8266开发环境**

先将ESP8266串口WIFI ESP-01模块正确插入USB转ESP-01S
WIFI模块串口测试扩展板中，然后将USB转ESP-01S
WIFI模块串口测试扩展板插入电脑的USB口，点击arduino
IDE（也可以采用最新版本的）进入界面。

|image127|

在Arduino IDE里面进行下载安装：

A.点击 **文件** → **首选项**\ ，在 **其他开发板管理器网址:**
框中复制粘贴这个地址：\ ``http://arduino.esp8266.com/stable/package_esp8266com_index.json``\ ，然后点击“\ **\*确定\***\ ”保存这个地址。

|image128|

|image129|

|image130|

B. 在开发板搜索框中，搜索
“\ **ESP8266**\ ”，点击安装最新版本，右下角可以看到开发板安装进度，等待几分钟安装完成。\ **安装过程中请保持网络稳定，如安装失败，请重复以上步骤，重新安装开发板即可。**\ （可能会出现下载安装出错，有可能是服务器原因，需要重新点击“安装”就可以了，但由于网络原因，大多用户可能无法搜到
esp8266 by esp8266
Community，对于小白而言不推荐使用此方法添加，推荐下面方法2）

\ **注意：\ 本教程使用的是\ ESP8266 3.1.2版本**
制作的请保持一致，以免出现代码不兼容情况。

|image131|

**假如，由于网络问题实在是下载安装不了ESP8266开发板，我们也提供有ESP8266开发板的压缩包**\ ，\ **ESP8266开发板的压缩包下载地址：**
https://pan.baidu.com/s/1-w3hVlYeEFErWwfnI2uY4g?pwd=i6b5

**提取码:** i6b5

**压缩包下载后解压，把解压后的ESP8266开发板文件夹按照以下路径添加。ESP8266开发板一般需要存放于以下路径，才能说明ESP8266开发板安装好。**

- **Windows
  系统**\ ：路径为C:\\Users\\你的用户名\\AppData\\Local\\Arduino15\\packages 。其中，AppData 是一个隐藏文件夹，你需要在文件夹选项中开启
  “显示隐藏的文件、文件夹和驱动器” 才能看到。
- **macOS
  系统**\ ：位于~/Library/Arduino15/packages。Library 也是一个隐藏文件夹，你可以通过在
  “\ **访达**\ ” 中使用快捷键Command + Shift +
  G ，然后输入该路径来访问。
- **Linux 系统**\ ：存于~/.arduino15/packages 。

C. 安装成功后，重新启动 Arduino IDE，然后点击“\ **\*工具\***\ ” →
“\ **\*开发板:\***\ ”，你可以在里面查看到各种不同型号ESP8266开发板。选择对应的ESP8266开发板型号和COM口，选中后即可对ESP8266进行编程。

|image132|

|image133|

|image134|

通过工具对ESP8266进行安装：（推荐使用这种方法）

A.点击 **文件** → **首选项**\ ，在 **其他开发板管理器网址:**
框中复制粘贴这个地址：\ ``http://arduino.esp8266.com/stable/package_esp8266com_index.json``\ ，然后点击“\ **\*确定\***\ ”保存这个地址。

|image135|

|image136|

|image137|

B.使用 “ESP8266 one-click installation of Arduino board version
2.5.0.exe”，一键安装，此方法安装便捷，且安装较快，推荐此方法安装。

|2023-07-01_132611|

鼠标左键双击“ESP8266 one-click installation of Arduino board version
2.5.0.exe”，然后就安装完成了。

|image138|

在上述工具安装完成之后，重启 Arduino IDE 软件，点击 Arduino 菜单栏
**工具** →
**开发板**\ ，可查看到各种不同型号ESP8266开发板。选择对应的ESP8266开发板型号和COM口，选中后即可对ESP8266进行编程。

|image139|

|image140|

|image141|

**实验代码**

**注意：**
打开IDE后，一定要先设置好板型和COM口。手机和设备需要连接在同一个WiFi上，打开手机热点共享WIFI是最好的方法。

**特别注意：**
需要先将项目代码\ |image142|\ 中的用户Wifi名称和用户Wifi密码改成你们自己的Wifi名称和Wifi密码。

ESP8266串口WIFI ESP-01模块的UTXD引脚是由Arduino
Nano主板的IO口RX（0）控制，URXD引脚是由Arduino
Nano主板的IO口TX（1）控制。

.. code:: c++

   Project 16 WIFI test
   */
   #include <ESP8266WiFi.h>
   #include <ESP8266mDNS.h>
   #include <WiFiClient.h>

   #ifndef STASSID
   //#define STASSID "your-ssid"
   //#define STAPSK  "your-password"
   #define STASSID "ChinaNet-2.4G-0DF0"   //the name of user's wifi
   #define STAPSK  "ChinaNet@233"       //the password of user's wifi
   #endif

   const char* ssid = STASSID;
   const char* password = STAPSK;

   // TCP server at port 80 will response the HTTP requirement
   WiFiServer server(80);

   void setup(void) {
     Serial.begin(115200);

     //  connect WiFi 
     WiFi.mode(WIFI_STA);
     WiFi.begin(ssid, password);
     Serial.println("");

     // wait connection
     while (WiFi.status() != WL_CONNECTED) {
       delay(500);
       Serial.print(".");
     }
     Serial.println("");
     Serial.print("Connected to ");
     Serial.println(ssid);
     Serial.print("IP address: ");
     Serial.println(WiFi.localIP());

     // set the mDNS responder::
     // - in this example. the first parameter is domain name
     //   The fully qualified domain name is “esp8266.local”
     // - the second parameter is IP address
     //   send the IP address via WiFi
     if (!MDNS.begin("esp8266")) {
       Serial.println("Error setting up MDNS responder!");
       while (1) {
         delay(1000);
       }
     }
     Serial.println("mDNS responder started");

     // activate TCP (HTTP) server
     server.begin();
     Serial.println("TCP server started");

     // add the server to MDNS-SD
     MDNS.addService("http", "tcp", 80);
   }

   void loop(void) {

     MDNS.update();

     // check the client side is connected or not
     WiFiClient client = server.available();
     if (!client) {
       return;
     }
     Serial.println("");
     Serial.println("New client");

     // wait the effective data from the client side
     while (client.connected() && !client.available()) {
       delay(1);
     }

     // read the first row of HTTP requirement
     String req = client.readStringUntil('\r');

     // the first row of the HTTP requirement is shown below: "GET /path HTTP/1.1"
     // Retrieve the "/path" part by finding the spaces
     int addr_start = req.indexOf(' ');
     int addr_end = req.indexOf(' ', addr_start + 1);
     if (addr_start == -1 || addr_end == -1) {
       Serial.print("Invalid request: ");
       Serial.println(req);
       return;
     }
     req = req.substring(addr_start + 1, addr_end);
     Serial.print("Request: ");
     Serial.println(req);
     client.flush();

     String s;
     if (req == "/") {
       IPAddress ip = WiFi.localIP();
       String ipStr = String(ip[0]) + '.' + String(ip[1]) + '.' + String(ip[2]) + '.' + String(ip[3]);
       s = "HTTP/1.1 200 OK\r\nContent-Type: text/html\r\n\r\n<!DOCTYPE HTML>\r\n<html>Hello from ESP8266 at ";
       s += ipStr;
       s += "</html>\r\n\r\n";
       Serial.println("Sending 200");
     } else {
       s = "HTTP/1.1 404 Not Found\r\n\r\n";
       Serial.println("Sending 404");
     }
     client.print(s);

     Serial.println("Done with client");
   }
   //**********************************************************************************

**实验现象**

Wifi名称和Wifi密码修改后，确保USB转ESP-01S
WIFI模块串口测试扩展板上的拨码开关已经拨到Uart Download
端，并且也确定USB转ESP-01S
WIFI模块串口测试扩展板已经插入电脑的USB口。然后按照前面方法设置板型和COM口，IDE右下角显示对应板型和COM口，再点击\ |image143|\ 将测试代码上传到ESP8266串口WIFI
ESP-01模块上，上传成功。（\ **注意：如果上传失败，在板型和COM口没问题下，将USB转ESP-01S
WIFI模块串口测试扩展板从电脑的USB口拔下来再次插到电脑的USB口**)

|image144|

WIFI实验代码上传成功后，先将USB转ESP-01S
WIFI模块串口测试扩展板从电脑的USB口拔下来，再将USB转ESP-01S
WIFI模块串口测试扩展板上的拨码开关拨到Flash Boot
端，然后再次插到电脑的USB口上。打开串口监视器，设置波特率为115200，即可看到你的WIFI信息，如下图所示：

|image145|

Project 17: APP控制8x8点阵
~~~~~~~~~~~~~~~~~~~~~~~~~~

**实验简介：**

在前面的实验中，我们已经知道ESP8266串口WIFI
ESP-01模块通过WIFI测试代码得到相关的WIFI信息。那么在这个实验中，我们将使用ESP8266串口WIFI
ESP-01模块通过APP和WIFI来控制小车上8*8点阵。

将WIFI模块串口测试扩展板插入电脑的USB口

将ESP8266串口WIFI ESP-01模块正确方向插入USB转ESP-01S
WIFI模块串口测试扩展板上。

|image146|

先将USB转ESP-01S
WIFI模块串口测试扩展板上的拨码开关拨到UartDownload端，再将USB转ESP-01S
WIFI模块串口测试扩展板插入电脑的USB口。

|image147|

**ESP8266代码**

**特别注意：** 需要先将项目代码

|image148|\ 中的用户Wifi名称和用户Wifi密码改成你们自己的Wifi名称和Wifi密码。

ESP8266串口WIFI ESP-01模块的UTXD引脚是由Arduino
Nano主板的IO口RX（0）控制，URXD引脚是由Arduino
Nano主板的IO口TX（1）控制。

.. code:: c++

   //**********************************************************************************
   /*
   Project 17.1 ESP8266_Code
   */
   // generated by KidsBlock
   #include <Arduino.h>
   #include <ESP8266WiFi.h>
   #include <ESP8266mDNS.h>
   #include <WiFiClient.h>
   //#include <WiFi.h>

   #ifndef STASSID
   #define STASSID "ChinaNet-2.4G-0DF0"  //the name of user's Wifi
   #define STAPSK  "ChinaNet@233"       //the password of the user's wifi
   #endif
   const char* ssid = STASSID;
   const char* password = STAPSK;

   //IPAddress local_IP(192,168,4,22);
   //IPAddress gateway(192,168,4,22);
   //IPAddress subnet(255,255,255,0);
   //
   //const char *ssid = "ESP8266_AP_TEST";
   //const char *password = "12345678";

   WiFiServer server(80);
   String unoData = "";
   int ip_flag = 0;
   int ultra_state = 1;
   String ip_str;


   void setup() {
     Serial.begin(9600); 
   //   WiFi.mode(WIFI_AP); //设置工作在AP模式
   //
   //  WiFi.softAPConfig(local_IP, gateway, subnet); //设置AP地址
   //  while(!WiFi.softAP(ssid, password)){}; //启动AP
   //  Serial.println("AP启动成功");
   //
   //  Serial.print("IP address: ");
   //  Serial.println(WiFi.softAPIP()); // 打印IP地址
   //
   //  WiFi.softAPsetHostname("myHostName"); //设置主机名
   //  Serial.print("HostName: ");
   //  Serial.println(WiFi.softAPgetHostname()); //打印主机名
   //
   //  Serial.print("mac Address: ");
   //  Serial.println(WiFi.softAPmacAddress()); //打印mac地址

     WiFi.mode(WIFI_STA);
     WiFi.begin(ssid, password);
     while (WiFi.status() != WL_CONNECTED) {
       delay(500);
       Serial.print(".");
     }
     Serial.print("IP ADDRESS: ");
     Serial.println(WiFi.localIP());
     if (!MDNS.begin("esp8266")) {
       //Serial.println("Error setting up MDNS responder!");
       while (1) {
         delay(1000);
       }
     }
    // Serial.println("mDNS responder started");
     server.begin();
     //Serial.println("TCP server started");
     MDNS.addService("http", "tcp", 80);
     ip_flag = 1;
   }

   void loop() {
     //Serial.println(WiFi.softAPgetStationNum()); //打印客户端连接数
     if(ip_flag == 1)
     {
       for(int i=3; i>0; i--)
       {
         Serial.print("IP: ");
         Serial.print(WiFi.localIP());
         Serial.println('#');
         delay(500);
       }
       ip_flag = 0;
       
     }
       MDNS.update();
       WiFiClient client = server.available();
       if (!client) {
         return;
       }
       //Serial.println("");
       while (client.connected() && !client.available()) {
         delay(1);
       }
       String req = client.readStringUntil('\r');
       int addr_start = req.indexOf(' ');
       int addr_end = req.indexOf(' ', addr_start + 1);
       if (addr_start == -1 || addr_end == -1) {
         //Serial.print("Invalid request: ");
         //Serial.println(req);
         return;
       }
       req = req.substring(addr_start + 1, addr_end);
       int len_val = String(req).length();
       String M_req = String(req).substring(0,6);
       //Serial.println(M_req);
       if(M_req == "/btn/u")
       {
         String s_M_req = String(req).substring(5,len_val);
         Serial.print(s_M_req);
         Serial.print("#");
       }
       if(M_req == "/btn/v")
       {
         String s_M_req = String(req).substring(5,len_val);
         Serial.print(s_M_req);
         Serial.print("#");
       }
       client.flush();
       String s;
       if (req == "/") {
         IPAddress ip = WiFi.localIP();
         String ipStr = String(ip[0]) + '.' + String(ip[1]) + '.' + String(ip[2]) + '.' + String(ip[3]);
         s = "HTTP/1.1 200 OK\r\nContent-Type: text/html\r\n\r\n<!DOCTYPE HTML>\r\n<html>Hello from ESP8266 at ";
         s += ipStr;
         s += "</html>\r\n\r\n";
         //Serial.println("Sending 200");
         Serial.println(WiFi.localIP());
         Serial.write('*');
         client.println(WiFi.localIP());
         ip_flag = 0;
       }
       else if(req == "/btn/F")
       {
         Serial.write('F');
         client.println(F("F"));
       }
       else if(req == "/btn/B")
       {
         Serial.write('B');
         client.println(F("B"));
       }
       else if(req == "/btn/L")
       {
         Serial.write('L');
         client.println(F("L"));
       }
       else if(req == "/btn/R")
       {
         Serial.write('R');
         client.println(F("R"));
       }
       else if(req == "/btn/S")
       {
         Serial.write('S');
         client.println(F("S"));
       }
       else if(req == "/btn/a")
       {
         Serial.write('a');
         client.println(F("a"));
       }
       else if(req == "/btn/b")
       {
         Serial.write('b');
         client.println(F("b"));
       }
       else if(req == "/btn/c")
       {
         Serial.write('c');
         client.println(F("c"));
       }
       else if(req == "/btn/d")
       {
         Serial.write('d');
         client.println(F("d"));
       }
       else if(req == "/btn/e")
       {
         Serial.write('e');
         client.println(F("e"));
       }
       else if(req == "/btn/f")
       {
         Serial.write('f');
         client.println(F("f"));
       }
       else if(req == "/btn/g")
       {
         Serial.write('g');
         client.println(F("g"));
       }
       else if(req == "/btn/z")
       {
         Serial.write('z');
         client.println(F("z"));
       }
       else if(req == "/btn/i")
       {
         Serial.write('i');
         client.println(F("i"));
       }
       else if(req == "/btn/j")
       {
         Serial.write('j');
         client.println(F("j"));
       }
       else if(req == "/btn/k")
       {
         Serial.write('k');
         client.println(F("k"));
       }
       else if(req == "/btn/y")
       {
         Serial.write('y');
         client.println(F("y"));
       }
       else if(req == "/btn/l")
       {
         Serial.write('l');
         client.println(F("l"));
       }
       else if(req == "/btn/m")
       {
         Serial.write('m');
         client.println(F("m"));
       }
       else if(req == "/btn/n")
       {
         Serial.write('n');
         client.println("n");
       }
       else if(req == "/btn/o")
       {
         Serial.write('o');
         client.println(F("o"));
       }
       else if(req == "/btn/p")
       {
         Serial.write('p');
         client.println(F("p"));
       }
       else if(req == "/btn/q")
       {
         Serial.write('q');
         client.println("q");
       }
       else if(req == "/btn/x")
       {
         Serial.write('x');
         client.println(F("x"));
       }
       else if(req == "/btn/1")
       {
         Serial.write('1');
         client.println(F("1"));
       }
       else if(req == "/btn/2")
       {
         Serial.write('2');
         client.println("2");
       }
       else if(req == "/btn/3")
       {
         Serial.write('3');
         client.println(F("3"));
       }
       else if(req == "/btn/4")
       {
         Serial.write('4');
         client.println("4");
       }
       else if(req == "/btn/5")
       {
         Serial.write('5');
         client.println(F("5"));
       }
       else if(req == "/btn/0")
       {
         Serial.write('0');
         client.println("0");
       }
       else {
         //s = "HTTP/1.1 404 Not Found\r\n\r\n";
         //Serial.println("Sending 404");
       }

       client.print(F("IP : "));
       client.println(WiFi.localIP());
   }
   //**********************************************************************************

Wifi名称和Wifi密码修改后，确保USB转ESP-01S
WIFI模块串口测试扩展板上的拨码开关已经拨到Uart Download
端，并且也确定USB转ESP-01S
WIFI模块串口测试扩展板已经插入电脑的USB口。然后按照 **Project 16**
中的方法设置板型和COM口，IDE右下角显示对应板型和COM口，再点击\ |image149|\ 将ESP8266
代码上传到ESP8266串口WIFI
ESP-01模块上，上传成功。（注意：如果上传失败，在板型和COM口没问题情况下，将USB转ESP-01S
WIFI模块串口测试扩展板从电脑的USB口拔下来再次插到电脑的USB口)

ESP8266 代码上传成功后，先将USB转ESP-01S
WIFI模块串口测试扩展板从电脑的USB口拔下来，再将ESP8266串口WIFI
ESP-01模块从USB转ESP-01S WIFI模块串口测试扩展板上拔下来。

**Arduino Nano 实验代码**

**注意：**
打开IDE后，一定要先设置好板型和COM口。如果家里没有WIFI需要打开手机热点共享WIFI

.. code:: c++

   //**********************************************************************************
   /*
   Project 17.2 WiFi control dot matrix
   */
   #include <ks_Matrix.h>
   Matrix myMatrix(A4,A5);//Define the dot matrix pins in A4,A5
   //Array, used to store the data of the pattern, can be calculated yourself 
   //or retrieved from the touch tool
   uint8_t matrix_smile[8]={0x00,0x66,0x00,0x00,0x18,0x42,0x3c,0x00};
   uint8_t matrix_heart[8]={0x0e,0x11,0x21,0x42,0x21,0x11,0x0e,0x00};
   uint8_t matrix_ten[8]={0x08,0x08,0x08,0x08,0xff,0x08,0x08,0x08};
   uint8_t LEDArray[8];
   char wifiData;

   void setup() {
     Serial.begin(9600);
     myMatrix.begin(112);
     myMatrix.clear();
     myMatrix.writeDisplay();
   }

   void loop() {
     if(Serial.available() > 0)
     {
       wifiData = Serial.read();
       Serial.print(wifiData);
       if(wifiData == '#')
       {
         Serial.println("");
       }
       delay(100);
       
       if(wifiData == 'i')
       {
         myMatrix.writeDisplay();
         matrix_display(matrix_smile); 
       }
       else if(wifiData == 'k')
       {
         myMatrix.writeDisplay();
         matrix_display(matrix_heart);
       }
       else if(wifiData == 'j')
       {
         myMatrix.writeDisplay();
         matrix_display(matrix_ten);
       }
       else if(wifiData == 'y')
       {
         myMatrix.clear();
       }
     }
   }

   //Dot matrix display pattern function
   void matrix_display(unsigned char matrix_value[])
   {
     for(int i=0; i<8; i++)
       {
         LEDArray[i]=matrix_value[i];
         for(int j=7; j>=0; j--)
         {
           if((LEDArray[i]&0x01)>0)
           myMatrix.drawPixel(j, i,1);
           LEDArray[i] = LEDArray[i]>>1;
         }
       } 
       myMatrix.writeDisplay();
   }
   //**********************************************************************************

**实验现象**

点击Arduino 菜单栏的 "工具" → "开发板："，选择 “Arduino
Nano”，选择正确的COM端口，最后将Arduino Nano实验代码上传至Arduino
Nano主板。

|image150|

Arduino Nano实验代码上传成功后，再将ESP8266串口WIFI
ESP-01模块插入小车PCB板上的WiFi插口。（\ **注意：USB线不要拔下来，否则读取不了COM端口**\ ）

|image151|

点击\ |image152|\ 打开串口监视器窗口，将波特率设置为9600。这样，串口监视器就显示此时你们WIFI的IP地址。（\ **WIFI的IP地址有时候会改变，如果原来的IP地址不行，需要重新检测WIFI的IP地址**)

|image153|

**\*安卓系统设备（手机/平板）APP：\***

现将文件夹中的 **Beetlebot.apk** 文件转移到安卓系统手机或平板上

|image-20230701141106477|

或者使用手机浏览器中的扫描功能，扫描下面二维码进行下载

|image-20230701140459935|

点击 **Beetlebot.apk**
文件进入安装页面，点击“\ **\*ALLOW\***\ ”按钮，然后再点击“\ **\*INSTALL\***\ ”按钮，安装完成后点击“\ **\*OPEN\***\ ”按钮就可以进入APP界面。

|image154|

|image155|

|image156|

|image157|

|image158|

|image159|

|image160|

--------------

|image161|

先在WIFI按钮前面的文本框中输入检测到的WIFI
IP地址（\ **例如，上面串口监视器检测到的IP地址：192.168.1.134**\ ），再切换WIFI按钮来连接WiFi（\ **白色WIFI按钮变成绿色WIFI按钮**\ ），同时WIFI
IP地址前的文本框中会显示对应的WIFI
IP地址“192.168.1.134”。这样，就说明APP已经连接上了WIFI。

|image162|

**\*IOS系统设备（手机/iPad）APP\***

a.打开App Store。

|image163|

b.在搜索框输入 **Beetlebot**
，点击搜索，出现下载界面，点击“\ |image164|\ ”，就可以下载安装Beetlebot的APP。接下来的操作和安卓系统类似的，可以参考上面安卓系统的步骤进行操作。

**注意：点击APP上的按钮，ESP8266串口WIFI
ESP-01模块上的蓝色指示灯会闪烁，说明APP已经连接上WIFI。**

APP已经连接上了WIFI之后，开始进行如下操作：

点击APP上的按钮，串口监视器窗口打印一些对应的控制字符，如下图所示：

|image165|

APP上各个按钮（控件）对应的功能，如下图所示：

|image166|

**\*此代码实验APP操作及现象：\***

点击\ |image167|\ 按钮，小车前面的8\ *8点阵显示“笑脸”图案；点击\ img\ 按钮，小车前面的8*\ 8点阵显示“十”图案；点击\ |image168|\ 按钮，小车前面的8*8点阵显示“❤”图案。

Project 18: WiFi控制多功能小车
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

|img-20230518083704|

学习前面的课程，我们学完了控制Beetlebot小车的所有模块的功能。前面学的每样功能都要烧录一次对应的代码，我们想玩其它功能时就比较麻烦。现在我们编写个代码，将多个功能集合到一起，通过APP来切换功能，这样就会比较方便的玩多种功能了。

1.
ESP8266wifi的代码和上一课一样，修改好自己的WiFi密码。（如果上一课已经烧录过了，就不需要重复烧录）

|2023-07-01_134851|

2. 给Beetlebot的主控Arduino Nano主板烧录代码，代码在如下图文件夹中。

|2023-07-01_134850|

.. code:: c++

   //**********************************************************************************
   /*
   Project 18.2_Wifi_Multi_Function
   */
   #include<music.h>

   #include <Adafruit_NeoPixel.h>
   Adafruit_NeoPixel rgb_display_A3 = Adafruit_NeoPixel(4,A3,NEO_GRB + NEO_KHZ800);
   #include <Servo.h>
   Servo lgservo;
   Servo u_servo;
   #include <ks_Matrix.h>
   uint8_t  LEDArray[8];
   uint8_t matrix_smile[8]={0x42, 0xa5, 0xa5, 0x00, 0x00, 0x24, 0x18, 0x00};
   uint8_t matrix_front[8]={0x18, 0x3c, 0x5a, 0x99, 0x18, 0x18, 0x18, 0x18};
   uint8_t matrix_back[8]={0x18, 0x18, 0x18, 0x18, 0x99, 0x5a, 0x3c, 0x18};
   uint8_t matrix_left[8]={0x08, 0x04, 0x02, 0xff, 0xff, 0x02, 0x04, 0x08};
   uint8_t matrix_right[8]={0x10, 0x20, 0x40, 0xff, 0xff, 0x40, 0x20, 0x10};
   uint8_t matrix_stop[8]={0xff, 0x81, 0xbd, 0xa5, 0xa5, 0xbd, 0x81, 0xff};
   uint8_t matrix_tsundere[8]={0x00, 0xf7, 0x00, 0x08, 0x14, 0x20, 0x00, 0x00};
   uint8_t matrix_squinting[8]={0x00, 0x41, 0x22, 0x14, 0x22, 0x41, 0x1c, 0x00};
   uint8_t matrix_despise1[8]={0x00, 0x11, 0x77, 0x00, 0x1c, 0x00, 0x00, 0x00};
   uint8_t matrix_speechless[8]={0x00, 0x77, 0x00, 0x1c, 0x14, 0x1c, 0x00, 0x00};
   uint8_t matrix_heart[8]={0x00, 0x66, 0x99, 0x81, 0x81, 0x42, 0x24, 0x18};
   uint8_t matrix_clear[8]={0x00,0x00,0x00,0x00,0x00,0x00,0x00,0x00};

   #define ML 4
   #define ML_PWM 6
   #define MR 2
   #define MR_PWM 5
   #define buz 3
   #define Echo 7
   #define Trig 8
   #define servo1 9
   #define trackL 11
   #define trackR 10
   #define ir 12
   #define neo A3
   #define servo2 A0

   char val;
   char wifiData;
   int ip_flag = 1;
   int neo_flag=0;

   music Music(buz);

   Matrix myMatrix(A4,A5);
   int matrix_flag;
   boolean face1_flag = 0;
   boolean face2_flag = 0;
   int face_count=0;

   boolean neo_state = 0;
   String left_str,right_str;
   int left_val=150;
   int right_val=150;

   void setup() {
     Serial.begin(9600);
     pinMode(ML, OUTPUT);
     pinMode(ML_PWM, OUTPUT);
     pinMode(MR, OUTPUT);
     pinMode(MR_PWM, OUTPUT);
     pinMode(buz, OUTPUT);
     pinMode(Echo, INPUT);
     pinMode(Trig, OUTPUT);
     pinMode(trackL, INPUT);
     pinMode(trackR, INPUT);
     pinMode(ir, INPUT);

     rgb_display_A3.begin();
     lgservo.attach(A0);
     lgservo.write(180);
     u_servo.attach(9);
     u_servo.write(90);
     delay(300);

     myMatrix.begin(112);
     myMatrix.clear();
     matrix_display(matrix_smile);
     delay(100);
   }

   void loop() {
     if(Serial.available() > 0)
     {
       val = Serial.read();
       Serial.print(val);
       if(val == 'u')
       {
         Serial.println("left speed : ");
         left_str = Serial.readStringUntil('#');
         left_val = String(left_str).toInt();
         Serial.println(left_val);
       }
       if(val == 'v')
       {
         Serial.println("right speed : ");
         right_str = Serial.readStringUntil('#');
         right_val = String(right_str).toInt();
         Serial.println(right_val);
       }
     }
     switch(val)
     {
       case 'F': car_forward(); break;
       case 'B': car_back(); break;
       case 'L': car_left(); break;
       case 'R': car_right(); break;
       case 'S': car_stop(); break;
       case 'a': tone(buz, 294); delay(200); break;
       case 'b': noTone(buz); break;
       case 'c': Music.birthday(); break;
       case 'd': noTone(buz); break;
       case 'e': func_neo1(); break;
       case 'f': neo_stop(); break;
       case 'g': func_neo2(); break;
       case 'z': neo_state = 0; break;
       case 'i': face1(); break;
       case 'j': face_stop(); break;
       case 'k': face2(); break;
       case 'y': face1_flag=0; break;
       case 'l': tracking(); break;
       case 'm': avoid(); break;
       case 'n': followLightCar(); break;
       case 'o': followCar(); break;
     }
   }


   void followLightCar()
   {
     int lightL = analogRead(A6);
     int lightR = analogRead(A7);
     Serial.print(lightL);
     Serial.print("  ");
     Serial.println(lightR);
     if((lightL > 500) && (lightR > 500))
     {
       digitalWrite(ML,LOW);
       analogWrite(ML_PWM,150);
       digitalWrite(MR,LOW);
       analogWrite(MR_PWM,150);
     }
     else if((lightL > 500) && (lightR <= 500))
     {
       car_left();
     }
     else if((lightL <= 500) && (lightR > 500))
     {
       car_right();
     }
     else
     {
       car_stop();
     }
   }

   void followCar()
   {
     int distance = checkdistance();
     Serial.print("distance = ");
     Serial.println(distance);
     if((distance > 10) && (distance < 35))
     {
       digitalWrite(ML,LOW);
       analogWrite(ML_PWM,150);
       digitalWrite(MR,LOW);
       analogWrite(MR_PWM,150);
     }
     else if((distance > 6) && (distance <= 10))
     {
       car_stop();
     }
     else if(distance <= 6)
     {
       digitalWrite(ML,HIGH);
       analogWrite(ML_PWM,100);
       digitalWrite(MR,HIGH);
       analogWrite(MR_PWM,100);
     }
     else
     {
       car_stop();
     }
     
   }

   void avoid()
   {
     int distance = checkdistance();
     Serial.print("distance = ");
     Serial.println(distance);
     if(distance <= 8)
     {
       car_stop();
       delay(300);
       u_servo.write(180);
       delay(500);
       int distanceL = checkdistance();
       delay(50);
       u_servo.write(0);
       delay(600);
       int distanceR = checkdistance();
       delay(50);
       if(distanceL > distanceR)
       {
         car_left();
         u_servo.write(90);
         delay(400);
       }
       else
       {
         car_right();
         u_servo.write(90);
         delay(400);
       }
     }
     else
     {
       digitalWrite(ML,LOW);
       analogWrite(ML_PWM,150);
       digitalWrite(MR,LOW);
       analogWrite(MR_PWM,150);
     }
   }

   float checkdistance() {
     digitalWrite(Trig, LOW);
     delayMicroseconds(2);
     digitalWrite(Trig, HIGH);
     delayMicroseconds(10);
     digitalWrite(Trig, LOW);
     float distance = pulseIn(Echo, HIGH) / 58.00;
     delay(10);
     return distance;
   }

   void tracking()
   {
     boolean trackL_val = digitalRead(trackL);
     boolean trackR_val = digitalRead(trackR);
     Serial.print(trackL_val);
     Serial.print("  ");
     Serial.println(trackR_val);
     if((trackL_val == 1) && (trackR_val == 1))
     {
       digitalWrite(ML,LOW);
       analogWrite(ML_PWM,120);
       digitalWrite(MR,LOW);
       analogWrite(MR_PWM,120);
     }
     else if((trackL_val == 1) && (trackR_val == 0))
     {
       digitalWrite(ML,HIGH);
       analogWrite(ML_PWM,150);
       digitalWrite(MR,LOW);
       analogWrite(MR_PWM,150);
     }
     else if((trackL_val == 0) && (trackR_val == 1))
     {
       digitalWrite(ML,LOW);
       analogWrite(ML_PWM,150);
       digitalWrite(MR,HIGH);
       analogWrite(MR_PWM,150);
     }
     else
     {
       car_stop();
     }
   }

   void face1()
   {
     if(face1_flag==0){
       matrix_flag = 1;
     }
     if(matrix_flag == 1)
     {
       face_count++;
       if(face_count == 6)
       {
         face_count = 6;
       }
       matrix_flag = 0;
       face1_flag = 1;
     }
     switch(face_count)
     {
       case 1: myMatrix.clear();myMatrix.writeDisplay();matrix_display(matrix_smile); break;
       case 2: myMatrix.clear();myMatrix.writeDisplay();matrix_display(matrix_tsundere); break;
       case 3: myMatrix.clear();myMatrix.writeDisplay();matrix_display(matrix_squinting); break;
       case 4: myMatrix.clear();myMatrix.writeDisplay();matrix_display(matrix_despise1); break;
       case 5: myMatrix.clear();myMatrix.writeDisplay();matrix_display(matrix_speechless); break;
       case 6: myMatrix.clear();myMatrix.writeDisplay();matrix_display(matrix_heart); break;
     }
   }

   void face_stop()
   {
     myMatrix.clear();myMatrix.writeDisplay();
   }

   void face2()
   {
     if(face1_flag==0){
       matrix_flag = 1;
     }
     if(matrix_flag == 1)
     {
       face_count--;
       if(face_count == 1)
       {
         face_count = 1;
       }
       matrix_flag = 0;
       face1_flag = 1;
     }
     switch(face_count)
     {
       case 1: myMatrix.clear();myMatrix.writeDisplay();matrix_display(matrix_smile); break;
       case 2: myMatrix.clear();myMatrix.writeDisplay();matrix_display(matrix_tsundere); break;
       case 3: myMatrix.clear();myMatrix.writeDisplay();matrix_display(matrix_squinting); break;
       case 4: myMatrix.clear();myMatrix.writeDisplay();matrix_display(matrix_despise1); break;
       case 5: myMatrix.clear();myMatrix.writeDisplay();matrix_display(matrix_speechless); break;
       case 6: myMatrix.clear();myMatrix.writeDisplay();matrix_display(matrix_heart); break;
     }
   }

   int matrix_display(uint8_t led_array[8]){
     for(int i=0; i<8; i++)
     {
       LEDArray[i]=led_array[i];
       for(int j=7; j>=0; j--)
       {
         if((LEDArray[i]&0x01)>0)
         myMatrix.drawPixel(j, i,1);
         LEDArray[i] = LEDArray[i]>>1;
       }
     }
     myMatrix.writeDisplay();  // dot matrix shows
   }


   void func_neo1()
   {
     if(neo_state == 0)
     {
       neo_flag++;
       neo_state = 1;
     }
     if(neo_flag >= 6)
     {
       neo_flag = 6;
     }
     switch(neo_flag)
     {
       case 1: for (int i = 1; i <= 4; i = i + (1)) {
         rgb_display_A3.setPixelColor(i-1, (((100 & 0xffffff) << 16) | ((0 & 0xffffff) << 8) | 0));rgb_display_A3.show();
       }
       break;
       case 2: for (int i = 1; i <= 4; i = i + (1)) {
         rgb_display_A3.setPixelColor(i-1, (((0 & 0xffffff) << 16) | ((100 & 0xffffff) << 8) | 0));rgb_display_A3.show();
       }
       break;
       case 3: for (int i = 1; i <= 4; i = i + (1)) {
         rgb_display_A3.setPixelColor(i-1, (((0 & 0xffffff) << 16) | ((0 & 0xffffff) << 8) | 100));rgb_display_A3.show();
       }
       break;
       case 4: for (int i = 1; i <= 4; i = i + (1)) {
         rgb_display_A3.setPixelColor(i-1, (((100 & 0xffffff) << 16) | ((100 & 0xffffff) << 8) | 0));rgb_display_A3.show();
       }
       break;
       case 5: for (int i = 1; i <= 4; i = i + (1)) {
         rgb_display_A3.setPixelColor(i-1, (((0 & 0xffffff) << 16) | ((100 & 0xffffff) << 8) | 100));rgb_display_A3.show();
       }
       break;
       case 6: for (int i = 1; i <= 4; i = i + (1)) {
         rgb_display_A3.setPixelColor(i-1, (((100 & 0xffffff) << 16) | ((100 & 0xffffff) << 8) | 100));rgb_display_A3.show();
       }
       break;
     }
     
   }

   void func_neo2()
   {
     if(neo_state == 0)
     {
       neo_flag--;
       neo_state = 1;
     }
     if(neo_flag <= 1)
     {
       neo_flag = 1;
     }
     switch(neo_flag)
     {
       case 1: for (int i = 1; i <= 4; i = i + (1)) {
         rgb_display_A3.setPixelColor(i-1, (((100 & 0xffffff) << 16) | ((0 & 0xffffff) << 8) | 0));rgb_display_A3.show();
       }
       break;
       case 2: for (int i = 1; i <= 4; i = i + (1)) {
         rgb_display_A3.setPixelColor(i-1, (((0 & 0xffffff) << 16) | ((100 & 0xffffff) << 8) | 0)); rgb_display_A3.show();
       }
       break;
       case 3: for (int i = 1; i <= 4; i = i + (1)) {
         rgb_display_A3.setPixelColor(i-1, (((0 & 0xffffff) << 16) | ((0 & 0xffffff) << 8) | 100)); rgb_display_A3.show();
       }
       break;
       case 4: for (int i = 1; i <= 4; i = i + (1)) {
         rgb_display_A3.setPixelColor(i-1, (((100 & 0xffffff) << 16) | ((100 & 0xffffff) << 8) | 0));rgb_display_A3.show();
       }
       break;
       case 5: for (int i = 1; i <= 4; i = i + (1)) {
         rgb_display_A3.setPixelColor(i-1, (((0 & 0xffffff) << 16) | ((100 & 0xffffff) << 8) | 100)); rgb_display_A3.show();
       }
       break;
       case 6: for (int i = 1; i <= 4; i = i + (1)) {
         rgb_display_A3.setPixelColor(i-1, (((100 & 0xffffff) << 16) | ((100 & 0xffffff) << 8) | 100));rgb_display_A3.show();
       }
       break;
     }
     
   }

   void neo_stop()
   {
     neo_state = 0;
     for (int i = 1; i <= 4; i = i + (1)) {
       rgb_display_A3.setPixelColor((i)-1, (((0 & 0xffffff) << 16) | ((0 & 0xffffff) << 8) | 0));rgb_display_A3.show();
     }
   }

   void car_forward()
   {
     digitalWrite(ML,LOW);
     analogWrite(ML_PWM,left_val);
     digitalWrite(MR,LOW);
     analogWrite(MR_PWM,right_val);
   }

   void car_back()
   {
     digitalWrite(ML,HIGH);
     analogWrite(ML_PWM,(255-left_val));
     digitalWrite(MR,HIGH);
     analogWrite(MR_PWM,(255-right_val));
   }

   void car_left()
   {
     digitalWrite(ML,HIGH);
     analogWrite(ML_PWM,127);
     digitalWrite(MR,LOW);
     analogWrite(MR_PWM,127);
   }

   void car_right()
   {
     digitalWrite(ML,LOW);
     analogWrite(ML_PWM,127);
     digitalWrite(MR,HIGH);
     analogWrite(MR_PWM,127);
   }

   void car_stop()
   {
     digitalWrite(ML,LOW);
     analogWrite(ML_PWM,0);
     digitalWrite(MR,LOW);
     analogWrite(MR_PWM,0);
   }
   //**********************************************************************************

3. APP操作，如下图。

可实现小车前、后、左、右电机控制，控制蜂鸣器鸣叫和播放音乐，控制RGB灯、点阵功能，控制小车循迹、避障、寻光和跟随等功能。

|2023-07-01_140100|

.. |img| image:: ./img/b3a038ae2b7a644dcd4255d8bb48a4ab.png
.. |image1| image:: ./img/e9b7164b9c464642cd29c5a437e99212.png
.. |image2| image:: ./img/6a0a425a0f77b70224c2cf2a16924efc.png
.. |image3| image:: ./img/5f74a2b7c80c703878975e687447d51f.png
.. |image4| image:: ./img/6f703ca32fc060617688e8afa9fd8a78.png
.. |image5| image:: ./img/ed23c424fc333857d61e7762e808140d.png
.. |image6| image:: ./img/8d0c2c24e10cf33209e7e718977fc16c.png
.. |image7| image:: ./img/4fd867a252ec6fff2804fc046d97f02a.png
.. |image8| image:: ./img/e979f8ed3570e353d11715a461af4ba7.png
.. |image9| image:: ./img/5b5c18a5f27fbe61f1ee0b015010cbae.png
.. |image10| image:: ./img/b666e6a6b6863b7943cbeb8d7fcdddfc.png
.. |Img| image:: ./media/img-20250507135020.png
.. |image11| image:: ./img/f29997b5880f536087c51e8c9a5fdc1f.png
.. |image12| image:: ./img/1f3c008adb6d1e7dadf797f142203baf.png
.. |image13| image:: ./img/ce0e4329fd21cd1b81d59f73968d4ad1.png
.. |image14| image:: ./img/6be5eb6ef9b24c9835e1603c0c135b73.png
.. |image15| image:: ./img/31f32d9721d7b5991e1c954b6b80f39f.png
.. |image16| image:: ./img/ef67bcdcf0340ef46ae0c5d8f2dc7c67.png
.. |image17| image:: ./img/cea9acd41af51a00bbe781f2e6f3a48c.png
.. |image18| image:: ./media/img-20250507135541.png
.. |image19| image:: ./img/d49f7693d4af256d9f59653ef7e8eb62.png
.. |image20| image:: ./media/img-20250507140106.png
.. |image21| image:: ./img/e2c5b97ed534bc382cb50b05498b445d.png
.. |image22| image:: ./img/7f7365967c1556604179415a67b03f7b.png
.. |image23| image:: ./img/28f3235b60a49be9cb20087d9542d390.png
.. |image24| image:: ./img/17905dc94b39de00e0d3c872363f3bb1.png
.. |image25| image:: ./img/bff846d943f6d7ba6168856233bb37f6.png
.. |image26| image:: ./img/096c2b8f73b4b12982a065d37c7ff848.png
.. |image27| image:: ./img/2e0f4e1c611dd272a7f5b99ed66e8c6d.png
.. |image28| image:: ./img/4ff5fd5171d1de67eb694e90464a3c2a.png
.. |image29| image:: ./img/0c6f8953cd1687bd71e0d9b5aed459fc.png
.. |image30| image:: ./img/5ecac913601bd56d8fdaff2a318cb610.png
.. |image31| image:: ./img/a7ee2b56f0b22a8933c26e1b13021ea5.png
.. |image32| image:: ./img/867d6e1de673fdb4e5a06c8017e3b270.png
.. |image33| image:: ./img/f9a1bd4b7cdbcdb902f0279be65ad004.png
.. |image34| image:: ./img/7a4185384de3ab0958cdd9a8353c3c84.png
.. |image35| image:: ./img/be43ef69c2fd2c1c2723d24468573cc4.png
.. |image36| image:: ./img/8b9100cce770c8f5419d0ec0563631d7.png
.. |image37| image:: ./img/beaee4aa464de7c9f47add9d0134009c.png
.. |image38| image:: ./img/131eff95de6085d7c6ed6714800165d8.png
.. |image39| image:: ./img/f5977283eff4c7b0a53951e8e311ebec.png
.. |image40| image:: ./img/2201137b009927a36b8fe1afe2ed15b1.png
.. |image41| image:: ./img/a5b4e321220aa6c7868c5dec0e7a2715.png
.. |image42| image:: ./img/a51be6d5e18021eb37abc2ea6c74d15d.png
.. |image43| image:: ./img/118625117684778402498298bf190dac.png
.. |image44| image:: ./img/a6e562b5eb9ddccdfed732d651d40782.png
.. |image45| image:: ./img/aff7ecb420c322fee9d9de3e75eeb45a.png
.. |image46| image:: ./img/b80b728f5a534ec46b2fe2fd7a8d708f.png
.. |image47| image:: ./img/b73f11967672269f810326cc2a0d4a29.png
.. |image48| image:: ./img/f1df4d95cb851b82d25596e253d8f677.png
.. |image49| image:: ./img/e6bea10210e2d3735df0b55c4d61da16.png
.. |image50| image:: ./img/c817703031ecbe7cb77dcf3ba219ecdc.png
.. |image51| image:: ./img/7d1ea114f1407074233e67675a70d2e3.png
.. |image52| image:: ./img/241b86fb829ce685efa08b96be05955c.png
.. |image53| image:: ./media/img-20250506165645.png
.. |image54| image:: ./img/a8f6709e5a632b99a84fa92a0a19a9ef.png
.. |image55| image:: ./img/27bc39fdd33e565aa5941312d72cb9c5.png
.. |image56| image:: ./img/2afb6740208c23db41b6915e111d9f96.png
.. |image57| image:: ./img/1ac0e42df914a36e6c7151e663efbee5.png
.. |image58| image:: ./img/c8944fba70e9063746089e60cbbaa895.png
.. |image59| image:: ./img/e6ebe93729ed6417c3bd001bdd08d97e.png
.. |image60| image:: ./img/b74daf2b842ca755aa816cfb49476025.png
.. |image61| image:: ./img/568f7d83c5d3c6779be0a63557e996a8.png
.. |image62| image:: ./img/6cf3210c945571f558a8ab14d23fe9f8.png
.. |image63| image:: ./img/8902bf63965998b38da6855f2408b0fa.png
.. |image64| image:: ./img/6978dba6cec6ec2574f1fc60bca20649.png
.. |image65| image:: ./img/4cbad70822552466bd5be1344c50c84f.png
.. |image66| image:: ./img/51cd0bb3497a05dc5c8dd0fb0835b05c.png
.. |image67| image:: ./img/4291e559a26b63b79ad9be643c27a61b.png
.. |image68| image:: ./img/d7b9fdf1d37256fb218453e88d74dc3a.png
.. |image69| image:: ./img/d29698a3d45116f4f993fb345e43f86e.png
.. |image70| image:: ./img/31838ecc19d439ae795efbf0803cc321.png
.. |image71| image:: ./img/199b3964695cd66e61195e70a11f2c22.png
.. |image72| image:: ./img/4b3c136b7c1efc680fa14725133ee889.png
.. |image73| image:: ./img/0986986b8f851f2318e7351ae69516b9.png
.. |image74| image:: ./img/8a2b454cedad5e8049b540f8b573c858.png
.. |image75| image:: ./img/a5b69a16cf6dc2cda08225591eb43702.png
.. |image76| image:: img/268e08be6b5a34a5f9c1173ad3e0afc1.png
.. |image77| image:: img/1fd8374eca6b82f577a7efc097c74469.png
.. |image78| image:: img/86e292d0666046b72a1e0e68adfb17e8.png
.. |image-20230701141308990| image:: ./img/e372085d11dbc0fef8fb01c10f10c5ba.png
.. |image79| image:: ./img/468ca6e05b6ea2aa7fc8de0fefb41279.png
.. |image80| image:: ./img/7dcd8e8777afbce5eb8a13b0094acfae.png
.. |image81| image:: ./img/d8d87f9799ab2765c64976b9d505f2d8.png
.. |image82| image:: ./img/cc40a878dba4747ee74ca12fc721c577.jpg
.. |image83| image:: ./img/89afd416fead663ee51bc77c527b77db.jpg
.. |image84| image:: ./img/7c59ab3c12b318ff777ed4d8c1802f4d.jpg
.. |image85| image:: ./img/2eafcb3b223fcaa99cd39e1560e9c567.jpg
.. |image86| image:: ./img/8216886ff73de29d166d219358df924b.jpg
.. |img-20230531141128| image:: ./img/74b4d05014830e9730c37c4638b06ec6.jpg
.. |image87| image:: ./img/095a2a284be6399674293f2483baad91.jpg
.. |image88| image:: ./img/648f9401dbf37fb3ebeeca0ba844a100.png
.. |image89| image:: ./img/45c9a62519ce5957279c900c76e9581a.jpg
.. |image90| image:: ./img/e0cfccb2e7c2f5466526e36a309680e0.jpg
.. |image91| image:: ./img/4f1aeb23ec0776866fa15770ea667007.jpg
.. |image92| image:: ./img/45766e6912d003fb9b7d9d7bc8b64f44.jpg
.. |image93| image:: ./img/19a7d7b8b781b96e522d76e24ccb4250.jpg
.. |image94| image:: ./img/214e242a571d2a7640fa158d3b1ef5d4.jpg
.. |image95| image:: ./img/6a911bafb450a10052ff5629e51d029f.jpg
.. |image96| image:: ./img/4c755de678c244e4bbad6c2aee2fab1a.png
.. |image97| image:: ./img/19fe9dff26120114ec82afd8155c7496.jpg
.. |img-20230518083845| image:: ./img/b72e7eac78576768030175967685d93d.png
.. |image98| image:: ./img/62e52b99bea115bd0542aba2a1f6daea.jpg
.. |img-20230518083634| image:: ./img/b7056f0656565bc6b70ad34fcf4b9005.png
.. |image99| image:: ./img/fbf6114bc89b2e606c5f957e3527fa2e.jpg
.. |image-20230701141513611| image:: ./img/72ea28d3025cb43be4960a0d7415275b.png
.. |image-20230701114014751| image:: ./img/52d5146feff9ff8d89320f40e9acf7d9.png
.. |img-20230518082944| image:: ./img/94f4dae1640a9ee3bc9da6640e7d6d8f.png
.. |image100| image:: ./img/9b8dff0696b77e68e559fcacb82a5abd.jpg
.. |img-20230508101729| image:: ./img/img-20230508101729.png
.. |img-20230508101203| image:: ./img/c0ef8c45e0deb300f02dc042d706c114.png
.. |image101| image:: ./img/7d0eeb0f0c69130b020c5e5840d1ca84.jpg
.. |img-20230518083512| image:: ./img/a134587241cbee2f4b48bc5205eedaaa.png
.. |image102| image:: ./img/be6d1bf04bfc5fd993187dcad3147a5a.jpg
.. |image103| image:: ./img/87e3e900c13153bf53395faa4853cdc0.jpg
.. |image104| image:: ./img/3dba0ac96be665009a0eb35b5f2719da.jpg
.. |image105| image:: ./img/e155f3a67478960882cf36f67ca5f783.jpg
.. |image106| image:: ./img/6047d6df76cf7a5139eef1484e51e3b3.jpg
.. |image107| image:: ./img/dd3e5ba64fe62b1ed2ab6dfca87acd96.jpg
.. |image108| image:: ./img/6bc5562a488cdd2b9da67e85e043c66d.jpg
.. |image109| image:: ./img/435d61f87a975058df8f44a5da66fc1c.jpg
.. |image110| image:: ./img/ecf7103411099cad4bcd8c8ca02fc9b5.jpg
.. |image111| image:: ./img/af0c76f1e716472fef8afe63180102ef.jpg
.. |image112| image:: ./img/ed97d0fec17c230bcdb6982456c9372d.png
.. |img-20230518082547| image:: ./img/aa7f0455a8054bd2dd9824ea096703e0.png
.. |image113| image:: ./img/6686fb6a5fa369cf1dca7965f9d07588.jpg
.. |image114| image:: ./img/5b38862d54ed0e1721bc8d74d4896f6b.jpg
.. |image115| image:: ./img/6279fedd5047b9825770517dca7ce32e.jpg
.. |image116| image:: ./img/8acad3f097c6be8c098a51b935b4a332.jpg
.. |image117| image:: ./img/4d1d763f124bfb50ac2f0c06e2e3b0f0.jpg
.. |image118| image:: ./img/b9b334ce33b0d5598623ecbd19cee4ab.jpg
.. |image119| image:: ./img/wps42.jpg
.. |image120| image:: ./img/3b45391fb485edd6cb63aab10aa3cc54.png
.. |image121| image:: ./img/7c3a0edbed1e3dc4f146ed8ea76b3fb9.png
.. |image122| image:: ./img/2149680b806329c7072b08150a1a68d6.jpg
.. |image123| image:: ./img/832a5cc79de1ae8b5b0e846e4a64646e.jpg
.. |image124| image:: ./img/d0edef0f6ef2cdaf4c0f33c28ba403a2.jpg
.. |image125| image:: ./img/76f52c7837abf06bb0e53cb2affef519.jpg
.. |image126| image:: ./img/e6785d5be5f1e2db4c27215bc1b8eb4b.png
.. |image127| image:: ./img/e6ac4a5525075915c47eab7e14bd554d.jpg
.. |image128| image:: ./img/d8ea27544c70220228a60392c6a4606d.jpg
.. |image129| image:: ./media/img-20250507094719.png
.. |image130| image:: ./media/img-20250507094742.png
.. |image131| image:: ./media/img-20250507095306.png
.. |image132| image:: ./img/e8babb1e9fd40b7ab46dedd854e8c8b6.jpg
.. |image133| image:: ./img/66cfec811b4510bbaa0fc4a7c757e8bf.jpg
.. |image134| image:: ./img/f4c82df9d5fae8ff88ce3477e72308ba.jpg
.. |image135| image:: ./img/d8ea27544c70220228a60392c6a4606d.jpg
.. |image136| image:: ./media/img-20250507094719.png
.. |image137| image:: ./media/img-20250507094742.png
.. |2023-07-01_132611| image:: ./img/665ef575c4ec0260c06ba9454b2470f1.png
.. |image138| image:: ./img/ff6a9e322b3a91d8725da6014783146b.jpg
.. |image139| image:: ./img/e8babb1e9fd40b7ab46dedd854e8c8b6.jpg
.. |image140| image:: ./img/66cfec811b4510bbaa0fc4a7c757e8bf.jpg
.. |image141| image:: ./img/f4c82df9d5fae8ff88ce3477e72308ba.jpg
.. |image142| image:: ./img/fca5cf2a734a095ecd6024a84b9e0f7e.jpg
.. |image143| image:: ./img/wps65.jpg
.. |image144| image:: ./img/wps66.jpg
.. |image145| image:: ./img/wps67.jpg
.. |image146| image:: ./img/76f52c7837abf06bb0e53cb2affef519.jpg
.. |image147| image:: ./img/e6785d5be5f1e2db4c27215bc1b8eb4b.png
.. |image148| image:: ./img/b7c05c445dd30cf5ec743fb09bfec1fc.jpg
.. |image149| image:: ./img/wps71.jpg
.. |image150| image:: ./img/wps73.jpg
.. |image151| image:: ./img/wps75.jpg
.. |image152| image:: ./img/wps76.jpg
.. |image153| image:: ./img/wps77.jpg
.. |image-20230701141106477| image:: ./img/image-20230701141106477.png
.. |image-20230701140459935| image:: ./img/image-20230701140459935.png
.. |image154| image:: ./img/wps80.jpg
.. |image155| image:: ./img/wps81.png
.. |image156| image:: ./img/wps82.jpg
.. |image157| image:: ./img/wps84.png
.. |image158| image:: ./img/wps85.jpg
.. |image159| image:: ./img/wps86.png
.. |image160| image:: ./img/wps87.jpg
.. |image161| image:: ./img/wps88.png
.. |image162| image:: ./img/wps89.png
.. |image163| image:: ./img/wps90.jpg
.. |image164| image:: ./img/wps91.jpg
.. |image165| image:: ./img/wps92.jpg
.. |image166| image:: ./media/img-20250507090501.png
.. |image167| image:: ./img/wps94.jpg
.. |image168| image:: ./img/wps96.jpg
.. |img-20230518083704| image:: ./img/46277ad803e4c3c05e1d31afa5e1b088.png
.. |2023-07-01_134851| image:: ./img/928e2e0bc9141b7852322adfaccc2328.png
.. |2023-07-01_134850| image:: ./img/8aac71e4a6a52f11591731d25ab90057.png
.. |2023-07-01_140100| image:: ./img/36ffeedf595e0750e42b83a86c693a73.png
