# subsidence-arcgis-experience
Files for subsidence project version on ArcGIS experience

Author: Pilartes-Congo
Email: jcongo@islander.tamucc.edu / japcongo@hotmail.co.uk
Created: October 08, 2019.
******************************************************************************************************************************************************************************************

Data availability/sources/links
	- CBI cGPS Data: provided by Jason Louis (Conrad Blucher Institute, December 2019)

	- CORS Data: https://beta.ngs.noaa.gov/corsmap/#layers
		More information on NOAA CORS: https://www.ngs.noaa.gov/CORS_Map/

	- Tide Gauges Data: https://tidesandcurrents.noaa.gov/map/index.shtml?region=Texas (through lighthouse: http://lighthouse.tamucc.edu/)
		NGS NCAT Tool used to convert between SPCS and lat/lon: https://beta.ngs.noaa.gov/NCAT/
		It appears that Eastings and Northings are more accurate than the lat/lon 
		So NCAT was used to make the conversion instead of using the provided values
		PTMS used lat/lon because SPCS coordinates were too far off

	- UNAVCO Stations Data: https://www.unavco.org/data/gps-gnss/data-access-methods/dai2/app/dai2.html#Grouping=COCONet;scope=Station;sampleRate=normal;GroupingMod=contains;GroupingMod=contains
		UNAVCO includes: COCONet, GulfNet, HoustonNet, TLALOCNet

	- TxDOT RRPs Data: http://ftp.dot.state.tx.us/pub/txdot-info/isd/gps/Documents/TxDOT_RTN_RRP_Coordinates_rev_03-17-2019.pdf
		Additional information: https://www.txdot.gov/inside-txdot/division/information-technology/gps.html or http://ftp.dot.state.tx.us/pub/txdot-info/isd/gps/Documents/

	- Some of these features are hosted feature layers saved on ArcGIS Online. Errors might occur if the right permissions are not given to the client/viewer. Right now, they are set to only 
		the owner, and the Subsidence Project team. Permissions need to be updated as needed 

	- Data conversion software (from csv to GeoJSON): https://www.convertcsv.com/csv-to-geojson.htm
		This tool was used to convert UNAVCO stations data into GeoJSON. There might exist other 
		tools that can be used for the same purpose. One can also use the JSON beautify tools 
		found online to make the code look consistent.	

	- Geojson beautifier: https://codebeautify.org/jsonviewer
	- Converter to Geojson>SHP>CSV: https://mapshaper.org/
	- Legend icons: https://icons8.com/icons/pack/free-icons

******************************************************************************************************************************************************************************************

Page information:
	This project has been developed using ArcGIS API and Mapbox API as well as ArcGIS online capabilities. These functionalities were combined into ArcGIS Experience Builder for display.
	Page 1 > Homepage: 
		- uses only Experience Builder and its widgets
	Page 2 > Stations and Tide Gauges:
		- uses Mapbox API with information of the various stations and tide gauges as provided earlier in this document
		- code was written using html, without external links to other JavaScript or CSS or even html links
		- code embedded copied into an Experience Builder embedded page
	Page 3 > Heatmaps:
		- same procedure as Page 2
	Page 4 > Feature Query:
		- same procedure as Page 2; except it used ArcGIS API and not Mapbox API
		- features are not internally referenced like in Pages 2 and 3, they were loaded onto ESRI Online as hosted layers
		- features were merged into a single "ALL_LAYERS" file, that includes a count attribute column for each of them (i.e. CORS count vs CBI cGPS count, etc)
		- icons were manually changed to avoid having the same symbology, and keep consistency with previous pages
	Page 5 > Features of Interest:
		- features used are online as hosted layers
		- does not use any API; instead, uses ArcGIS Online capabilities
		- meant to include additional features such as Corpus Christi Sea Wall, and others as needed
	Page 6 > About Us:
		- information about the institute
		- does not use any API; made using ArcGIS Online

******************************************************************************************************************************************************************************************

YouTube instructions link: https://youtu.be/f_ETn4gHbnM