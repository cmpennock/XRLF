# X-ray Radio Luminosity Function (XRLF) for AGN

Actively accreting supermassive black holes (SMBH), also known as active galactic nuclei (AGNs), can produce radiation across the electromagnetic spectrum (e.g. P. Padovani et al. 2017, and references therein). The source of the emission in the AGN structure is distinct to each wavelength. The primary originator of X-ray emission in an AGN is the inverse Compton scattering of photons from the accretion disc, which takes place in a hot corona. For the brightest radio emitters, often referred to as the radio-loud population which are expected to only take up ∼10 per cent of the entire AGN population, the emission is primarily from synchrotron emission in large (up to megaparsec scales) powerful relativistic jets. Radio and X-ray emission are often good indicators of the presence of an AGN, even when the AGN is obscured at other wavelengths (see R. C. Hickox & D. M. Alexander 2018, and references therein). 

The detection of X-ray emission is a reliable indicator due to X-ray emission from other astrophysical processes (e.g. X-ray binaries) being typically weak in comparison, and only the most massive and highly star-forming (and rarer) galaxies being capable of producing X-ray emission where AGNs are expected to dominate. Therefore host galaxy contamination is only an issue for low luminosity AGNs and heavily obscured AGNs, where the X-ray emission is suppressed via absorption. Similarly, in the radio, whilst star-forming galaxies can be bright in radio, AGNs are easily distinguishable from star-formation at the highest radio luminosities.  

Measurements of the luminosity functions of AGNs in both the X-ray and radio bands provide a means of quantifying the intrinsic space density of sources across differing luminosities and over cosmic time, capturing the diversity of the AGN population. Luminosity functions (LFs), however, tend to only look at the space densities in a single waveband, and inclusion of other wavelengths would be as subsets of varying properties in the additional waveband. Before C.M. Pennock et al. (2025) an LF in more than one waveband, a multidimensional LF, had not been explored yet. Exploring a multidimensional LF would allow us to investigate how AGNs evolve in the X-ray and radio (other wavelengths can be used as well) concurrently, as well as to see if there are any links/correlations between the emission produced at different distances to the SMBH, corona/accretion disc (X-ray) and relativistic jets (radio), across cosmic time.

See paper, [C.M. Pennock et al. (2025)](https://ui.adsabs.harvard.edu/abs/2025MNRAS.544.1779P/abstract)   

## The XRLF - Method
To estimate the luminosity functions for the individual X-ray and radio wavebands, we use the method described in M. J. Page & F. J. Carrera (2000), modified to account for changing sensitivity across survey area:

$$\phi_{\rm est, \lambda} = \frac{N_{\lambda}(l_{\lambda},z)}{\int_{z_{\rm min}}^{z_{\rm max}} \int_{l_{\rm \lambda, min}}^{l_{\rm \lambda, max}}A(f_{\lambda}(L_{\lambda},z)) \frac{dV}{dz}dz \ d\log(L_{\lambda})} $$

Where $N_\lambda$ is the total number of sources in a specified redshift and luminosity (X-ray or radio) range, $\lambda$ represents the wavelength at which the luminosity function is being measured (X-ray or radio) and $A$ is the survey area that is sensitive to a source with a specified flux (as defined by the sensitivity curves in the X-ray and the flux cuts in the radio), $f_\lambda$, corresponding to a given luminosity, $L_\lambda$, and redshift, $z$.
$\frac{dV}{dz}$ is the differential co-moving volume (with respect to $z$) per unit area. 
$l_{\rm \lambda,min},l_{\rm \lambda,max}$ (where $l_{\rm \lambda,min},l_{\rm \lambda,max}) \equiv (\log L_{\rm \lambda,min}, \log L_{\rm \lambda,max}$) and $z_{\rm min},z_{\rm max}$ indicate the limits of the luminosity and redshift bin over which the binned luminosity function is calculated.
1 $\sigma$ equivalent uncertainties on
$\phi_{\rm est, \lambda}$ are calculated based on the Poisson uncertainties in the observed
source number, $N_\lambda$, using the relations given by Gehrels (1986).

To estimate the X-ray--radio luminosity function we modify this equation, to calculate a single volume which allows for whether the radio or X-ray detection limits place the most stringent constraints on the survey area that we are sensitive to at a given $L_{\mathrm{X}}$ or $L_{\mathrm{R}}$ and $z$. By integrating over these joint limitations we are able to accurately assess the cosmological volume that we are probing with the combination of our X-ray and radio surveys for a given luminosity/redshift bin. 
Our binned estimator of the X-ray--radio luminosity function is thus given by:

$$ \phi_{\mathrm{XR}} = \frac{N_{\mathrm{XR}}(L_{\mathrm{X}},L_{\mathrm{R}}, z)}{\int_{z_{\rm min}}^{z_{\rm max}} \left[\int_{l_{\rm X, min}}^{l_{\rm X, max}} \int_{l_{\rm R, min}}^{l_{\rm R, max}} A_{\rm m} d\log(L_{\mathrm{X}}) d\log(L_{\mathrm{R}}) \right] \frac{dV}{dz}dz } $$


where $A_{\rm m} =min\Bigl(A\bigl(f_{\mathrm{X}}(L_{\mathrm{X}},z)\bigr), A\bigl(f_{\mathrm{R}}(L_{\mathrm{R}},z)\bigr) \Bigr)$ and $N_{\mathrm{XR}}$ is the total number of sources in a specified redshift, X-ray luminosity and radio luminosity range. 
While $\phi_{\rm est}$ has units of $\mathrm{Mpc}^{-3}$ $(\log L_\lambda)^{-1}$ i.e. per unit volume per logarithmic luminosity interval, $\phi_{\mathrm{XR}}$, which involves an integration over both the X-ray and radio luminosity interval, has units of $\mathrm{Mpc}^{-3}$ ($\log L_{\mathrm{X}})^{-1} (\log L_{\mathrm{R}})^{-1}$. We note that to compare directly to measurements of luminosity functions in a single band thus requires us to multiply by the size of the bin in the other wavelength. We thus define $\phi_{\mathrm{X}}(L_{\mathrm{X}} | L_{\mathrm{R}})$, the X-ray luminosity function for sources of a given radio luminosity as:

$$ \phi_{\mathrm{X}}(L_{\mathrm{X}} | L_{\mathrm{R}}) = \int_{l_{\rm R,min}}^{l_{\rm R,max}} \phi_{\mathrm{XR}}(L_{\mathrm{X}},L_{\mathrm{R}}) d \log (L_{\mathrm{R}}) $$

$$ \approx \phi_{\mathrm{XR}}(L_{\mathrm{X}},L_{\mathrm{R}}) \times \Delta \log L_{\mathrm{R}} $$

where $\Delta \log L_{\mathrm{R}} = l_{\rm R,max}-l_{\rm R,min}$ is the size of the logarithmic radio luminosity bin. 
The radio luminosity function of sources of a given X-ray luminosity, $\phi_{\mathrm{R}}(L_{\mathrm{R}} | L_{\mathrm{X}})$, is defined in an equivalent manner.

## The XRLF - Quick plot
[XRLF_plot](https://github.com/cmpennock/XRLF/tree/main/XRLF_plot) contains all the measurements, and their corresponding upper and lower limits, of the XRLF of AGN found across the Bootes and COSMOS regions across 8 redshift ranges, as shown in Figures 5 & A1 in [C.M. Pennock et al. (2025)](https://ui.adsabs.harvard.edu/abs/2025MNRAS.544.1779P/abstract). 

The Jupiter notebook, [XRLF.ipynb](https://github.com/cmpennock/XRLF/blob/main/XRLF_plot/XRLF.ipynb), will use these measurements to create a plot of the XRLF of your chosen redshift range (note, only uses the same redshifts as used in the paper), that you can then interact with. 

![RXLF_3D_example_v7.pdf](https://github.com/user-attachments/files/30710773/RXLF_3D_example_v7.pdf)

## The XRLF - Measuring and plotting
[XRLF_measure_and_plot](https://github.com/cmpennock/XRLF/tree/main/XRLF_measure_and_plot) contains the catalogue of X-ray and radio detected sources in the COSMOS and Bootes fields ([X-ray_Radio_Bootes_COSMOS_v5.csv](https://github.com/cmpennock/XRLF/blob/main/XRLF_measure_and_plot/X-ray_Radio_Bootes_COSMOS_v5.csv)), as well as the X-ray area curves for Bootes ([areacurve_bootes](https://github.com/cmpennock/XRLF/blob/main/XRLF_measure_and_plot/cdwfs_sens_broad.csv)) and COSMOS ([areacurve_cosmos](https://github.com/cmpennock/XRLF/blob/main/XRLF_measure_and_plot/areacurve_cosmosCass_HSCUVista.csv)), used in [C.M. Pennock et al. (2025)](https://ui.adsabs.harvard.edu/abs/2025MNRAS.544.1779P/abstract). Also, the code is provided in the Jupiter notebook, [XRLF_measure_and_plot.ipynb](https://github.com/cmpennock/XRLF/blob/main/XRLF_measure_and_plot/XRLF_measure_and_plot.ipynb), that will allow you to measure and plot the XRLF of AGN across Bootes and COSMOS over a redshift range of your choice and plots the results in an interactive 3D plot.






