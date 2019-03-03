# 4xiDraw

The 4xiDraw Extensions for Inkscape - Software to drive the 4xiDraw drawing machine.

More about 4xiDraw:  https://www.instructables.com/id/4xiDraw/

Now I have added support for HC-06 Bluetooth module for Wireless plotting.

---------


Install as you would any other Inkscape extension.

I use the following GRBL setup:

```
$100=100.000
$101=100.000
$110=5000.000
$111=5000.000
$120=1000.000
$121=1000.000
$130=200.000
$131=200.000
$132=200.000
$N0=M3S90
```


---------
Dependencies:

1. [plotink](https://github.com/evil-mad/plotink) helper routines for Inkscape extensions.
2. eggbot_hatch.py from the [EggBot extensions for Inkscape](https://github.com/evil-mad/EggBot/).
3. [Pyserial](https://pypi.python.org/pypi/pyserial). (Note that an older version, 2.7, must be used on Windows.)


---------

Known issues:

- There is apparently a rounding error somewhere, so the start and end of a drawing does not always line up.
- The speed is lower than it should be.

---------

This is based on the AxiDraw inkscape plugin, https://github.com/evil-mad/AxiDraw/
