# X-ray Radio Luminosity Function (XRLF) for AGN

Actively accreting supermassive black holes (SMBH), also known as active galactic nuclei (AGNs), can produce radiation across the electromagnetic spectrum (e.g. P. Padovani et al. 2017, and references therein). The source of the emission in the AGN structure is distinct to each wavelength. The primary originator of X-ray emission in an AGN is the inverse Compton scattering of photons from the accretion disc, which takes place in a hot corona. For the brightest radio emitters, often referred to as the radio-loud population which are expected to only take up ∼10 per cent of the entire AGN population, the emission is primarily from synchrotron emission in large (up to megaparsec scales) powerful relativistic jets. Radio and X-ray emission are often good indicators of the presence of an AGN, even when the AGN is obscured at other wavelengths (see R. C. Hickox & D. M. Alexander 2018, and references therein). 

The detection of X-ray emission is a reliable indicator due to X-ray emission from other astrophysical processes (e.g. X-ray binaries) being typically weak in comparison, and only the most massive and highly star-forming (and rarer) galaxies being capable of producing X-ray emission where AGNs are expected to dominate. Therefore host galaxy contamination is only an issue for low luminosity AGNs and heavily obscured AGNs, where the X-ray emission is suppressed via absorption. Similarly, in the radio, whilst star-forming galaxies can be bright in radio, AGNs are easily distinguishable from star-formation at the highest radio luminosities.  

Measurements of the luminosity functions of AGNs in both the X-ray and radio bands provide a means of quantifying the intrinsic space density of sources across differing luminosities and over cosmic time, capturing the diversity of the AGN population. Luminosity functions (LFs), however, tend to only look at the space densities in a single waveband, and inclusion of other wavelengths would be as subsets of varying properties in the additional waveband. Before C.M. Pennock et al. (2025) an LF in more than one waveband, a multidimensional LF, had not been explored yet. Exploring a multidimensional LF would allow us to investigate how AGNs evolve in the X-ray and radio (other wavelengths can be used as well) concurrently, as well as to see if there are any links/correlations between the emission produced at different distances to the SMBH, corona/accretion disc (X-ray) and relativistic jets (radio), across cosmic time.

See paper, [C.M. Pennock et al. (2025)](https://ui.adsabs.harvard.edu/abs/2025MNRAS.544.1779P/abstract)   

## The XRLF - Quick plot
[XRLF_plot](https://github.com/cmpennock/XRLF/tree/main/XRLF_plot) contains all the measurements, and their corresponding upper and lower limits of the XRLF of AGN found across the Bootes and COSMOS regions across 8 redshift ranges, as shown in Figures 5 & A1 in C.M. Pennock et al. (2025). 

The Jupiter notebook, [XRLF.ipynb](https://github.com/cmpennock/XRLF/blob/main/XRLF_plot/XRLF.ipynb), will use these measurements to create a plot of the XRLF of your chosen redshift range (note, only uses the same redshifts as used in the paper), that you can then interact with. 

## Calculating the XRLF (still adding...)
'Pennock2025' contains the catalogues used in C.M. Pennock et al. (2025) and the code is provided in the Jupiter notebook that will allow you to plot all the plots found in the paper, including the code that was used to measure the XRLF of AGN across Bootes and COSMOS.

