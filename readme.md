# Constraining $\Omega_m$ with DESI and DES data

## Description
The idea of this project is to reproduce the results of Ruiz-Zapatero et al 2021 (https://arxiv.org/abs/2201.07025) with new data from DESI and DES.
In this project we want to use the Jeans equation for the linear growth of anisotropies to constrain $\Omega_m$:

$$
𝑓'+ 𝑓^2 + \left( 1 + \frac{d ln a H}{d ln a} \right) = \frac{3}{2} \Omega_m(z)
$$

This equation only depends on the LCDM model through H(z). Thus, we can obtain a model independent constraint on \Omega_m by modelling H(z) with a Gaussian Process.
In order to improve the constraining power, we fit the Gaussian Process simultaneously to H(z) and comoving distance data as well as $f\sigma_8$ data.

## New data
- DESI Full Shape: https://arxiv.org/pdf/2411.12021 (table 9)
- ACTxQuaia: https://arxiv.org/pdf/2507.08798 (Fig 12)
- DES Y5 supernova: https://github.com/des-science/DES-SN5YR/tree/main/4_DISTANCES_COVMAT

## To Do's
- [ ] Finish the auto-differentiable pipeline for comoving distances.
- [ ] Implement the pipelien for fsigma8.
- [ ] Connect the pipeline to the newest data.
- [ ] Potentially include the m-parameter but this would be quite involved.
