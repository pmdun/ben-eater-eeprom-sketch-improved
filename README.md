## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/pmdun/ben-eater-eeprom-sketch-improved/edit/master/README.md)

This is a update I made to ben-eater sketch that enable you to program up to 16k using a nano.
this sketch saves the rom image to the nanos 32k internal memory

first you do a hexdump using the example below then copy the content to the arduino sketch and then you past it in to the line:

const byte Rom[] PROGMEM = {(hexdump contents of nameOfRom txt)please past here!};

then compile and upload sketch

good example of 0xff, format dump for ben eater eeprom programmer using hexdump that works!

hexdump -v -e '/1 "0x"' -e '/1 "%02x, "'  nameOfRom.hex > nameOfRom.txt

P M Dunne.
