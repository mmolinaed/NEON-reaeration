NEON Reaeration Rate
================

<!-- README.md is generated from README.Rmd. Please edit that file -->
<!-- ****** Description ****** -->
Contains functions to format data and calculate reaeration rates of tracer gas and oxygen.

<!-- ****** Usage ****** -->
Usage
-----

The functions in this package have the following purpose: (1) to format downloaded data, (2) to calculate travel time, (3) to calculate reaeration rates, and (4) to normalize to Schmidt 600 number. See help files for individual functions for details. The general flow of using this package is:

1.  download data from the NEON data portal, into location "myDataPath", which is the path of the zip file and should end in .zip or set dataDir = "API" and identify a specific site or set site = "all" to pull in data for all NEON sites from the API.
2.  reaFormatted &lt;- def.format.reaeration(dataDir = "myDataPath"), returns a data frame called reaFormatted
3.  reaRatesCalc &lt;- def.calc.reaeration(inputFile = reaFormatted, dataDir = "myDataPath", plot = T), returns a list of two dataframes, the input dataframe of data for up to 4 stations per site per date and an output dataframe appended with loss rate, travel time, SF6 reaeration rate, O2 gas transfer velocity, and Schmidt number 600 for a given site and date.

<!-- ****** Acknowledgements ****** -->
Credits & Acknowledgements
--------------------------

<!-- HTML tags to produce image, resize, add hyperlink. -->
<!-- ONLY WORKS WITH HTML or GITHUB documents -->
<a href="http://www.neonscience.org/"> <img src="logo.png" width="300px" /> </a>

<!-- Acknowledgements text -->
The National Ecological Observatory Network is a project solely funded by the National Science Foundation and managed under cooperative agreement by Battelle. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the author(s) and do not necessarily reflect the views of the National Science Foundation.

<!-- ****** License ****** -->
License
-------

GNU AFFERO GENERAL PUBLIC LICENSE Version 3, 19 November 2007

<!-- ****** Disclaimer ****** -->
Disclaimer
----------

*Information and documents contained within this pachage are available as-is. Codes or documents, or their use, may not be supported or maintained under any program or service and may not be compatible with data currently available from the NEON Data Portal.*
