### @diffs true

# Servo Motors with Microbit & Grove
```template
basic.showIcon(IconNames.Yes)
```
## {Introduction @unplugged}
Let's create movement using @boardname@ , Grove and Servo Motors!
![WTS Logo](https://raw.githubusercontent.com/CarlTS/microbit-grove/master/assets/WTSLogo.png)

  - :lightbulb: Look out for hints indicated by a light bulb
Click the ``||game: OK ➔ ||`` or ``| ➔ Next |`` button on the right after each step to continue.

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

## Coding Time 
► From the ``||input:Input||`` category in your toolbox, find the ``||input:on button [A] pressed||`` and add it to your workspace.  
💡 This will be the trigger for our servo motor. We will worry about this later!

```blocks
// @highlight
input.onButtonPressed(Button.A, function () {
	
})
```

## differentblocks
different
```diffblocks
let x = 1
----------
let x = 1
let y = 1
```

## Testing Hint
Words that are not hidden
~hint This content is hidden until the user clicks here.
  - :lightbulb: Bullet 1
  - :mouse pointer: Bullet 2
hint~

```blocks
// @highlight
input.onButtonPressed(Button.A, function () {
	
})
```


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