# Numerical solution of the heat equation in 1D, 2D, 3D and data reader
## Context and presentation of the approach:

You will find here the [presentation (PDF)](https://raw.githubusercontent.com/carlmonnaert/Resolution-numerique/main/pr%C3%A9sentation.pdf) in french.

The list of objectives of this study and references to other studies can be found [here (PDF)](https://github.com/carlmonnaert/Resolution-numerique/blob/main/MCOT.pdf)


<img src="https://github.com/carlmonnaert/Resolution-numerique/blob/main/combo_blocs.png" alt="alt text" width="100%" height="whatever">
 
## Solution in simple cases:

The file `Résolution1D.py` displays the solution to the 1D heat equation in real time for a bar with thermal conductivity that can be modified at the beginning of the code.
This bar is subjected to a temperature imposed at the right end (temp_sol) and a conductive-convective flow on the left

The file `Résolution2D.py` displays the solution to the 2D heat equation in real time for a plane with thermal conductivity that can be modified at the beginning of the code.
This plane is subjected to a temperature imposed on the top (temp_sol).

The file `Résolution3Djoli.py` displays a 3D solution with the same boundary conditions as for the 2D solution.


## Resolution in special cases:

The following files solve the heat equation for a swimming pool subjected to conductive convection at its surface, with no heat flow on the sides of the pool and a customisable heat exchanger grid on the bottom of the pool and possibly on the sides.

The files `Résolution3Drp.py` and `Résolution3Dopti.py` enable the heat equation to be solved for an Olympic-sized swimming pool and can be adapted to any other system governed by thermal conduction.

It is necessary to create a folder with the same name as the extension variable, in which data will be saved by the execution of `Résolution3Drp.py` and `Résolution3Dopti.py`. This data can be accessed by the `reader_all.py` reader, in which the extension (folder name) to be viewed is entered.

As the execution of Resolution3Drp takes a long time (approximately 5 hours for the attached files), the attached folders contain the results for different geometries of the heated water/pool water exchanger.

This data can be viewed by executing `reader_all.py`.
