# Aperture-Photometry-for-Galaxies-with-Photutils
This is the code for my aperture photometry pipeline using Photutils (Bradley et al., 2016). This pipeline was adopted for my research project as well as my bachelor thesis. 

Galaxies can have diverse shapes (compact, elongated, or irregular). Therefore, it would be more accurate to adopt an aperture that can adapt diverse galaxy morphologies, rather than apply a fixed circular aperture for every galaxy in the sample. By using Kron elliptical aperture, we can derive robust photometry data that match the standard catalog's results. 

The following flowchart describes the key steps of the flowchart which are the Background estimation (Step 1); Image segmentation (Step 2); Aperture correction (Step 3); Total flux and error calculation (Step 4). 

<img width="946" height="441" alt="aper-phot-flowchart" src="https://github.com/user-attachments/assets/f2b5dacd-4461-4b47-a6ea-e56840fdd619" />

Further documentation on photometry using Photutils can be found at: https://photutils.readthedocs.io/en/latest/user_guide/index.html

