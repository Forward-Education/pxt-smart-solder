# pxt-learn-to-solder

Smart Solder Kit, by Forward Education

Find us at [forwardedu.com](https://forwardedu.com/) and [learn.forwardedu.com](https://learn.forwardedu.com/).

## Example Usage

Our learning systems are designed to simplify teaching coding and computer science for educators at all experience levels.
Our Smart Solder Kit can be used on its own or joined with other kits to access our wider library of sensors, motors, lights, and buttons.
Check out our lesson catalogue for curriculum-aligned lessons, including educator notes.
A sample of coding with the Smart Solder Kit can be seen below.

The green, yellow, and red lights simulate a traffic stop and the speed of the light change can be changed with the buttons.

```blocks
buttons.BTN2.onEvent(jacdac.ButtonEvent.Down, function () {
    delay = 3000
})
buttons.BTN1.onEvent(jacdac.ButtonEvent.Down, function () {
    delay = 1000
})
buttons.BTN3.onEvent(jacdac.ButtonEvent.Down, function () {
    delay = 5000
})
let delay = 0
delay = 3000
basic.forever(function () {
    lights.YELLOW.setBrightness(0)
    lights.RED.setBrightness(100)
    basic.pause(delay)
    lights.RED.setBrightness(0)
    lights.GREEN.setBrightness(100)
    basic.pause(delay)
    lights.GREEN.setBrightness(0)
    lights.YELLOW.setBrightness(100)
    basic.pause(delay)
})
```

## Supported Targets

-   for PXT/microbit

## License

MIT
