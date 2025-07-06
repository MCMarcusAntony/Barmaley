--------------------------------------------------------------------------------
Barmaley Variable Load Cartridge
Copyright (c) 2024-2025 RBSC
Last updated: 06.07.2025
--------------------------------------------------------------------------------

About
-----

WARNING!
PUTTING EXCESSIVE LOAD ON THE POWER SUPPLY MAY DAMAGE IT, SO USE WITH CAUTION!
WARNING!

The RBSC is proud to present yet another project for the MSX platform. It's called "Barmaley". Barmaley is the evil
character from the Russian cartoon, the antagonist of doctor Aibolit. As you probably remember, the iBolit2 project that
RBSC presented some time ago, helps to diagnose and fix MSX computers. Barmaley, on the contrary, is designed to test
and stress-test MSX computers, their power rails in particular.

The device is a large size air-cooled cartridge that imposes variable load on all 3 power rails of MSX computer. It can
test each power rail with variable loads and it can also test all of them at the same time. The load stepping for the 5V
rail is 150mA, for +12V and -12V the stepping is 25mA. According to the standard, MSX should provide 300mA for each
cartridge slot (600mA in total) and 50mA on both 12V power rails together. This load can be set with eight small slide
switches on the board. When the load is activated, the corresponding LED is lit.

It's important to remember that all resistors that are used to test MSX's power rails must be aircooled, otherwise their
temperature will exceed 150 degrees Celsius. Both fans consume up to 350-400mA, so only two 5V load resistors should be
activated to reach the designed load on the 5V rail. However, 2 more resistors can be still activated to stress-test the
power supply, bringing the total load on the 5V rail to 1A. For +12V and -12V power rails only one of two resistors
should be activated - this brings the total load to 50mA. It's still possible to activate 2 additional load resistors to
bring the load to 50mA for each of 12V power rails.


Usage instructions
------------------

Before inserting Barmaley cartridge into a computer make sure that all switches are in the OFF (lower) position. Then
power up your computer and first switch on both fans. Then you can gradually increase the load on all power rails.

Start with the 5V power rail - activate one switch and see if there's any anomaly, then activate the second switch and
keep an eye on computer's power supply. If you see anything suspicious (smoke, sparks) or smell anything overheated or
burnt, immediately switch off the computer and check the power supply.

As stated above, with working fans only 2 switches may be activated on the 5V power rail and only one swich may be
activated on either 12V power rails. That will bring the load capacity to the one described in the MSX standard. Most
of power supplies will work with all activated switches as they were designed to withstand the excessive load. But
not all power supplies are equal and some of them may be on the brink of failure. So, applying excessive load is likely
to cause them to fail sooner than later.

Certain computers, for example Casio PV series and some others do not have power on 12V power rails, so it will not be
possible to test these power rails. Switching on any of 12V load switches will not produce any visible result.

If you have other cartridges inserted into MSX slot beside Barmaley, please keep in mind that those cartridges may
(and will) draw power, so the total load on power rails will be higher. If you would like to test your computer with
third-party cartridges, please adjust the applied load accordingly (for example activate one less switch on 5V power
rail).


Where to buy parts
------------------

The parts for assembling the cartridge can be purchased from these sellers on AliExpress:

 - https://www.aliexpress.com/item/1005003595630530.html	(40x40x10 5V DC brushless fans)
 - https://www.aliexpress.com/item/32971605141.html		(18mm M3 bolts)
 - https://www.aliexpress.com/item/1005007593861199.html	(M3 nuts)
 - https://www.aliexpress.com/item/1005005600798857.html	(SMD resistors)
 - https://www.aliexpress.com/item/1005006003779801.html	(through-hole 2W resistors)
 - https://www.aliexpress.com/item/1005004324474428.html	(transparent plastic washers)
 - https://www.aliexpress.com/item/32799108713.html		(dual-color or just any simple 5mm LED)
 - https://www.aliexpress.com/item/4000933759536.html		(XH2.54 2-pin fan connectors)
 - https://www.aliexpress.com/item/1005004436568134.html	(flat 2x5x7mm LEDs of 4 different colors)
 - https://www.aliexpress.com/item/4000699811538.html		(MSS22D18 miniature DIP slide switch, 6-pin, 2-pos)
 - https://www.aliexpress.com/item/1005007660225984.html	(5mm long 3.2mm inner diameter spacer)

The 3D model of the 5mm spacer for both fans (you will need 8 pieces) could be found here in the "3DModel" subfolder
of Barmaley's repository.


Assembling notes
----------------

Please read the following notes carefully:

 - Use only resistors with defined resistance and wattage, otherwise they may be damaged or a damage occurs to your MSX
   computer. The resistance is calculated according to MSX standards and exceeding it is always a risk

 - It is important to cool down installed resistors, otherwise their temperature will exceed 150 degrees Celsius and may
   cause burns and degradation of these components. During the operation both fans must be always working

 - It's is strongly advised to install washers on the front side of the board under all bolts that hold both fans. The
   best cosmetic results could be achieved by installing transparent plastic washers (see above for the product's link)

 - Both fans must be installed with a 5mm high 3D-printed spacer or with a similar factory-made spacer. The fans must
   stay at least 5mm away from the back of the circuit board in order to provide adequate cooling for load resistors
   (see above for the product's link)

 - Both fans must be installed so that their airflow is directed fowards - to cool down all load resistors

 - If fans have too long cables, it's advised to either shorten them or to use cable ties to organize the cables on the
   back side of the board. Make sure that cables don't block the rotation of either fan

 - For securing fans to the circuit board use eight 18mm long 3mm (M3) bolts and nuts. Longer bolts are not recommended

 - Do not bridge the SW1+2 solder jumper pad unless your MSX computer refuses to power on with the inserted Barmaley
   cartridge

 - It's advised to use green LEDs for fan indication, blue LEDs for -12V power rail indication, yellow LEDs for +12V
   power rail indication and red leds for +5V power rail indication


IMPORTANT!
----------

The RBSC provides all the files and information for free, without any liability (see the disclaimer.txt file). The provided
information, software or hardware must not be used for commercial purposes unless permitted by the RBSC. Producing a small
amount of bare boards for personal projects and selling the rest of the batch is allowed without the permission of RBSC.

When the sources of the tools are used to create alternative projects, please always mention the original source and the
copyright!

The Barmaley logo was created by the digital artist named Alu Orlov (alu.orlov.art @ gmail.com) based on existing character
design. She has also created RBSC's main logo, iBolit2 logo, as well as Carnivore2 and 2+ stickers and carton boxes. If you
would like to have a cool logo or any other form of digital art, contact her by e-mail.


Contact information
-------------------

The members of RBSC group Tnt23, Wierzbowsky, Pyhesty, Ptero, GreyWolf, SuperMax, VWarlock, ALSP and DJS3000 can be contacted
via the group's e-mail address:

info@rbsc.su

The group's coordinator could be reached via this e-mail address:

admin@rbsc.su

The group's website can be found here:

https://rbsc.su/
https://rbsc.su/ru

The RBSC's hardware repository can be found here:

https://github.com/rbsc

The RBSC's 3D model repository can be found here:

https://www.thingiverse.com/groups/rbsc/things

-= ! MSX FOREVER ! =-
