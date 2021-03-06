# PDB-parser
### A PDB parser to correct errors, change characters and convert ATOM to HETATM
By Nicolas Pettican, for the Tabernero and Bella labs, University of Manchester.

<hr />

> :grey_exclamation: note that this requires Python 2.7

<hr />

#### Motivation:

The PDB format is kind of special in that every single white space is important. So forget about importing it into Python, modifying it, and outputting each column separated by a tab, it doesn't work.

I created this parser in order to modify characters that are repeated throughout the PDB file. Since there still isn't a straightforward way to e.g. add specific glycans to specific residues in a protein, you kind of have to play around with it. And that can create PDB files that have columns that need to be modified.

I also wanted a program that could convert certain ATOMs to HETATMs defined by the user, a function I recently added to PDBparser.

<hr />

#### Development:

At the moment I am working on increasing its functionality. I recently added the option "change ATOM to HETATM (v/v)" for when you have Ca2+ ions and glycans and want to convert them into HETATM so that Molecular Dynamics Simulation programs can identify these elements. Future options may include changing entire columns if e.g. the order of residues or atoms is wrong or broken and needs mending, or remove the second protein if you have a double protein PDB file.

<hr />

#### Usage:

To use, simply run ```python PDBparser.py``` on your Python environment, or open ```PDBparser.ipynb``` in a iPython or [jupyter notebook](http://jupyter.readthedocs.io/en/latest/install.html). You may want to edit DATADIR, DATAFILE and OUTFILE to your requirements before running.

<hr />

Feel free to fork it and collaborate! Let us contribute to the advancement of computational biology :computer: :microscope:

<br />
<br />
<center><a href="https://github.com/nickpettican/PDB-parse/blob/master/PDBparser.py"><img src="https://raw.githubusercontent.com/nickpettican/SparkzLab/master/img/code_white_small.gif" style="width: 40%; border-radius: 50%; height: auto;"></img></a></center>
