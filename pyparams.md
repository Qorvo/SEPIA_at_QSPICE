# PyQSPICE: SEPIA@QSPICE Option Control

The PyQSPICE provides a function **opt4SEPIA()** to manipulate the option string, as in the 2nd simulation above with this line.

````
run2.opt4SEPIA(run2.path['tran.cir'], Verbose = True)
````

***

This is the full arguments of the **opt4SEPIA()** method.  
***
***
***\_file_name_***:  the schematic name to manipulate.  This must be the first argument.
***
***
**prnPeak = True** or **prnPeak = False**:  
Print peak info,  
**False** is the default when not specified.

**Verbose = True** or **Verobse = False**:  
Verbose output,  
**False** is the default when not specified.

**log = True** or **log = False**:  
Logging output,  
**False** is the default when not specified.

**runTran0 = True** or **runTran0 = False**:  
Automatic simulation on the **model-0 transient** model,  
**False** is the default when not specified.  
Because of no way to know an auto-generated filename from the PyQSPICE, you must specify the **fnTran0** parameter together with this option.

**runTran1 = True** or **runTran1 = False**:  
Automatic simulation on the **model-1 transient** model,  
**False** is the default when not specified.  
Because of no way to know an auto-generated filename from the PyQSPICE, you must specify the **fnTran1** parameter together with this option.

**runAC0 = True** or **runAC0 = False**:  
Automatic simulation on the **model-0 AC** model,  
**False** is the default when not specified.  
Because of no way to know an auto-generated filename from the PyQSPICE, you must specify the **fnAC0** parameter together with this option.

**runAC1 = True** or **runAC1 = False**:  
Automatic simulation on the **model-0 AC** model,  
**False** is the default when not specified.  
Because of no way to know an auto-generated filename from the PyQSPICE, you must specify the **fnAC1** parameter together with this option.

***
***
**fnLog = \_file_name_**:  
Generate logging output file into a file named ***\_file_name_***

**fnTran0 = \_file_name_**:  
Generate **model-0** of transient model into a file named ***\_file_name_***

**fnTran1 = \_file_name_**:  
Generate **model-1** of transient model into a file named ***\_file_name_***

**fnAC0 = \_file_name_**:  
Generate **model-0** of AC model into a file named ***\_file_name_***

**fnAC0 = \_file_name_**:  
Generate **model-1** of AC model into a file named ***\_file_name_***

