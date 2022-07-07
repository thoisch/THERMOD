# THERMOD
THERMOD consists of three programs (THERMOD8, THERMODSUBDUCT, and PREPARRAYS) and a user’s manual.  THERMOD8 performs numerical simulations of heat conduction and advection in 1d and 2d systems; 2d systems may involve faults of specified geometry and displacement velocity. THERMODSUBDUCTION performs 2d numerical simulations of subduction zones and includes features not included in THERMOD8 (mantle corner flow, corner flow truncation, and frictional heating). The programs are operated through graphical user interfaces to set up models, run models, and export the results. Previously run model setups may be easily modified. Each program is discussed separately in the user’s manual.
### System Requirements
THERMOD runs under operating systems Windows XP to Windows 11, and may run under future versions. THERMOD8 and THERMODSUBDUCT both sequester 1 GB of memory, and PREPARRAYS sequesters 200 MB. 
### Installation
Run the installer to install the programs and user’s manual. 
### Code Description
The programs are written in APL2000 v. 3.6 and are provided as locked runtime applications. Sources codes and active workspaces can be provided upon request. 
### Quick Start: Tutorial and Model Examples
The best way to get started is to build and run the examples described in the user’s manual in section II.11 *THERMOD8 tutorial*, and section III.2 *Example: Alaskan flat-slab subduction model* (from Petersen et al., 2021). The user’s manual provides step-by-step instructions.  Completed model files generated as described in these sections are available in the repository.  The models described in section II.11 were created in THERMOD8 and may be rerun or modified to create new models.  The model described in section III.2 was created in THERMODSUBDUCT and may also be rerun or modified to create new models.  Note that the initial arrays for subduction models are created in PREPARRAYS.  Arrays exported from PREPARRAYS are loaded into THERMODSUBDUCT in preparation for running a model. If modifying a subduction model involves changes to the initial physical constant arrays, then it will be necessary to create new arrays using the PREPARRAYS program to be uploaded into THERMODSUBDUCT. See user’s manual for further details. 

Three additional subduction models, not described in the user's manual, are provided in the repository. These are models of Laramide subduction along the western margin of North America. Two are high-resolution models (1 km node spacing) of the near-trench portion of the system and are designed to test the effect of frictional heating along the fault; one  incorporates a high value (0.1) for the frictional coefficient and the other is identical except for incorporating a frictional coefficient of zero.  The third model (2 km node spacing) extends 1050 km from the trench and simulates conditions that existed from the trench to the far edge of the Colorado Plateau assuming a frictional coefficient of 0.1. Completed model files and associated PREPARRAYS files are provided for these examples. 
### License Agreement
The licensing agreement is displayed when running the installer.  Users are asked to agree to the terms of the license as a condition for proceeding with the installation.
### Developer and Contact
THERMOD was created by Thomas Hoisch, Professor, School of Earth & Sustainability, Northern Arizona University. 
### Acknowledgements
The development of THERMODSUBDUCT and PREPARRAYS were funded by NSF grant EAR-1929520. Testing of the program was carried out in conjunction with research conducted by Sarah E. Petersen on Alaskan flat-slab subduction (Petersen et al., 2021) and Samantha Winston-Seitz on Laramide flat-slab subduction.
### References Cited
Hoisch, T. D. (2005). Thermod7: A general two-dimensional numerical modeling program for heat conduction and advection, with special application to faults. Computers & Geosciences, 31(6), 698–703. https://doi.org/10.1016/j.cageo.2005.01.005

Petersen, S. E., Hoisch, T. D., & Porter, R. C. (2021). Assessing the role of water in Alaskan flat-slab subduction. Geochemistry, Geophysics, Geosystems, 22, e2021GC009734. https://doi.org/10.1029/2021GC009734
### Explanation of Uploaded Folders and Files
- Folder: THERMOD Installer. *Contains installer file*
- Folder: THERMOD License Agreement. *Contains pdf of license agreement*
- Folder: Model Examples. *Contains uploadable examples of models*
  - Folder: THERMOD8 models described in section II.11 of the user's manual
      - File: MANUAL1.sf. *THERMOD8 model file*
      - File: MANAUL2.sf. *THERMOD8 model file*
      - File: MANUAL3.sf. *THERMOD8 model file*
      - Folder: MANUAL4 model file and two example outputs
          - File: MANUAL4.sf. *THERMOD8 model file*
          - File: Manual4 ihp array 10my with fault.jpg. *Exported internal heat production array at 10 m.y. contoured with Surfer 7 using power law regression*
          - File: Manual4 T array 10my with fault.jpg. *Exported temperature array at 10 m.y. contoured with Surfer 7 using Kriging regression*  
  - Folder: Subduction Models
      - Folder: Alaskan flat-slab subduction. *This model was presented in Petersen et al. (2021) and is also described in section III.2 of the user's manual. See user’s manual for details on the calculation of the geotherms used to create the initial temperature array.  Node spacing for this model is 2 km.*
          - File: Cont 1d2km 35 km boundary.sf. *THERMOD8 model file. Continental geotherm model calculated to 150 km depth.*
          - File: Oceanic 1d2km 80 km depth.sf. *THERMOD8 model file. Oceanic geotherm model calculated to 80 km depth.*
          - File: Preparrays SE Alaska 2 km.sf. *PREPARRAYS file for Alaskan subduction model.*
          - Folder: Model file and graphed exported temperature array 
              - File: SE Alaska 2km.sf. *THERMODSUBDUCT model file.*
              - File: SE Alaska 2 km T array 20 my with fault.jpg. *Exported temperature array at 20 m.y. contoured with Surfer 7 using Kriging regression. White lines shows subduction fault and truncated mantle corner flow domain.*
      - Folder: Laramide subduction models
          - Folder: Near trench simulations. *Node spacing for the models is 1 km. 
              - File: Cont 1d1km 35 km boundary.sf. *THERMOD8 model file. Continental geotherm model calculated to 150 km depth. Same geotherm as for Alaskan model, except calculated for 1 km node spacing*
              - File: Oceanic geotherm 1 km 80 km depth.sf. *THERMOD8 model file. Oceanic geotherm model calculated to 80 km depth. Same geotherm as for Alaskan model, except calculated for 1 km node spacing*
              - File: Prepararrys file for hi res 8 degrees near trench.sf. *PREPARRAYS file for high resolution (node spacing of 1 km) near-trench models.*
              - Folder: Model with frictional coefficient of 0.1
                  - File: Laramide near trench fric .1 1 km.sf. *THERMODSUBDUCT model file. Frictional coefficient of 0.1 is assumed.*
                  - File: Laramide near trench fric .1 1 km 4  m.y. T array with fault.jpg. "Exported temperature array at 4 m.y. contoured with Surfer 7 using Kriging regression*
              - Folder: Model with frictional coefficient of zero
                  - File: Laramide near trench nofric 1 km.sf. *THERMODSUBDUCT model file. Frictional coefficient of zero is assumed.*
                  - File: Laramide near trench nofric 1 km 4 m.y. T array with fault.jpg. "Exported temperature array at 4 m.y. contoured with Surfer 7 using Kriging regression*    
          - Folder: Simulation that extends 1050 km from trench. *1d geotherms used to create the initial temperature array for this model are the same as for the Alaskan subduction model*   
               - File: Preparrays 2km Laramide model.sf.* PREPARRAYS file for model that extends 1050 km from the trench, node spacing of 2 km.*
               - Folder:  Model file and graphed exported temperature array 
                   - File: Laramide fric .1.sf. *THERMODSUBDUCT model file.* 
                   - File: Laramide fric .1  40 my T array with fault.jpg.  "Exported temperature array at 40 m.y. contoured with Surfer 7 using Kriging regression*    
                   
