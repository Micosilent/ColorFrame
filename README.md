# ColorFrame
DIY LED panel
--------------------------------------------------
The object of this project is to create a modular LED panel that can display
images and animations in a 8bit style (like retrogame sprites or low res images)

The total project consists of a set of slaves, that will be an atmega mcu wich
will control a led array of 16 RGB pixels in width and height. And a computer
or raspberrpi master, that will extract the RGB values from the images or animations
and send them to the slaves.

*****************************************************
*****************************************************

TODO:


Slaves:
------------------------------------------
    -Control of LED array
    -Recive frama data
      -Over SPI
      -Be able to send a ACK in order to framesync

Master:
------------------------------------------
    -Decode
      -Bitmaps
      -Animations
      -Videos??
    -Send frame data to each slave
    -Serve a webpage to configure and control the ColorFrame
    -Maybe Colorchord? https://github.com/cnlohr/colorchord


********************************************************
********************************************************

Masters will be probably python coded, and slaves can be prototyped in arduino
IDE but, should probably be codded in native AVR code in order to maximize fps
and enable us to use a smaller mcu
