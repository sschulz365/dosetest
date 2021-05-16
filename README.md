# dosetest
Dosetest file for electron beam lithography using Raith eline control software.


Description of the file clearingdose_publicv2.gds

This file contains a dose test, drift test and write field alignment test pattern and is designed for use with the Raith Eline control software.
How to use the file
Include a copy of the file in the position list for your E-beam exposure, placing it near the centre of your sample (or near your structures), making sure that is kept away sufficiently for the edges to have a similar resist thickness as near your structures and avoiding edge beads. Towards the beginning of your write expose layers 0,1. These contain the dose test squares (including the labels) and the WF test pattern, as well as half of the drift pattern. At a later point, e.g. towards the end of the write, expose a second copy of the structure, placed at the identical coordinates as the first one, this time only exposing layer 8. This layer contains the second half of the drift test pattern, Therefore any misalignment in the drift test pattern represents a drift in the coordinate system over the time between these two parts of your exposure, while any misalignment in the WF pattern is due to the WF alignment and does not depend on the drift. 
Within both the drift and WF test structures, one division corresponds to a 10nm shift. If the central lines match up, then there is no error, while each division further out corresponds to an additional 10nm WF error (or drift respectively). E.g. if the fourth line from the centre matches in the vertical section of the pattern and the second from the centre in the horizontal section, then the WF error was 40nm along the vertical axis and 20n along the horizontal axis. 

This file was original created by Liam O'Faolain (William Whelan-Curtin).
