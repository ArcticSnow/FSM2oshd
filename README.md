# FSMOSHD

FSMOSHD is a variant of the Flexible Snow Model developed by [Essery (2015)](#Essery2015) with new components added for 
forest processes, snow cover fraction computations etc. The model is used for snow-hydrological predictions in Switzerland
within the [operational snow-hydrological service](https://www.slf.ch/en/snow/snow-as-a-water-resource/snow-hydrological-forecasting.html) maintained at SLF.

## Building and running the model

The main computation routines of FSMOSHD are located in the src/core folder. For demonstration purposes, the model
can be run for a point simulation using input data stored in a text file (see data directory). The code for handling model setup and input/output operations related to the text file driving option is found in the src/txt folder.

To compile the model for windows, use the [gfortran](https://gcc.gnu.org/wiki/GFortran) compiler and execute the compile script in the root folder:

`./compil.bat`

Run the executable with the command:

`./FSMOSHD.exe nlst_fsmoshd.nam`

## References

<a name="Essery2015"></a> Essery (2015). A Factorial Snowpack Model (FSM 1.0). *Geoscientific Model Development*, **8**, 3867-3876, [doi:10.5194/gmd-8-3867-2015](http://www.geosci-model-dev.net/8/3867/2015/)
