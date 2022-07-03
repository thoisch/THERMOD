# THERMOD
THERMOD consists of three programs (THERMOD8, THERMODSUBDUCT, and PREPARRAYS) and a user’s manual.  THERMOD8 performs numerical simulations of heat conduction and advection in 1d and 2d systems; 2d systems may involve faults of specified geometry and displacement velocity. THERMODSUBDUCTION performs 2d numerical simulations of subduction zones and includes features not included in THERMOD8 (mantle corner flow, corner flow truncation, and frictional heating). The programs are operated through graphical user interfaces to set up models, run models, and export the results. Previously run model setups may be easily modified. Each program is discussed separately in the user’s manual.
### System Requirements
The programs run under operating systems Windows XP to Windows 11, and may run under future versions. THERMOD8 and THERMODSUBDUCT both sequester 1 GB of memory, and PREPARRAYS sequesters 200 MB. 
### Installation
Run the installer to install the programs and user’s manual. 
### Code description
The programs are written in APL2000 v. 3.6 and are provided as locked runtime applications. Sources codes and active workspaces can be provided upon request. 
### Quick Start
The easiest way to get started is to build and run the examples described in the user’s manual in section II.12 *THERMOD8 tutorial*, and section III.2 *Example: Alaskan flat-slab subduction model* (from Petersen et al., 2021). The user’s manual provides step-by-step instructions.  Completed model files generated as described in these sections are available in the repository.  Models described in section II.12 were created in THERMOD8. The completed model files may be loaded into THERMOD8 where they may be rerun or modified then run to create new models.  The model described in section III.2 was created in THERMODSUBDUCT.  The model file for this simulation may be loaded into THERMODSUBDUCT where it may be rerun or modified then run to create new models.  Note that the initial arrays for the subduction model were created in PREPARRAYS. These arrays were exported from PREPARRAYS and loaded into THERMODSUBDUCT in preparation for running the model. If modifying a subduction model involves changes to the initial physical constant arrays, then it will be necessary to create new initial arrays using the PREPARRAYS program for upload into THERMODSUBDUCT. See user’s manual for further details. 

Three additional subduction models, not described in the user's manual, are provided in the repository. These are models of Laramide subduction along the western margin of North America. Two are high-resolution models (1 km node spacing) of the near-trench portion of the system and are designed to test the effect of frictional heating along the fault; one  incorporates a high value (0.1) for the frictional coefficient and the other is identical except for incorporating a frictional coefficient of zero.  The third model (2 km node spacing) extends 850 km from the trench and simulates conditions that existed from the trench to the far edge of the Colorado Plateau assuming a frictional coefficient of 0.1. Completed model files and associated PREPARRAYS files are available for these examples. 
### License agreement
The licensing agreement is displayed when running the installer.  Users are asked to agree to the terms of the license as a condition for proceeding with the installation.
### Developer and contact
The programs were written by Thomas Hoisch, Professor, School of Earth & Sustainability, at Northern Arizona University. 
### Acknowledgements
The development of THERMODSUBDUCT and PREPARRAYS were funded by NSF grant EAR-1929520. Testing of the program was carried out in conjunction with research conducted by Sarah E. Petersen on Alaskan flat-slab subduction (Petersen et al., 2021) and Samantha Winston-Seitz on Laramide flat-slab subduction.
### References Cited
Hoisch, T. D. (2005). Thermod7: A general two-dimensional numerical modeling program for heat conduction and advection, with special application to faults. Computers & Geosciences, 31(6), 698–703. https://doi.org/10.1016/j.cageo.2005.01.005

Petersen, S. E., Hoisch, T. D., & Porter, R. C. (2021). Assessing the role of
water in Alaskan flat-slab subduction. Geochemistry, Geophysics, Geosystems,
22, e2021GC009734. https://doi.org/10.1029/2021GC009734
