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

```blocks
basic.showIcon(IconNames.Yes)
```

## Collecting Parts @unplugged

Lets Connect all the parts, you will need
![GroveShield,Servo,Microbit,Cable](https://raw.githubusercontent.com/CarlTS/grove-sensor-tutorial/master/images/GroveSensors/ServoMotor.png)

## Connecting Everything @unplugged
Connect the parts together.
![Servo to Grove in P0/P14, microbit into the Grove Shield](https://raw.githubusercontent.com/CarlTS/grove-sensor-tutorial/master/images/GroveServoAssembled.png)


## Coding Time
► From the ``||input:Input||`` category in your toolbox, find the ``||input:on button [A] pressed||`` and add it to your workspace.  
💡 This will be the trigger for our servo motor. We will worry about this later!

```blocks
// @highlight
input.onButtonPressed(Button.A, function () {
	
})
```


## Step 1 - Collect Parts @unplugged
How far away?
=============
In this activity you will learn how to make a servo motor move

Collect the parts you will need;
![Parts Needed: 1 Servo Motor, 1 microbit, 1 sheild](https://raw.githubusercontent.com/CarlTS/grove-sensor-tutorial/master/images/GroveSensors/ServoMotor.png)

## Step 2 - Connect Wires
Physical Connection
-------------------
1. Plug the microbit into the Shield 
2. Plug the 180 Degree Servo Motor into the P0 pin
![Connection Image](https://raw.githubusercontent.com/CarlTS/grove-sensor-tutorial/master/images/GroveServoAssembled.png)

## Step 3 - Program
Coding: Setup the first position
------------------
Place a ``||pins:servo write pin||`` block inside a ``||input:On Button A Pressed||``
Set the number "180" to "0"
```blocks
input.onButtonPressed(Button.A, function () {
    pins.servoWritePin(AnalogPin.P0, 20)
})
```


## Step 4 - Program
Coding: Setup the Second position
------------------
Place another ``||pins:servo write pin||`` block inside another ``||input:On Button A Pressed||``
Change the Button A to Button B Pressed
Set the number to "180"
```blocks
input.onButtonPressed(Button.B, function () {
    pins.servoWritePin(AnalogPin.P0, 180)
})
input.onButtonPressed(Button.A, function () {
    pins.servoWritePin(AnalogPin.P0, 0)
})
```


## Step 5 - Test in the simulator
Testing: Does the simulator microbit and servo move
------------------
In the simulator on the left, press the Button A and Button B on the microbit
Does the servo on the screen move?


## Step 7 - Download Program
Download & Test
--------------------
Click ``|Download|`` to transfer your code
If it doesn't move correctly try reducing the range the servo is moving, so instead of 0 to 180, try 20 to 160. 
