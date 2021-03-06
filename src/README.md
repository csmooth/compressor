# Warm Compress - an L77 Compressor built with Java

## About
This file explains how to use Compressor and DeCompressor.  These programs implement a basic L77
compressor which appends unique characters using 8 bits following a '0' bit and repeated characters
or strings using a '1' bit followed by 12 bit pointers and 4 bit lengths, allowing phrases 2^4 long
and 2^12 away.

## Instructions
To use the compressor, open up a shell and cd into the directory "compressor\src" containing Compressor.jar .
In your terminal, run Compressor.jar by providing TWO arguments: "Input.file" and "Output.file"

For example:
```SUPERSHELL>> .\Compressor.jar .\Input.file .\Output.file```

Your "Output.file" does not need to actually exist when you first run the program.  This simply tells
the Compressor where to store the resulting output data.

DeCompressor works exactly the same, except your "Input.file" should now point to the previously
compressed information, or another file compressed by Compressor.

Example:
```SUPERSHELL>> .\DeCompressor.jar .\Input.file .\Output.file```
