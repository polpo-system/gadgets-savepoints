# gadgets-savepoints

SavePoints for [polpo](https://github.com/polpo-system/polpo): a fader of the screen saver SaveScreen (the
package savescreen): figures made of points, read from SavePoints.Data.

```
portia.Install gadgets-savepoints
```

## Using

    SavePoints.Install          Points becomes the current fader

## What is here

    src/SavePoints.Mod
    share/SavePoints.Data       the figures
    share/SavePoints.Text       its notes (MakePoints, which made the data, is not here)
    test/SavePointsTest.Mod

SavePoints is by Jaco Geldenhuys; it draws with Display3 of the gadgets. The source comes from ETH Linux Oberon (OLR, 2017-06-18), converted from an Oberon text to plain
text; the first commit has it unchanged. It compiles unchanged with all five of polpo's compilers
(x86, ARM, ARMv7, RISC-V, MIPS).

## Tests

    SavePointsTest.Run      1 check: the module loaded; it needs the desktop's display

The license is GPL-3 (`LICENSE`); the code comes from ETH Oberon, whose license (`LICENSE.ETH`)
asks to keep its copyright notice and conditions, which `LICENSE.ETH` does.
