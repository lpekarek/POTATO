# POTATO
Practical Optical Tweezers Analysis TOol

*************** README - POTATO ***************
To analyze the great amount of data generated by this technique, we developed an automated python pipeline. This tool, POTATO (Practical Optical Tweezers Analysis TOol), allows marking the unfolding steps with pre-defined key parameters automatically. To open the data analysis to a broader audience, we wrapped the whole pipeline in a user-friendly graphical interface. All the analysis parameters can be easily changed without the need for a bioinformatics background. 

Developed by Lukáš Pekárek and Stefan Buck at the Helmholtz Institute for RNA-based Infection Research
    In the research group REMI - Recoding Mechanisms in Infections
    Supervisor - Jun. Prof. Neva Caliskan """
""" This script processes Force-Distance Optical Tweezers data in an automated way, to find unfolding events """
""" The script is developed to handle h5 raw data, produced from the C-Trap OT machine from Lumicks,
    as well as any other FD data prepared in a csv file (2 columns: Force(pN) - Distance(um)) """
""" The parameters can be changed in the GUI before each run.
    Alternatively they can be changed permanently in this script under 'default values for each data type' at line 264"""
""" The python file "Subprocess" has to be kept in the same directory as it is used

***Dependencies***


***Navigation***

POTATO is structured in three tabs: "Folder Analysis", "Show Single File" and "Advanced Settings"


***Input***

POTATO supports three different datasets for folder analysis.
The appropriate dataset has to be selected prior to the analysis.
ATTENTION: When changing between datasets, all parameters are reset to the default values!
ATTENTION: If there are too many files in the dictionary, you might run out of memory.

1) High frequency (Piezo Distance):
      Analyses the high frequency data out of all Lumicks h5 files in a given directory.
      The data gathering frequency is derived directly out of the h5 files.
2) Low Frequency
      Analyses the low frequency data out of all Lumicks h5 files in a given directory.
      The data gathering frequency is calculated directly out of the h5 files.
3) CSV (F/D)
      Analyses all csv files in a given directory.
      The architecture of these files need to consist out of two columns (Force and Distance) without headers.
      The data gathering frequency and all other parameters are derived out of the GUI.


***Parameters***

Parameters can be changed directly in the Graphical User Interface (GUI).
Upon changing, each parameter needs to be validated with the ENTER key.


***Output***
