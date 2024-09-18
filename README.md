# Alternative Logic Set (ALST)
ALST is a computer-aided non-binary logic research, design and simulation system (which can also simulate binary logic).
In essence, ALST is a CAD for all imaginable logic systems (binary, ternary, etc) which allows you to create your own basic components, create schemes utilizing those components, and then simulate their behavior with various types of stimuli.

ALST provides rich functionality to create and maintain a component library using user-created elements; analyze and simulate complete systems.
This CAD was used by me and some close colleagues of mine for the last 17 years to develop new system designs and architectures.
Nearly all of my hardware projects were prototyped in ALST first.

The system provides an intuitive workflow, where user can easily start a simulation, detect a bug, fix it, and continue the simulation from exactly the last saved point.
It's just as easy as setting a wire or removing an IC from a breadboard.

You can easily create interactive systems as well as purely batch-processing ones.

## System requirements

ALST works well on almost any machine: from old P1-90 with 32MB of RAM and Windows 95, all the way up to modern Windows 11 PCs.
It also works perfectly well in any \*nix system which has WINE: from FreeBSD to Ubuntu.
You can even run ALST in DosBox on your palm-top game machine using HX Dos Extender.
It's safe to say that if you can run vanilla DOOM on something, you can run ALST on the same thing :)

## Building from source

Please take a look at the `BUILD.md` file - it has step-by-step instructions on how to build ALST from this repository.

## How to use it?!

Unfortunately, I haven't updated the documentation since early 2008, which means it's a bit... stale. So I didn't bother to even include it in this repo.

The plan for now is to rewrite the documentation from scratch, accomodating for all changes in ALST over the last decade.
As usual, code comes first, docs come... later :) So no promises and/or concrete dates.

If you're willing to write documentation, please let me know via GitHub or email. Feel free to open a pull request as well.

## Some examples

### Simple oscillator and counters
![simple scheme](doc/img/simple.png)

### Small CPU
![small CPU](doc/img/small_cpu.jpg)

### Simple Neural Networks
![simple neural net](doc/img/neural_net.png)

### More complex Neural Networks (Hopfield network) with interactive UI
![Hopfield network](doc/img/hopfield.jpg)

### Another small PU (4-bit Turing Machine)
![4bit CPU](doc/img/4bit_cpu.jpg)

## TODO

**This document is still WIP. More updates will come soon.**


## Old project location
[old location at SourceForge](https://sourceforge.net/projects/alst)
