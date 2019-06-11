# RapidCFD-Tests
Test cases for RapidCFD

- cavity - basic icoFoam test. Prepared in reply to https://github.com/Atizar/RapidCFD-dev/issues/44?_pjax=%23js-repo-pjax-container

- coil-pisoFoam. Speed test for RapidCFD. Kindly prepared by and submitted by [Chengtun](https://www.cfd-online.com/Forums/members/chengtun.html) in response to the discussion found on [CFD-Online](https://www.cfd-online.com/Forums/openfoam-community-contributions/170410-discussion-thread-how-install-use-rapidcfd-3.html)  - see posts #54-57.

- damBreak-rapidCFD. Dam Break test was inspired by [this](https://www.cfd-online.com/Forums/openfoam-installation/178078-comparison-openfoam-i7-xeon-32-cores-xeon-phi-knights-landing-tesla-k20m.html) CFD-Online posting by [ma-tri-x](https://www.cfd-online.com/Forums/members/ma-tri-x.html). Nvidia-smi output and the log file for the run are included. Test was stopped at ~0.402 seconds. For more details, see the README in the damBreak-rapidCFD folder.

- sloshingTank3D.  Sloshing tank tutorial from OpenFOAM 2.3.x, with modified fvSchemes and fvSolution for adaptation to RapidCFD. Gridding (blockMesh) and setFields (e.g., in the Allrun script) needs to be done with OpenFOAM 2.3.x before running `interDyMFoam` with RapidCFD.

- pitzDaly. OpenFOAM tutorial for rhoPimpleFoam-LES. Use blockMesh from CPU based OpenFOAM, e.g., 2.3.x, to create the grid. Execute with rapidCFD's `rhoPimpleFoam`.

