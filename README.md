This repository contains radial velocity datasets that have been published in peer-reviewed literature.

**Note**: Check the data carefully before using it for scientific work. If you notice any issues with one of the datasets, please do a pull request on this repository or [file an issue](https://github.com/j-faria/rvdb/issues).


The repository is structured as a collection of plain-text files. 
Each star has an associated file with extension .sys (system); 
this file contains a few stellar parameters and references to the radial velocity files associated with the star.

Each star can be associated with multiple radial velocity files with extension .vels (velocities). 
The header of .vels files contains information about the telescope and instrument used to gather the data, 
and a reference to the paper where the RVs were published. 
After this header, each .vels file contains the data in at least three whitespace-separated columns: 
time of observation in JD, RV measurement in m/s and uncertainty on the RV measurement in m/s, e.g.:

```
# telescope = 9.2M HOBBY EBERLY TELESCOPE (HET)
# instrument = HRS
# observatory = MCDONALD OBSERVATORY, TEXAS
# reference = WITTENMYER ET AL. 2009 (APJS, 182, 97)
# bibcode = 2009APJS..182...97W
# source = http://exoplanetarchive.ipac.caltech.edu//data/ExoData/0071/0071395/data/UID_0071395_RVC_003.tbl
  2453462.96527            -137.0                           4.1
  2453479.81567            -147.0                           4.4
  2453480.91902            -136.9                           5.7
  ...
```

The meaning of any other additional columns is also specified in the .vels file.


## Where does the data come from?
The initial release of the database, created by Stefano Meschiari on 01/30/15, contained data originally hosted on the [NASA Exoplanet Archive](http://exoplanetarchive.ipac.caltech.edu), cleaned up and with duplicate datasets removed. Any data added after that date was pulled from published peer-reviewed papers.



Based on: [stefano-meschiari/rvdb](https://github.com/stefano-meschiari/rvdb)
