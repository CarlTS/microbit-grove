# Servo Motors with Microbit & Grove
```template
basic.showIcon(IconNames.Yes)
```

## {Introduction @unplugged}
Let's create movement using @boardname@ , Grove and Servo Motors!
![WTS Logo](https://raw.githubusercontent.com/CarlTS/microbit-grove/master/assets/WTSLogo.png)

## {Testing the micro:bit}
We'll begin by testing our microbit

► Plug in your microbit   
► In the bottom left of the screen select  ``|Download|``  
► You should now see a ✓ on your microbit  -  💡 [Need help connecting?](https://www.youtube.com/watch?v=qSjMDG84bMY)
►   
►   
nospaceafter
►
►

```blocks
basic.showIcon(IconNames.Yes)
```

## Collecting Parts @fullscreen

Lets Connect all the parts, you will need
![GroveShield,Servo,Microbit,Cable](https://raw.githubusercontent.com/CarlTS/grove-sensor-tutorial/master/images/GroveSensors/ServoMotor.png)

## Connecting Everything @unplugged
Connect the parts together.
![Servo to Grove in P0/P14, microbit into the Grove Shield](https://raw.githubusercontent.com/CarlTS/grove-sensor-tutorial/master/images/GroveServoAssembled.png)


## Coding Time @unplugged @fullscreen
► From the ``||input:Input||`` category in your toolbox, find the ``||input:on button [A] pressed||`` and add it to your workspace.  
💡 This will be the trigger for our servo motor. We will worry about this later!

```blocks
// @highlight
input.onButtonPressed(Button.A, function () {
	
})
```


```validation.global
# BlocksExistValidator
```