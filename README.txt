Decombinator: a tool for fast, efficient gene assignment in T cell receptor
sequences using a finite state machine

Niclas Thomas, James Heather, Wilfred Ndifon, John Shawe-Taylor, Benny Chain.

*****************************************************************************
PLEASE SEE www.ucl.ac.uk/innate2adaptive/software FOR AN EXECUTABLE VERSION
OF DECOMBINATOR, WITH NO NEED TO DOWNLOAD AND INSTALL ALL DEPENDENCIES LISTED
BELOW.
*****************************************************************************

Introduction
############

Decombinator is a tool for the fast, efficient analysis of T cell receptor (TcR)
repertoire samples, designed to be accessible to those with no previous
programming experience. It is based on the Aho-Corasick algorithm which
uses a finite state automaton (FSA) to quickly assign a specific V and J
gene segment. From these assignments, it is then able to determine the number
of germline V and J deletions and the string of contiguous nucleotides which
lie between the 3' end of the V gene segment and the 5' end of the J gene
segment. These 5 variables form the identier which uniquely categorises each
distinct TcR sequence. For more details, please see (Thomas et al.).
Decombinator assumes no prior programming experience.

############
Decombinator has been tested on Python v2.6 and v2.7.
Decombinator requires the following Python modules:-

NumPy
Biopython
matplotlib
acora
Levenshtein

NumPy, BioPython and matplotlib install in a very straightforward manner - just follow the instructions,
accepting all defaults. To install acora, you will need GCC or something akin to it for your platform.
For Linux users, installation of GCC should be straightforward. For Windows users, something like MinGW
is needed - I recommend installing the GCC Win32 binaries from this website http://www.develer.com/oss/GccWinBinaries,
which is very straightforward to install - again, follow the instructions provided there. Installation on
a Mac should be possible with Xcode, though I haven't tested this yet. Installation of the Levenshtein
package will probably require Python setuptools to be downloaded and installed.

For anyone requiring further guidance for installation of any of the above packages, please see
www.ucl.ac.uk/innate2adaptive/software for a comprehensive set of instructions on installation and usage.

Once these modules have been successfully installed, Decombinator can be run
using Python from the command prompt (assuming Python has already been added
to your PATH using: -

cd location/of/decombinator-master/folder/on/your/system
python decombinator-v1.1.py

It is then simply a case of following the instructions given on screen.

Please email niclas.thomas@gmail.com to report bugs/for help in installtion or usage.