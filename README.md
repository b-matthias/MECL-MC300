# MECL-MC300

#### Introduction

This the goal of this project is to enumerate each MECL circuit from the 1963 Motorola catalog in a SPICE circuit/sub-circuit file, and to provide sample circuits from application notes.
In 1962, Motorola introduced a new family of logic circuits called MECL. Motorola continued to introduce subsequent versions of the MECL family.
In later versions of Motorola manuals (e.g. MECL System Design Book, Forth Edition), Motorola uses five logic family names of MECL I, MECL II, MECL III, MECL 10K, and MECL 10KH

#### Series

Most of the MECL logic circuits are available as two different series, with part numbers which differ by "50" (e.g. MC303 and MC353 or MC311 and MC361).
The MC300 series is "military" operating temperature range -55 to +125 (degrees C)
The MC350 series is "industrial" operating temperature range 0 to +75 (degrees C)
There are some exceptions (see Packages), and some idiosyncrasies to the part numbering schemes. I will try to identify each of these situations in separate markdown files for each part number, as needed.

#### Packages

MECL is offered in 10-lead metal can (TO-5), and 10-lead flat package (TO-91).
The flat package is designated with an "F" suffix on the ordering part number, and "G" for the metal can.
Some exceptions is a 14-lead flat package (TO-86), also using the suffix "F" for ordering.
The MC313F is only available in the 14-lead flat package.
The MC363F is only available in the 14-lead flat package.
The MC369F is only available in the 14-lead flat package.
The MC369G is only available in the metal can package.

#### MECL circuits in SPICE

At the time of this document I am using a (partial) copy of the Motorola MECL Data Book, [Archive.org bitsavers collective](https://ia801902.us.archive.org/25/items/bitsavers_motoroladactronics02MECL_15757786/02_MECL.pdf)
The MECL family is detailed in section 2 of this book, and this PDF starts at section 2.

Also, Application Note IC-11 written by Emory Garth has good information about the implementation of MECL logic blocks. A copy can be found in Google Books, [American Microelectronics Data Annual 1964–65](https://books.google.com/books?id=tdCjBQAAQBAJ&lpg=PA250&ots=P0it3LPHe_&dq=emory%20garth%20motorola&pg=PA250#v=onepage&q=emory%20garth%20motorola&f=false)
Page 250

#### SPICE version

I am currently using MacSpice locally on my MacBook Pro, which I use to test each circuit and sub-circuit.
Nevertheless, I believe that this syntax should work for all SPICE 3

#### Personal Note

My first job after "higher education" was working on the UNIVAC 1100/90 at the Sperry manufacturing facility. As a matter of course, at that time, Unisys was being created with the merger of Sperry and Burroughs.
The UNIVAC 1100/90 and Unisys 2200/100 (and other versions if this system) employed ECL logic gates for the Central Processor Unit.
The CPU circuit boards (52 in total) used a complex set of many layers and large edge connectors on three sides to achieve a very high density of logic circuits; which Sperry terms High Performance Packaging (HPP).
This high-density logic required liquid cooling using a cold plate sandwiched between two PCBs placed face-to-face.
While the UNIVAC 1100/90 did not use MECL circuits or packages; the concept is similar, and the MECL family has much better documentation.
All of this to say: I have a fondness for ECL logic and systems built with ECL logic.
