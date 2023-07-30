# Servo Motors with Microbit & Grove
```template
basic.forever(function () {
	
})
```

## {Introduction @unplugged}

Let's create movement using @boardname@ , Grove and Servo Motors!

![WTS Logo](https://raw.githubusercontent.com/CarlTS/microbit-grove/master/assets/WTSLogo.png)

## {Testing the micro:bit}

We'll begin by testing our microbit

► In the bottom left of the screen select  ``|Download|``  
► You should now see a ✓ on your microbit      💡 [Need help connecting?](https://www.youtube.com/watch?v=qSjMDG84bMY)

```blocks
basic.showIcon(IconNames.Yes)
```


## {Setting up the loop}

We'll begin by using a [__*for loop*__](#forLoop "repeat code for a given number of times using an index") to recreate the same sound 3 times.

► From the ``||loops:Loops||`` category in your toolbox, find the ``||loops:for [index] from 0 to [4]||`` loop and add it to your ``||basic:on start||`` container.  
► Change your loop to count from ``0`` to **``2``**.  
💡 This means the loop will count 0-1-2 instead of what we want, which is 3-2-1. We will worry about this later!

```blocks
// @highlight
for (let index = 0; index <= 2; index++) {
	
}
```

## Activity 9 - Servo Motor
### Step 1 - Collect Parts @unplugged
How far away?
=============
In this activity you will learn how to make a servo motor move

Collect the parts you will need;
![Parts Needed: 1 Servo Motor, 1 microbit, 1 sheild](https://raw.githubusercontent.com/CarlTS/grove-sensor-tutorial/master/images/GroveSensors/ServoMotor.png)

### Step 2 - Connect Wires
Physical Connection
-------------------
1. Plug the microbit into the Shield 
2. Plug the 180 Degree Servo Motor into the P0 pin
![Connection Image](https://raw.githubusercontent.com/CarlTS/grove-sensor-tutorial/master/images/GroveServoAssembled.png)

### Step 3 - Program
Coding: Setup the first position
------------------
Place a ``||pins:servo write pin||`` block inside a ``||input:On Button A Pressed||``
Set the number "180" to "0"
```blocks
input.onButtonPressed(Button.A, function () {
    pins.servoWritePin(AnalogPin.P0, 20)
})
```


### Step 4 - Program
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


### Step 5 - Test in the simulator
Testing: Does the simulator microbit and servo move
------------------
In the simulator on the left, press the Button A and Button B on the microbit
Does the servo on the screen move?


### Step 7 - Download Program
Download & Test
--------------------
Click ``|Download|`` to transfer your code
If it doesn't move correctly try reducing the range the servo is moving, so instead of 0 to 180, try 20 to 160. 
