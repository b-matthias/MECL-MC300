# MECL-MC300

#### Project

The goal of this project is to enumerate each MECL circuit in a SPICE circuit/sub-circuit file. A secondary goal is to provide sample circuits from the application notes.

#### Introduction

This family of high speed logic integrated circuits was developed by Motorola in the 1960's. ECL stands for Emitter-Coupled Logic and the Motorola series was known as MECL.
In later versions of Motorola manuals (e.g. MECL System Design Book, Forth Edition), Motorola uses five names when refering to the MECL logic family.
There were 5 series of MECL IC's from Motorola: MECL I 1962-1977 30MHz switching and 8ns gate propagation delay; MECL II 1966-1979 70MHz switching and 4ns gate propagation delay (which increased to 180MHz and 2ns over the years); MECL III 1968-19?? 500MHz switching and 1ns gate propagation delay; MECL 10K (1971-) and MECL 10KH (1981-) were further improvements.

This project will focus on MECL I, a.k.a. the MC300/MC350 series circuits.

#### MECL MC300 Series

The family of the MECL logic circuits are available as two different series, with part numbers which differ by "50" (e.g. MC303 and MC353).  
The MC300 series is "extended" operating temperature range -55 to +125 (degrees C).  
The MC350 series is "commercial" operating temperature range 0 to +75 (degrees C).  
There are some idiosyncrasies to the part numbering schemes. I will try to identify each of these situations in individual markdown files for each part number, as needed.

#### Package Case Styles

MECL is offered in 10-lead metal can ("G" suffix), and 10-lead flat package ("F" suffix).   
One exception is a 14-lead flat package, also using the "F" suffix for ordering.   
Again, there are some idiosyncrasies to the part numbering schemes. I will try to identify each of these situations in individual markdown files for each part number, as needed.    
The 1966 Motorola Semiconductor Handbook (page 13-59) details the packages as: 10-pin metal (CASE 71), 12-pin metal (CASE 98), 10-pin flat package (CASE 72), and 12-pin flat package (CASE 83).    
Other manuals refer to the metal can package as TO-5, the 10-lead flat package as TO-91, and the 14-lead flat package as TO-86.

#### MECL circuits in SPICE

At the time of this document I am using a (partial) copy of the Motorola Integrated Circuit Data Book, [Archive.org bitsavers collective](https://ia801902.us.archive.org/25/items/bitsavers_motoroladactronics02MECL_15757786/02_MECL.pdf)   
The MECL family is detailed in section 2 of this book, and my PDF copy starts at section 2.   

Also, Application Note IC-11 written by Emory Garth has good information about the implementation of MECL logic blocks. A copy can be found in Google Books, [American Microelectronics Data Annual 1964–65](https://books.google.com/books?id=tdCjBQAAQBAJ&lpg=PA250&ots=P0it3LPHe_&dq=emory%20garth%20motorola&pg=PA250#v=onepage&q=emory%20garth%20motorola&f=false)
Page 250.

#### SPICE version

MY current choice for SPICE is MacSpice v?.? on my MacBook Pro, which I use to test each circuit and/or sub-circuit.
Nevertheless, I believe that this syntax should work for all SPICE based on Berkley SPICE.

#### Personal Note

My first job after "higher education" was working on the UNIVAC 1100/90 at the Sperry manufacturing facility. As a matter of course, at that time, Unisys was being created with the merger of Sperry and Burroughs.
The UNIVAC 1100/90 and Unisys 2200/100 (and other versions if this system) employed ECL logic gates for the Central Processor Unit.
The CPU circuit boards (52 in total) used a complex set of many layers and large edge connectors on three sides to achieve a very high density of logic circuits; which Sperry terms High Performance Packaging (HPP).
This high-density logic required liquid cooling using a cold plate sandwiched between two PCBs placed face-to-face.
While the UNIVAC 1100/90 did not use MECL circuits or packages; the concept is similar, and the MECL family has much better documentation.
All of this to say: I have a fondness for ECL logic, and complex logic systems based on ECL logic.
