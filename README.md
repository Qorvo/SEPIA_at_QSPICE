# SEPIA @ QSPICE

***

Table of Contents
* *about* [SEPIA](#sepia)
* *about* [QSPICE](#QSPICE)
* *about* [PyQSPICE](#PyQSPICE)
* *about* [SEPIA@QSPICE](#SEPIAQSPICE)
* [Basic Operation](basic-operation)
* [Usage / Example](#usage--example)
* [Sub-Circuit Parameters](#sub-circuit-parameters)
* [Usage from PyQSPICE](#usage-from-pyqspice)

***


## SEPIA

**SEPIA**:  **S**tability **E**valuation for **P**ower **I**ntegrity **A**nalysis

The [SEPIA] is a control loop stability analysis tool developed by [Mr. Steve Sandler](https://www.signalintegrityjournal.com/authors/20-steve-sandler) at [Picotest.com](https://picotest.com).

The SEPIA extracts **frequency-domain parameters** of our target circuit/loop, **directly from time-domain, transient (.TRAN)** simulations.

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

## PyQSPICE

The [PyQSPICE](https://github.com/Qorvo/PyQSPICE) is a [Python](https://www.python.org/) wrapper-module for the QSPICE, available from this [Qorvo repository](https://github.com/Qorvo/) on [GitHub](https://github.com/).
By using the QSPICE as a strong back-end simulator, it supports complex data processing and data plotting.

## SEPIA@QSPICE

The QSPICE supports **user-defined C++ and/or Verilog** circuit blocks.  The SEPIA processing routines are implemented as one of such user-defined circuit blocks, that is the **DLL binary** available here.

> [!IMPORTANT]
> This SEPIA@QSPICE module is a **SUB-SET of the SEPIA**, where **NOT ALL the SEPIA PROCESUREs** implemented.

***

## Basic Operation

At a high-level, the SEPIA@QSPICE circuit module operates in following steps.

1. As a transient simulation goes, it detects ringing peaks and record them in its internal memory.
2. At the end of the transient simulation, it extracts the control loop parameters based on the SEPIA routines.  
  2a. It extracts basic loop information:  **Q** and frequency  
  2b. It model-fits and generates simplified RLC circuit model(s) representing the target loop, if options specified.
3. When specified by options, it further runs extra/follow-up simulations to RLC models.

## Usage / Example

The basic usage of the SEPIA@QSPICE and examples are summarized in this [session file](README.ipynb) by utilizing the [Jupyter Lab](https://jupyter.org/) environment.

> [!IMPORTANT]
> So to run the Python code recorded in the session file, please install below 2 software packages.
> * [QSPICE](https://qspice.com)
> * [PyQSPICE](https://github.com/Qorvo/PyQSPICE)

## Sub-Circuit Parameters

## Usage from PyQSPICE

