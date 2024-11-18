# CoCo Sprite Compiler (CoCoSC)

![image](https://github.com/user-attachments/assets/b2968d00-96ca-45a1-844b-8dbb48e6225a)

***
## What does CoCoSC do?

Quite simply, CoCoSC is a sprite compiler, targeting the Motorola MC6809 CPU - in particular the TRS-80 Color Computer 3. It gives you the ability to add amazingly fast graphics to your application. 

## What doesn't CoCoSC do?

The primary purpose of CoCoSC is to output compiled sprites, for direct use in your assembly code applications. CoCoSC is NOT a graphics editor. While there are some basic tools built into the application for manipulating imported graphics, CoCoSC is not a drawing utility. Why? I wanted to focus efforts on getting graphics into the Color Computer, rather than re-invent the graphics-editor wheel. There are countless other, freely available utilities for drawing and editing graphics - GIMP is a personal favorite of mine. However, once you have designed your artwork in a separate utility, CoCoSC makes it extremely easy to get those graphics into your Color Computer 3.

## What are the limitations of CoCoSC?

Currently, CoCoSC only supports 4bpp (16-color) graphics - therefore its only target system is the Color Computer 3.

## Is there any documentation on how to use CoCoSC?

At the moment, there is no written documentation, however the basic use of the tool was covered in an episode of 'The CoCoTECH! Show' a little while back. The episode may be found here - https://www.youtube.com/watch?v=IJbG_HDidaE

## How do I get started? The Compile and Test buttons are greyed-out.

To take full advantage of CoCoSC's capabilities, you must pair it with William Astle's LWASM utility (http://www.lwtools.ca/) and the 'Color Computer 3' VCC emulator (https://github.com/VCCE/VCC). The LWASM utility is used as a cross-assembler to assemble the graphics source code into .BIN files. The VCC emulator is then used to directly test those .BIN files.

Once you have installed these two tools, go to the Settings menu of the CoCoSC utility to set the paths to these two applications. After setting the paths, you simply drag/drop either a .PNG or .BMP image into the application. It's also possible to copy/paste clipboard graphic data, or use the File Open/Close method.

Another setting that is recommended is the path to your external editor (under Utilities). This will allow you to directly export generated code into your editor, including 'full sprite code' which shows what the Test code is running.

## Does CoCoSC do anything else besides compiled sprites?

Yes it does. It has a feature to output full-page graphics. While compiled sprites are nice because of how incredibly fast they render, they have a tendency to consume large amounts of RAM. I wanted the ability to preview large graphic objects (many cases full-screen splash pages), and compiled sprites don't work well in these scenarios. Instead, I'm using Ciaran Anscomb's DZIP utility/code to compress the full-screen graphics to load/view on the Color Computer 3. There are some basic tools to crop and resize images, to better fit the CoCo 3 graphic resolutions.

## CoCoSC is a Windows application - will you release a Mac or *nix version in the future?

The short answer - probably not. The longer answer, I'm not a developer (at least not in a true definition sense). I have the ability to hack and cobble together apps/tools/utilities for my specific needs and have never gotten into the practice of cross-platform support. 

## How can I help support the project?

I'm always looking for feedback and suggestions. Please touch base with me on any bugs you might find, or if you have thoughts on how to improve the utility. Also, documentation is currently non-existent for the application. This started off as a simple program with basic functionality, but quite a lot has been added over the last couple of years. If you would like to help in documenting the application, I'd certainly welcome the support.
