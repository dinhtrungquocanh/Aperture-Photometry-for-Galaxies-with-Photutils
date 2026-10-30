# Aperture-Photometry-for-Galaxies-with-Photutils
This is the code for my aperture photometry pipeline using Photutils (Bradley et al., 2016). This pipeline was adopted for my research project as well as my bachelor thesis. 

Galaxies can have diverse shapes (compact, elongated, or irregular). Therefore, it would be more accurate to adopt an aperture that can adapt diverse galaxy morphologies, rather than apply a fixed circular aperture for every galaxy in the sample. By using Kron elliptical aperture, we can derive robust photometry data that match the standard catalog's results. 

<img width="601" height="374" alt="kron-aper" src="https://github.com/user-attachments/assets/0783e3da-6615-4cd9-bc05-1223df8081b4" />

The following flowchart describes the key steps of the flowchart which are the Background estimation and Image segmentation (Step 1); Kron aperture calculation (Step 2); Aperture correction (Step 3); Total flux and error calculation (Step 4). 

<img width="946" height="441" alt="aper-phot-flowchart" src="https://github.com/user-attachments/assets/f2b5dacd-4461-4b47-a6ea-e56840fdd619" />

The main notebook (Main_Aper_Photometry.ipynb) is used to calculate photometry for individual galaxies in a studied sample. 

For aperture correction (Step 3), we need to construct empirical psf and extract the radial profile. Run these two first:
- Construct_empirical_PSF.ipynb
- Radial_Profile_PSF.ipynb

Alternatively, we can also conduct aperture correction using simulated psf. The SPSF extraction is also covered in:
- Simulated_PSF.ipynb
  
Further documentation from Photutils can be found at: https://photutils.readthedocs.io/en/latest/user_guide/index.html

Data for this project is obtained from Dawn JWST Archive (DJA): https://dawn-cph.github.io/dja/imaging/v7/?search=gds-grizli-v7.2-f

