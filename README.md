# SEPIA @ QSPICE

***

Table of Contents
* *about* [SEPIA](#sepia)
* *about* [QSPICE](#QSPICE)
* *about* [PyQSPICE](#PyQSPICE)
* [Usage / Example](#usage-example)
* [Sub-Circuit Parameters](#sub-circuit-parameters)
* [Usage from PyQSPICE](#usage-from-pysqpice)

***


## SEPIA

**SEPIA**:  **S**tability **E**valuation for **P**ower **I**ntegrity **A**nalysis

The [SEPIA] is a control loop stability analysis tool developed by [Mr. Steve Sandler](https://www.signalintegrityjournal.com/authors/20-steve-sandler) at [Picotest.com](https://picotest.com).

The SEPIA method is based on a simple fact that every single circuit sharing the same qualify factor **Q** exhibits the mathematically **"similar"** ringing to decay shape by assuming it is a quadratic system.

## SEPIA Copyright Notice

***Copyright © 2014 Picotest***

***The "SEPIA" compiled binary, the DLL (Windows Dynamic Link Library) file, available from this repository is a copyright intellectual property of [Picotest.com](https://picotest.com).  All rights reserved.***

Please contact [info@picotest.com](mailto:info@picotest.com) for more information.

***

In this repository, by a courtesy of Mr. Steve Sandler, the SEPIA is implemented into the [QSPICE](#qspice).

## QSPICE™

The <img src="https://www.qorvo.com/design-hub/-/media/images/qorvopublic/sic-qspice/qspice-icon.png" width="20" height="20">
[QSPICE](https://qspice.com) is a variant of SPICE (**S**imulation **P**rogram with **I**ntegrated **C**ircuit **E**mphasis, i.e. analog circuit simulator) software offered by [Qorvo](https://qorvo.com), that is available at **no cost**.

The QSPICE supports a **user-defined C++ and/or Verilog** circuit block and the SEPIA processing routines are implemented, that is the **DLL binary** available here.

## PyQSPICE

The [PyQSPICE](https://github.com/Qorvo/PyQSPICE) is a Python wrapper-module for the QSPICE.  By using the QSPICE as a strong back-end simulator, it supports complex data processing and data plotting.

***

## Usage / Example

## Sub-Circuit Parameters

## Usage from PyQSPICE

