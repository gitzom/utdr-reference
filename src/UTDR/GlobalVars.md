# Global Variables

## global.plot
In UT/DR global.plot is a `float` used to determine where in the plot the game is in, 0 being the start. 

### Example Usage

    if (global.plot < 12)
        global.plot = 12;

## global.flag
global.flag is an `array` used for pretty much anything that can happen. From decisions to storing specific values flags can be extremly diverse with their usage.


### Example Usage

    if (global.flag[23])
        global.flag[920]++