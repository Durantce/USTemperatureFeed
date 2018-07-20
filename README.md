# USTemperatureFeed

Run.py gets the most recent United States population weighted minimum, average, and maximum temperatures along with statewide minimum, average, and maximum temperatures using the NOAA api (https://www.ncdc.noaa.gov/cdo-web/webservices/v2).

Population data is read in by an excel file titled 'PopulationByFips.xlsx'.

Data is writen into another excel file titled 'FIPSTemperatureFeed5.0.xlsx'.

	State minimum cells are colored blue if they are below the national weighted minimum
		
	State maximum cells are colored orange if they are above the national weighted maximum
		
	State average text is colored orange if it is above one standard deviation from that days non-weighted average per state and blue if 			it is one standard deviation below or more
		
After the data is added into the excel spreadsheet, a plotly graph of temperature by state is displayed.

	Three files titled 'st99_d00.dbf', 'st99_d00.shp', and 'st99_doo.shx' are used for state borders during plotting
