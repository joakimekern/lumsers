# lumsers
Collection of Lumerical scripts (.lsf) used to analyse nanoplasmonic slot waveguides.

This code is part of a Master's thesis in M.Sc. in Nanotechnology at NTNU. Joakim Ekern: "Development of a Nanoplasmonic Silicon Nitride Sensor Platform for Use in SERS" (2023). It is available to the public through "NTNU Open". In Chapter 4, extensive explanation of the use of Lumerical, the parameters used, and the calculated results are given.

The scripts are used to extract values necessary to calculate the conversion efficency of the waveguide. Details of the conversion efficiency is found in Dhakal et al.: "Efficiency of evanescent excitation and collection of spontaneous Raman scattering near high index contrast channel waveguides" (2015).

Through sweeps, the conversion efficiency is calculated at several geometries. A single parameter (1D) or two parameters (2D) may be sweeped at a time. The two scripts used to achieve this are given as "sers_1D_sweep.lsf" and "sers_2D_sweep.lsf". Note that the 1D sweeps allows for the inclusion of the Stokes shift, however, the 2D sweep is better documented, and the code is more simplistic.

In order for the scripts to work, the Lumerical MODE file must be setup properly. This involves defining several structures, parameters in the "model" object, and including the setup script "setup.lsf" in the "model" object. Details are found in Appendix B.
