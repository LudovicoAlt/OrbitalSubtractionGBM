

[![DOI](https://zenodo.org/badge/736409431.svg)](https://doi.org/10.5281/zenodo.17831670)



Tested for Windows 11 and Ubuntu 22.04<br>
Python 3.11.7 (in case `conda create -n "myenv" python=3.11.7`)<br>
Requires:<br>
matplotlib (tested 3.8.2)<br>
astropy (tested 6.0.0)<br>
numpy (tested 1.25.2)<br>
argparse (tested 1.25.2) (included in Python standard lib) <br>
configobj (tested 5.0.8)<br>
wxPython (tested 4.2.1)<br>

To quickly install all the pakcages, run within the project directory :

`python -m pip install -r requirements.txt`

wxPython in particular requires gtk3 so install that if it gives you errors :

`sudo apt-get install libgtk-3-dev` (Linux)

Within the directory run :

`python osv.py`

To run the GUI. <br>

If you want to run osv.py from any location (Linux) :

Create an alias of the command
`alias osv="python /<dir_of_osv>/osv.py"`<br>
Update bash or restart the terminal 
`source ~/.bash_profile`<br>
You should be able to run osv in any directory
`osv`<br>

In general the possible commands are :

`python osv.py doconfig`

This lets you set a default directory and some other default values, so you don't have to input the everytime (for example the data directory)

`python osv.py getdata`

This is mainly used in the download script, but you can use it manually to download specific data 

`python osv.py checkdeps` 

Checks your dependencies

`python osv.py checkvers`

Checks the package versions of the modules above you have installed (good to verify reproducibility)

`python osv.py getconfig`

Prints out the current config file (not elegant at the moment) but it allows you to double check configurations without having to rerun "doconfig"

`python osv.py ver` 

Check osv.py version 

If you use my updated code, kindly it cite as

```bibtex
@misc{DeSantis_OSV,
  author       = {De Santis, Alessio Ludovico},
  title        = {{OSV}},
  publisher    = {Zenodo},
  year         = {2024},
  doi          = {10.5281/zenodo.17831670},
  url          = {https://doi.org/10.5281/zenodo.17831670}
}
```

Also acknowledge the original developers of the python2 version of the code
```bibtex
@ARTICLE{2011arXiv1111.3779F,
       author = {{Fitzpatrick}, Gerard and {Connaughton}, Valerie and {McBreen}, Sheila and {Tierney}, Dave},
        title = "{Uncovering low-level Fermi/GBM emission using orbital background subtraction}",
      journal = {arXiv e-prints},
     keywords = {Astrophysics - High Energy Astrophysical Phenomena, Astrophysics - Instrumentation and Methods for Astrophysics},
         year = 2011,
        month = nov,
          eid = {arXiv:1111.3779},
        pages = {arXiv:1111.3779},
          doi = {10.48550/arXiv.1111.3779},
archivePrefix = {arXiv},
       eprint = {1111.3779},
 primaryClass = {astro-ph.HE},
       adsurl = {https://ui.adsabs.harvard.edu/abs/2011arXiv1111.3779F},
      adsnote = {Provided by the SAO/NASA Astrophysics Data System}
}
```

