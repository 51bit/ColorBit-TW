#ColorBit driver

makecode pxt of ColorBit Tranditional Chinese version because of makecode bug: load zh folder for both zh-CN and zh-TW at present

once the makecode bug fix, this extension will merge into [ColorBit](https://github.com/51bit/ColorBit)

**ColorBit:**

![Alt text](icon.png?raw=true "ColorBit picture")

## Basic Usage

```blocks
let colorbit_51bit: colorbit.Strip = null
input.onButtonPressed(Button.A, function () {
    colorbit_51bit.showColorIcon(ColorIcon.ChristmasTree, colorbit.colors(BitColors.Red))
})
input.onButtonPressed(Button.AB, function () {
    colorbit_51bit.setMultiColor(false)
})
input.onButtonPressed(Button.B, function () {
    colorbit_51bit.showScrollStringColor("ABC#$123", colorbit.colors(BitColors.Red))
})
colorbit_51bit = colorbit.initColorBit(DigitalPin.P0, BitColorMode.RGB)
basic.forever(function () {

})
```

Use ``||initColorBit||`` to init ColorBit.

Use ``||showColorIcon||`` to show ColorBit icons.

Use ``||setMultiColor||`` to set multiple color per light.

Use ``||showScrollStringColor||`` to show scroll colorful string in ColorBit. 

![Alt text](GIF0.gif?raw=true "Basic Usage")
![Alt text](ku0.PNG?raw=true "showColorIcon")
![Alt text](ku.PNG?raw=true "showColorIcon")

## Gif demo

### Show single color string
![Alt text](GIF1.gif?raw=true "Demo 1")

### Show multiple color string
![Alt text](GIF2.gif?raw=true "Demo 2")

## Supported targets

* for PXT/microbit

## License

MIT
