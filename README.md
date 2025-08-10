# The following are Python scripts I wrote while interning at IIST. I explored detection and classification of Young Stellar Objects (YSOs) in HII Regions.

1) CCD_Region_File_Spitzer.ipynb
   -
   - Script that generates a color-color plot for a given csv file from archival data of the Spitzer Space Telescope's GLIMPSE mission.
   - The methodology adopted is in Gutermuth et al. (2009)
   - YSOs are classified into Class I/II/III, and the region files for overlaying on SAOds9 is also generated.
  
2) SED Fitting.ipynb
   -
   - Utilizes the modified blackbody function (graybody) to generate a pixel-by-pixel Spectral Energy Distribution via the technique of non-linear least-squares fitting.
   - For each pixel, the algorithm tries to find the best-fit dust temperature and column density values that give reduced chi-squared value closest to 1.
   - The values are written to FITS files to generate the dust temperature, hydrogen column density, and reduced chi-squared maps for the region of interest.

4) CutoutCode.ipynb
   -
   - A simple script where custom spatial dimension cutouts can be make to study smaller regions within larger FITS files. Especially useful for slower laptops/computers.
   - Creates only rectangular cutouts and also maintains WCS information.

5) Jybeam unit conversion.ipynb
   -
   - A useful python script that converts FITS files having "Jy/beam" as the unit of flux to "Jy/pixel" to accurately measure the total flux of sources.
   - Utilises information of the lenghts of the major and minor axes of the beam area, where beam refers to the telescope’s point spread function, usually a Gaussian with a specific major and minor axis size.
