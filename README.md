# IAUS391_JWST_Workshop
Material for the NIRSpec Hands-on workshop for researches based in Africa. 

 link for the workshop: https://www.youtube.com/watch?v=IMQCZ2M4CdI

## Proposal Planning 

### By Nimisha Kumari

Note from Nimisha: For the JWST Proposal planning tools session tomorrow, I am planning hands-on exercises for ETC and APT.
Online version of ETC is available here: https://jwst.etc.stsci.edu/
There is no installation needed for this, but the user needs an account to save the ETC workbooks. So, please get an account by clicking on “Create User” on the above page, and following the subsequent steps.
APT is essential for write the  JWST proposals. So for APT exercise, please install the software from here: https://www.stsci.edu/scientific-community/software/astronomers-proposal-tool-apt
Please follow the installation instructions according to your operating system: Linux, macOS, Windows.

### Q\&A Notes by Ken Duncan 

To add to my answer on the question about data products for e.g. planetary science/comets. On MAST High-level Science Products page: https://mast.stsci.edu/hlsp/#/ you can filter by astronomical object type. And in the main MAST archive you can search for data from any programme this is already public. So for example you could search by proposal ID for data from this programme: https://www.stsci.edu/jwst/science-execution/program-information?id=6714 to look at very recent cometary data. 

All of the various Solar System projects are listed on the Approved Projects for each JWST cycle: https://www.stsci.edu/jwst/science-execution/approved-programs/general-observers/cycle-2-go

Also, for the question on querying catalogues programmatically. MAST is accessible through the Astroquery interface: https://astroquery.readthedocs.io/en/latest/mast/mast.html
ESASky (including JWST) is also queryable through the same Python package: https://astroquery.readthedocs.io/en/latest/esasky/esasky.html  


## NIRSpec by Themiya Nanayakkara and Michael Maseda

To run the jwst notebooks (NIRSpec) you will first have to follow these steps

```
conda create --name nirspec_jdap python=3.11
conda activate nirspec_jdap
conda install ipykernel --name nirspec_jdap
python -m ipykernel install --user --name=nirspec_jdap
pip install ipython jupyter
pip install jwst
pip install msaexp pandas

cd LOCATION_OF_NOTEBOOKS

jupyter lab
```

You will have to set the CRDS server and path configurations. In the notebooks, we do this within the code itself, so check that out. 


## NIRCam by Ivo Labbe and Christina Williams

Note from Ivo: iau nircam workshop presentation and useful links
Updated based on hands-on presentation:
https://drive.google.com/file/d/148FH-CYjPT08cYwnrWpS-gu_RaUh31T7/view?usp=share_link
The link should open in google colab.

## SED fitting by Adam Carnall and Joel Leja

Note from Adam: For mine and Joel's session I've prepared some Google Colab notebooks (think Jupyter notebooks) that take you through the basic functions of my Bagpipes spectral fitting code. The link to access these is: https://drive.google.com/drive/folders/1eYntNnCeYDEbwG9fNK-L6LPfXsWExo9I?usp=sharing. You'll need to copy these into your own google drive in order to begin editing them.

Note from Joel: SED-fitting slides for those who'd like to follow along:
Prospector simple-start code and examples (see also Adam's BAGPIPES links, pinned above - all links are also in the presentation)
Quick start:
https://prospect.readthedocs.io/en/stable/quickstart.html
Demonstrations, examples of phot / spec fits:
https://prospect.readthedocs.io/en/stable/demo.html

Note from Ken: This is the Charlie Conroy Review that Adam was talking to people about: https://ui.adsabs.harvard.edu/abs/2013ARA%26A..51..393C/abstract


