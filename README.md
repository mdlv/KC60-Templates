# KC60-Templates
Various configuration files for the KC60 programmable keyboard.

The KC60 is great entry point for a low-cost programmable keyboard. While a little rough around the edges, it gives you full control over how the keyboard behaves. On the downside, programming functions can be a bit challenging if you can't read Chinese or have little or no experience with keyboard programming. These templates serve to help ease the process and help clear up some of the issues commonly encountered when working with this keyboard.

Included:
<ul>
<li>KC60 Basic: this is my current setup</li>
</ul>

To do:
<ul>
<li>Poker II default</li>
<li>Pok3r default</li>
<li>HHKB default</li>
<li>Provide links to configurator</li>
</ul>

<hr>

About the keyboard:
Manufactured by NPKC
60% standard layout
Programmable layers
Plate mounted Costar stabilizers
Cherry MX or Gateron switch compatible
Mini USB interface
Compatible with 60% cases that work with Poker
Plate mounted
ATmega32u4 controller
Windows / OSX Compatible
Plate has notches for switch top removal


Programming guide:
First, you're going to need the TKG tookit in order to reflash the board. This assumes your on a PC.
https://github.com/kairyu/tkg-toolkit.git

Second, you'll need to generate a .hex file from the config tool.
http://123.57.250.164:9128/

The config tool, despite being in Chinese, is fairly easy to use once you get the hang of it. Really it's just the functions that need attention. When assigning a function you'll be presented with the following options in the drop down. Here are the translations. I've expanded on a few of the options to better explain how they work (this is a work in progress).
空操作 – No operation
瞬时开启层 – Instantaneous open layer
The difference between this and open layer, is that this keeps the layer open while the key is depressed, while Open keep it open until you press the key you've assigned to close the layer.
开启层 – Open layer
关闭层 – Close Layer
开关层 – Switch layer
瞬时开启、 按键Momentary open , button
This option allow you to use the key normally by tapping, but opens a function layer while it is held down.
修饰键 – Modifier keys
组合键 – Key combination
单击修饰键 – Click modifier keys
开关修饰键 – Switch modifier keys
清除层状态 – Clear layer status
宏 – Macros

Here is an excellent guide from the developer of the TKG toolkit. 
https://github.com/tmk/tmk_keyboard/blob/master/tmk_core/doc/keymap.md

Here is a blog post over at Keychatter summing up the process, with some discussion in the comments that might be helpful.
https://www.keychatter.com/2015/07/05/programming-the-kc60/

Another link with some helpful notes:
https://gist.github.com/Leimi/4bf07c0822ba8b2cfaad

TIPS:
-  Install the drivers included with the toolkit
-  If you're using an aftermarket case, if there is not cutout for dip switches you won't be able to access the reset button. In which case you're want to remove the board from the case before relashing.
-  There are numerous mentions of the "did you forget to press reset" message when reflashing. They key is to hold it down for a good long while. I would say between 1 and 2 minutes. I didn't get any feedback from the installer until I let go of the reset button. I should also mention that at some point in my many attempts, they keyboard stopped working completely. DO NOT WORRY, just install the drivers and reflash and it should come back.
When relashing, be sure to install the drivers included with the toolkit. 

