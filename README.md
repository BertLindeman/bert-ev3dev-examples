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
    * [blinkleds](https://github.com/BertLindeman/bert-ev3dev-examples/blob/master/blinkleds)
    * [setled](https://github.com/BertLindeman/bert-ev3dev-examples/blob/master/setled)
    * [showleds](https://github.com/BertLindeman/bert-ev3dev-examples/blob/master/showleds)
    * [showmotor](https://github.com/BertLindeman/bert-ev3dev-examples/blob/master/showmotor)
    * [showpower](https://github.com/BertLindeman/bert-ev3dev-examples/blob/master/showpower)
    * [showsensors](https://github.com/BertLindeman/bert-ev3dev-examples/blob/master/showsensors)
    * [showsound](https://github.com/BertLindeman/bert-ev3dev-examples/blob/master/showsound)
    * [testmotor](https://github.com/BertLindeman/bert-ev3dev-examples/blob/master/testmotor)

### Have your EV3 report it's IP-address by speach after boot
For this an update is needed to `/media/mmc_p1/ev3dev.rc.local`

Add the next lines to the bottom of `/media/mmc_p1/ev3dev.rc.local`

```
if [ -e /media/mmc_p1/tellIP ]; then
echo "Executing /media/mmc_p1/tellIP"
. /media/mmc_p1/tellIP
fi
```


and an extra script [`tellIP`](https://github.com/BertLindeman/bert-ev3dev-examples/blob/master/tellIP)
in the same directory

