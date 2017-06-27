# msConverter Instructions

### Export data from mass spec software (i.e. Xcalibur) to a .raw file format
* right click spectra of interest then click: export > Write to RAW file
* save file with appropriate syntax
### [Convert .raw -> .mzXML](https://bix-lab.ucsd.edu/display/Public/Data+Conversion+to+.mzXML)
* open MSConvert
* click Browse and select file for conversion
* choose an output directory
* under options, choose output file format (.mzXML), 32-bit for binary encoding precision and uncheck Use zlib compression
* Under filters, choose Peak Picking with Vendor checked, in order to centroid the data. Indicate MS-Levels 1-2
* click Add to add the filter
* click Start
* confirm that .mzXML is in correct output directory
