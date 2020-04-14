# subsidence-arcgis-experience
Files for subsidence project version on ArcGIS experience

Author: Pilartes-Congo
Email: jcongo@islander.tamucc.edu
Created: October 08, 2019.


Data downloadble from:
	CBI cGPS Data: provided by Jason Louis (Conrad Blucher Institute, December 2019)
	CORS Data: https://beta.ngs.noaa.gov/corsmap/#layers
	Tide Gauges Data: http://gulfsubsidence.org/
	UNAVCO Stations Data: https://www.unavco.org/data/gps-gnss/data-access-methods/dai2/app/dai2.html#Grouping=COCONet;scope=Station;sampleRate=normal;GroupingMod=contains;GroupingMod=contains
		UNAVCO includes: COCONet, GulfNet, HoustonNet, TLALOCNet
		TxDOT RRPs was also retrieved from UNAVCO related sources. However, not directly from their website.


	More information on NOAA CORS: https://www.ngs.noaa.gov/CORS_Map/



Data conversion software (from csv to GeoJSON): https://www.convertcsv.com/csv-to-geojson.htm
	This tool was used to convert UNAVCO stations data into GeoJSON. There might exist other 
	tools that can be used for the same purpose. One can also use the JSON beautify tools 
	found online to make the code look consistent.	