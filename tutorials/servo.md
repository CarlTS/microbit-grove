### @diffs true

# Servo Motors with Microbit & Grove
```template
basic.showIcon(IconNames.Yes)
```
## {Introduction @unplugged}
Let's create movement using @boardname@ , Grove and Servo Motors!
![WTS Logo](https://raw.githubusercontent.com/CarlTS/microbit-grove/master/assets/WTSLogo.png)
**Helpful Hints**
  - :lightbulb: Look out for hints indicated by a light bulb   
You can click the ``||game: OK ➔ ||`` or ``| ➔ Next |`` button on the right after each step to continue.

## Testing the micro:bit @unplugged
We want to make sure everything is working correctly before we start.
![Plugging in microbit](https://raw.githubusercontent.com/CarlTS/microbit-grove/master/assets/microbitplugin.gif)   

## {Testing the micro:bit}
We'll begin by testing our microbit   
► Plug in your microbit   
► In the bottom left of the screen select  ``|Download|``  
► You should now see a ✓ on your microbit  -  💡 [Need help connecting?](https://www.youtube.com/watch?v=qSjMDG84bMY)

```blocks
basic.showIcon(IconNames.Yes)
```

## Collecting Parts @unplugged @fullscreen
Lets collect all the parts needed for this tutorial
![GroveShield,Servo,Microbit,Cable](https://raw.githubusercontent.com/CarlTS/grove-sensor-tutorial/master/images/GroveSensors/ServoMotor.png)

## Connecting Everything @unplugged
Connect the parts together.
![Servo to Grove in P0/P14, microbit into the Grove Shield](https://raw.githubusercontent.com/CarlTS/grove-sensor-tutorial/master/images/GroveServoAssembled.png)

## Time to Code @unplugged
In the next step, you will need to use ``||input:on button [A] pressed||``
```blocks
input.onButtonPressed(Button.A, function () {
	
})
```
```validation.local
# BlocksExistValidator
* Enabled: false
```

## Coding Time 
► From the ``||input:Input||`` category in your toolbox, find the ``||input:on button [A] pressed||`` and add it to your workspace.  
💡 This will be the trigger for our servo motor. We will worry about this later!
```blocks
// @highlight
input.onButtonPressed(Button.A, function () {
	
})
```

## differentblocks
► Now place a ``||pins: Servo Write Pin [P0] to [180]||`` inside the ``||input:on button [A] pressed||``   
💡 This will be tell the servo motor where to move to
```blocks
input.onButtonPressed(Button.A, function () {
    // @highlight
    pins.servoWritePin(AnalogPin.P0, 180)
})
```

## Download to micro:bit
► Time to test the movement   
► ``|Download|`` your code to the micro:bit and press the [A] button on the microbit


## Testing Single Movement @unplugged
You should have seen you micro:bit move!  
💡 If it is not moving, it might already be at position 180 **or** you might need a battery pack


## Test different numbers
► Try changing the value of 180, and test again   
💡 Don't forget to ``|Download|``  
```blocks
Only numbers between 0 and 180 will work.
You may need a battery pack if it is not moving at all
```

## More Control
► Let us get more control with another ``||input:on button [A] pressed||`` on the workspace   
► You will need to change the [A] pressed to [B] pressed
```blocks
input.onButtonPressed(Button.A, function () {
    // @highlight
    pins.servoWritePin(AnalogPin.P0, 180)
})
input.onButtonPressed(Button.B, function () {

})
```

## More Control - Second Location
► Place another ``||pins: Servo Write Pin [P0] to [180]||`` inside the ``||input:on button [B] pressed||``   
► Set [180] to [90]
```blocks
input.onButtonPressed(Button.A, function () {
    pins.servoWritePin(AnalogPin.P0, 180)
})
input.onButtonPressed(Button.B, function () {
    // @highlight
    pins.servoWritePin(AnalogPin.P0, 90)
})
```

## Download to micro:bit
► Time to test the movement   
► ``|Download|`` your code to the micro:bit 
► Press the [A] button on the microbit and it should go to position 180
► Pressing [B] should go to position 90
 
##Coding: Setup the first position
------------------
Place a ``||pins:servo write pin||`` block inside a ``||input:On Button A Pressed||``
Set the number "180" to "0"
```blocks
// @highlight
input.onButtonPressed(Button.A, function () {
    pins.servoWritePin(AnalogPin.P0, 20)
})
```




```validation.global
# BlocksExistValidator
```