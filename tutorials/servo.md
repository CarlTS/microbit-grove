# Servo Motors with Microbit & Grove
```template
basic.forever(function () {
	
})
```


## Introduction
### Introduction step @unplugged
<!---  @unplugged Deprecated use @showdialog --->

Making movement with a servo motor


# Countdown

## {Introduction @unplugged}

Let's create movement using @boardname@ , Grove and Servo Motors!

![WTS Logo](https://raw.githubusercontent.com/CarlTS/microbit-grove/master/assets/WTSLogo.png)

## {Setting up the loop}

We'll begin by testing our microbit

► In the bottom left of the screen select  ``|Download|``  
► You should now see a ✓ on your microbit  
💡 [Need help connecting?](https://www.youtube.com/watch?v=qSjMDG84bMY)

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

