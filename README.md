## bert-ev3dev-examples
### Examples of bits and pieces running at Jessie level 

These shell-scripts are located on my EV3-brick at `/usr/local/bin`
but with some simple edits you can place them where **you** want them.

 1. Supporting script(s) used by other scripts
    * [asciicolor] (https://github.com/BertLindeman/bert-ev3dev-examples/blob/master/asciicolors)

 2. Scripts related to managing the EV3-brick
    * [checkpower](https://github.com/BertLindeman/bert-ev3dev-examples/blob/master/checkpower)
    * [showactivity](https://github.com/BertLindeman/bert-ev3dev-examples/blob/master/showactivity)
    * [stopmotors](https://github.com/BertLindeman/bert-ev3dev-examples/blob/master/stopmotors)

 3. Scripts discovering sensors and / or motors
    * blinkleds
    * setled
    * showleds
    * showmotor
    * showpower
    * showsensors
    * showsound
    * testmotor 

### Have your EV3 report it's IP-address by speach after boot
For this an update is needed to `/media/mmc_p1/ev3dev.rc.local` 
and an extra script `tellIP` in the same directory

