## day 1:

firstly sorry this is like the next day of work in which i started writing this, anyways on day one i figured out what i wanted to make, it was just a small usb type c board with "analog" components so like no mcu, no programming, it uses a hr202 resistive humidity sensor and then with that was going to originally use a 555 timer to generate ac to power it and then have the value measured with some other ic, icl it was all overcomplicated as shit cuz i was using google overview for help and google overview is uh, well i don't trust any google model to do literally anything anymore, they are consistently just so so so buns, anyways so i left the day with a components list i had thought up and such pretty much and a repo to work in.


## day 2:

day 2 like second day i really worked, being today ofc.
so firstly i am writing this but other than that i basically stopped talking to google abt the project which helped and then i spent a couple hours legit watching tutorials to understand the 555 timer, which in the end i did not use lmao.

so i replace the whole overcomplicated circuit i had with a 55 for ac generation to just use a LTC1799, its a dc to ac generator that generates based on like a resistor a division factor controlled by just two pins, and so basically it made my life a lot a lot easier and i didnt have to deal with as much bullshit cuz i lowk havent used the 555 which is crazy but i just use mcus for the most part, anyways so i in the end got a usb 6pin for power only with 2 resistors at 5.1k so it can do c to c and then ofc i have my decoupling caps on everything like the components and as for the components like i mentioned i have a LTC1799, and then i also have a AD8307ANZ, this goober is just a log amp and from what i know, it, well while it isnt perfect at it it converts the like logarithmic response curve of the hr202 to sum normal that can then be read by a voltimeter, which is basically all i do, evereything goes out to 3 pins, one for voltimeter like signal, the others for 5v and gnd and then thats abt it really, the pcb is also pretty small, anyways ill attatch images of everything now, thanks for reading :)

![[cloudsensor/images/schematic.png]]![[cloudsensor/images/pcb.png]]![[render.png]]

oh lastly for credits i did use deepseek for a lot of help as im new to not working with an mcu lol, but yeah i had a lot of fun and im happy its done!

oh lastly heres the bom.csv
![[cloudsensor/images/bom.png]]

so with a bom done and this journal and the pcb all thats left is to fix up the readme and ship :)



made with love.
bye oxy <3