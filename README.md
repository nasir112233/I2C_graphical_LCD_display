I2C_graphical_LCD_display
=========================

Arduino library for LCD displays using I2C protocol.

Forked from https://github.com/nickgammon/I2C_graphical_LCD_display

Enhanced by Bruce Ratoff, KO4XL@yahoo.com, https://github.com/bratoff

For details about the theory, wiring, schematic, etc. see:
http://www.gammon.com.au/forum/?id=10940

LCD display: KS0108
IO expander: MCP23017 (also supported is the SPI version of the chip: MCP23S17)

Library documentation also on the above web page.

The original library has been expanded to include open and filled circles, and
an additional interface has been added using two 74HC595 latched shift registers.

Other enhancements include:
- Significant speed improvement in WRITETHRU_CACHE mode
- Optimization of shape drawing algorithms
- Conditional compilations based on presence of I2C and/or SPI libraries to reduce code size
- Platform-specific optimizations for AVR, some ARM architectures and ESP8266

Versions 2.x and 3.x Enhanced by B.Ratoff
Version 2.x - Add circle drawing
Version 3.x - Add support for 74HC595 2-wire interface see code comments for circuit info
Version 4.x - Eliminate need to include I2C and SPI libraries when 74HC595 is used
