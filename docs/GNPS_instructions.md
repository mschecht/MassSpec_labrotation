# Instructions for uploading data to [GNPS](http://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash.jsp)
For further details check [documentation](https://bix-lab.ucsd.edu/display/Public/Molecular+Networking+Documentation#MolecularNetworkingDocumentation-SubmitWorkflow)
1. Export data from Xcalibur (.raw)

	* right click spectra of interest then click: export > Write to RAW file

	* save file with appropriate syntax

2. [Convert .raw -> .mzXML](https://bix-lab.ucsd.edu/display/Public/Data+Conversion+to+.mzXML)

	a. open MSConvert

	b. click Browse and select file for conversion
	
	c. choose an output directory
	
	d. under options, choose output file format (.mzXML), 32-bit for binary encoding precision and uncheck Use zlib compression
	
	e. Under filters, choose Peak Picking with Vendor checked, in order to centroid the data. Indicate MS-Levels 1-2
	
	f. click Add to add the filter
	
	g. click Start
	
	h. confirm that .mzXML is in correct output directory
3. Go to [GNPS website](http://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash.jsp) and login.
```
username: MPI_MarineMicro
password: GNPS1811
email: massspec@mpi-bremen.de
```
4. Under "Create Public MassIVE Datasets" click Submit. This will take you to the [MassIVE website](http://massive.ucsd.edu/ProteoSAFe/static/massive.jsp?redirect=auth) where you can submit your data. You should now be on the [MassIVE website](http://massive.ucsd.edu/ProteoSAFe/static/massive.jsp?redirect=auth). Under "Create Public MassIVE Datasets" click Submit

6. Login with same credentials as [GNPS website](http://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash.jsp), then Under "create Public MassIVE Datasets" click Submit

7. Fill out Workflow page
* Workflow Selection:

	a. Title project starting with GNPS (i.e. "GNPS_title_of_project")

	b. Workflow: MassIVE Dataset Submission
* Dataset Metadata: Fill out ALL appropriate metadata
* Data File Selection: MUST include Raw Spectrum files, other submissions up to your own disgression
	
	a. click Raw Spectrum Files: Select Input Files

	b. make new directory under /MPI_MarineMicro

	c. connect to MassIVE server via FTP (Filezilla)

	d. click Quickconnect

	e. drag in .mzML files to appropriate directory

	f. back on MassIVE server select .mzML file you uploaded then press Raw Spectrum Files (this will move the upload .mzML file from Select Input Files to Selected files
	
	g. under Selected Files click Finish Selection

```
Host: ccms-ftp01.ucsd.edu
Username: MPI_MarineMicro
Password: GNPS1811
```

8. Click Submit
9. After job is complete go main page of [GNPS website](http://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash.jsp), click `jobs`, then click `back to main page`
10. Now you will submit your uploaded metabalome for social molecular networking
11. Workflow: Give it a title
12. Basic options: click `Select input files` to upload metabalomic dataset
13. provide an email and click `submit`
