# ch20edit for Vic-20 #

Vic-20 (unexpanded) character set editor

Hint: SPACE toggles pixel.  Menus are on screen.

Note: saves to FONT.BIN overwriting any existing file.   Manual load from BASIC is initially required to edit a font (after running/initializing program, and exiting).

``
LOAD "FONT.BIN",8,1
``

And wrote a [blog entry](https://techwithdave.davevw.com/2024/04/edit-vic-20-programmable-characters.html).

![prototype](media/functional.png)

Memory map - Unexpanded Vic-20

    0000-03FF lower RAM
    0400-0FFF (unpopulated)
    1000-17FF character RAM (was program RAM) ****
    1800-1DFF program RAM (reduced)
    1E00-1FFF video RAM
    2000-7FFF (unpopulated)
    8000-87FF character RAM set 1 (uppercase/graphics)
    8800-8FFF character RAM set 2 (lowercase/uppercase)
    9000-9FFF I/O and reserved
    A000-BFFF (unpopulated, or cartridge ROM)
    C000-DFFF BASIC ROM
    E000-FFFF KERNAL ROM

There is also a more fully featured [ch64edit](https://github.com/davervw/ch64edit) for Commodore 64
