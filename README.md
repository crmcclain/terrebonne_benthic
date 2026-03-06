*Information on data collection*

Samples were collected using sediment cores from a shallow-water benthic community in Terrebonne Bay, Louisiana.
Environmental data (water temperature, salinity, dissolved oxygen, chlorophyll) was gathered from the Environmental Monitoring Program at the Louisiana Marine Consortium (LUMCON) for the years 2018-2023. Data was gathered from the Terrebonne Bay and LUMCON monitoring stations. 
Only macrofaunal invertebrates were analyzed for this data set.

#######################################################################################################################################################################################################################

Data Files in Package: 

TB2B_CoreData.csv: relevant sampling, environmental, and sediment core data for site TB2B
	Sample ID: unique identifier for each sediment core from site TB2B with the notation [Station(TB2B)-Sampling Code(Year.Month)-Core Number(#)] (example: TB2B-18.6-17)
	Station: the site of each collected sediment core (example: TB2B)
	Collection Date: the date each sediment core was collected with the notation [Day/Month/Year] (example: 6/14/18)
	Sampling Code: unique code for each sampling event of sediment cores with the notation [Year.Month] (example: 18.6)
	Sample Event: unique identifier for each sampling event of sediment cores with the notation [Year.Month.Number] (example: 18.06.1)
	Grab: Ponar grab number for each collected sediment core (example: 2)
	Core: Core number for each collected sediment core (example: 17)
	Year: the year each sediment core was collected (example: 2018)
	Month: the month each sediment core was collected (example: June)
	Season: the season each sediment core was collected using the northern hemisphere meteorological seasonal cycle [Winter (December, January, February), Spring (March, April, May), Summer (June, July, August), 	Fall (September, October, November)] (example: Summer)
	Months_Since_Hurricane: number of months since a hurricane event for each collected sediment core [any sediment cores taken before a hurricane event are labeled as "Pre"] (example: 1) 
	Latitude_DD: latitude for each sediment core in decimal degrees (example:  29.178333°)
	Longitude_DD: longitude for each sediment core in decimal degrees (example: -90.540500°)
	Latitude_DMS: latitude for each sediment core in degrees minutes seconds (29° 10.700' N)
	Longitude_DMS: longitude for each sediment core in degrees minutes seconds (example:  90° 32.430' W)
	Depth_m: depth in meters (m) for each sediment core (example: 3.1)
	max_temp_C: maximum water temperature in degrees Celsius (C) during the 30 days leading up to sediment core collection
	min_temp_C: minimum water temperature in degrees Celsius (C) during the 30 days leading up to sediment core collection
	mean_temp_C: average water temperature in degrees Celsius (C) during the 30 days leading up to sediment core collection
	max_temp_F: maximum water temperature in degrees Fahrenheit (F) during the 30 days leading up to sediment core collection
	min_temp_F:  minimum water temperature in degrees Fahrenheit (F) during the 30 days leading up to sediment core collection
	mean_temp_F: average water temperature in degrees Fahrenheit (F) during the 30 days leading up to sediment core collection
	max_salinity_ppt: maximum salinity in parts per thousand (ppt) during the 30 days leading up to sediment core collection
	min_salinity_ppt: minimum salinity in parts per thousand (ppt) during the 30 days leading up to sediment core collection
	mean_salinity_ppt: average salinity in parts per thousand (ppt) during the 30 days leading up to sediment core collection
	max_DO_mg/L: maximum dissolved oxygen in milligrams per liter (mg/L) during the 30 days leading up to sediment core collection
	min_DO_mg/L: minimum dissolved oxygen in milligrams per liter (mg/L) during the 30 days leading up to sediment core collection
	mean_DO_mg/L: average dissolved oxygen in milligrams per liter (mg/L) during the 30 days leading up to sediment core collection
	max_chlorophyll_ug/L: maximum chlorophyll in micrograms per liter (ug/L) during the 30 days leading up to sediment core collection
	min_chlorophyll_ug/L: minimum chlorophyll in micrograms per liter (ug/L) during the 30 days leading up to sediment core collection
	mean_chlorophyll_ug/L: average chlorophyll in micrograms per liter (ug/L) during the 30 days leading up to sediment core collection
	Water Loss: type of water loss (if any) during sediment core collection [None (no water loss), Water Drain (lost some or all top water during core collection), Spill (water lost during sieving)] (example: 	None) -CONTRIBUTES 0 OR 1 POINT TOWARDS CORE QUALITY-
	Mud Disturbance: type of mud disturbance (if any) during sediment core collection [None (no mud disturbance), Slant (core was taken at any angle other than 90°), Split (coring was obstructed due to hard 	object within coring area), Wonky (visible disturbance or irregularity at top of coring area)] (example: None) -CONTRIBUTES 0 OR 1 POINT TOWARDS CORE QUALITY-
	Mud Amount: amount of mud taken for each collected sediment core with the desired amount being 5 centimeters (cm) ["Perfect" = 5cm, "Scant" = 4.9cm, "Scantish" = 4.8cm] (example: 5cm) -CONTRIBUTES 0 TO 5 	POINTS TOWARDS CORE QUALITY-
	Mud Loss: amount of mud lost (if any) during sediment core collection or processing with the desired amount being 0 centimeters (cm) [1 "spoonful" = 0.5cm] (example: 0cm) -CONTRIBUTES 0 TO 2 POINTS TOWARDS 	CORE QUALITY-
	Preservation: preservation state of sediment core at time of processing [Preserved (successful preservation of core), Low EtOH (low amount of ethanol in core), Dried Out (no ethanol in core), Desiccated 	(core not preserved)] (example: Preserved) -CONTRIBUTES 0 OR 1 POINT TOWARDS CORE QUALITY-
	Core Quality: quality of sediment core using a 10 point scale [10 (perfect quality), 9 (high quality), 8 (moderate quality), 7 (low quality), ≤ 6 (core thrown out)] (example: 10) -CRITERIA 			OUTLINED ABOVE-
	Status: processing status for each sediment core [Completed (core processing is complete and data inputted in .csv file), Not Started (core processing not started), In Progress (core processing is 		occurring), Missing (core cannot be located), Discarded (core was thrown out)] (example: Completed)

TB2B_Taxa.csv: relevant taxonomic and ecological information for each species
	Species ID: species identifiers, can be matched to the sample x species matrix
	Group: general grouping of each species for naming purposes
	Phylum, Class, Order, Family, Genus, Species: taxonomic information for each species
	Synonymies: alternative names or "nicknames" for each species
	Body Size: calculated as the mean biovolume of each species in cubic millimeters (mm^3). Biovolume was determined by calculating the surface area using ImageJ and multiplying that by the width/height/length.
	Notes: any other notes relevant to the species

TB2B_CoreByTaxa_With_Juv.csv: sample x species matrix including juveniles of each species
	First column contains sample identifiers; First row contains species identifiers.
	Numbers in each cell refer to abundance of that species for each collected sample at the TB2B site.
	Example: column C2 contains abundance of the species Biv-2 for the TB2B-18.6-17 sample


#######################################################################################################################################################################################################################
