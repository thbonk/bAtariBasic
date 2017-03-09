# bAtariBASIC

A Basic Compiler for the Atari 2600<br/>
Copyright 2005-2007 by Fred Quimby

bAtariBASIC continuing development, with improved support for Unix / macOS.

## bAtariBASIC Reborn

The last release of **bAtari Basic** was version 1.0 in 2007, and it's getting pretty long-in-the-tooth, so I've decided to make a fork for needed improvements, hosting on GitHub to make the project more visible and help with collaboration. See `bB/README.txt` for the original credits and instructions. I'll add updated summaries to this README as the project progresses.

**[bAtari Basic 1.0](http://bataribasic.com/)** remains a free and open source product, under copyright, with a permissive open source license. It is not "public domain" or "abandonware" but merely a project that lost its steam around 2007 due to lack of interest. Since that time there's been a steadily growing interest in the consoles-of-yore due to emulation, USB Atari joysticks, speedy laptops, 2600-in-a-joystick products, re-issues of classic titles, and so on. An exciting ["homebrew" scene](http://www.atari2600homebrew.com/) is producing games that never made it to the 2600, improved versions of games whose originals fell short (e.g., Pac Man), and many [new and original titles](https://www.atariage.com/store/).

While it is true that we can now use `cc65` to write 2600 code directly in C, and it's been demonstrated that C++18 can be used to produce highly optimized 6502 code, *bAtariBASIC* still has some utility. 2600 programs are usually not very large or complex, and *bAtariBASIC* is great for rapid prototyping. Since I've already begun working to rectify that situation with my [6502-Tools](/thinkyhead/6502-Tools) project, it seems like an opportune time to revive *bAtariBASIC* (and provide other tools) to make it easier to develop 2600 games on macOS.

## Planned Changes

- Clean up and standardize source code formatting
- Use macros and inlines to reduce repetition
- Allow more complex expressions (if evaluatable at compile-time)
- Add shorthand operators: `--`, `++`, `+=`, `*=`, `/=`, `^=`, `|=`, `&=`, `%=`
- Add a single-binary build option with flags for preprocess, postprocess, optimize
- Support bAtariBASIC in Sublime Text and Atom on macOS
- Option to produce asm output for `ca65`?
- Option to produce C output suitable for `cc65`?
- Write some tools for making 2600 graphics in JavaScript+HTML5

## Stuff to Retain

- Keep the language small and simple
- Keep the Makefile-based build system
