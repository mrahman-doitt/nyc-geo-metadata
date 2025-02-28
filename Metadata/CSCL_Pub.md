# CSCL Pub

Geometry Type: point, line, polygon<br><br>![image](../Images/CSCL.png)

# Table of Contents 
- [Identification](#identification)
- [Data Quality and Specifications](#data-quality-and-specifications)
- [Feature Classes](#feature-classes) 


## Identification


|     |     |
| --- | --- |
**Purpose** |The published Citywide Street Centerline (CSCL) is a comprehensive and authoritative spatial database for the City of New York. It contains a simplified version of the CSCL database and is intended for general-purpose use. CSCL is used by many city agencies including Public Safety call centers, the Department of City Planning's Geosupport, and FDNY EMS dispatch systems. The CSCL database is accessible to the public and will support the Next Generation 911 system.
**Description** |This published CSCL database is an [ESRI file geodatabase](https://en.wikipedia.org/wiki/Geodatabase_(Esri)) and includes a feature dataset, 40 feature classes, 3 tables, and 2 relationship classes. The source data for the published CSCL database is updated daily by the NYC Office of Technology and Innovation (OTI) and the Department of City Planning (DCP) and is governed by 8 city agencies.
**Publication Dates** |**Last Update**: Weekly<br>**Metadata**: 01/16/2025<br>**Update Frequency**: Features are updated daily by staff and released publicly on [NYCMaps](https://nycmaps-nyc.hub.arcgis.com/). 
**Available Formats** | (zipped) ESRI File Geodatabase 
**Use Limitations** |NYC Open Data policies and restrictions apply. See [Terms of Use](http://www.nyc.gov/html/data/terms.html)
**Access Rights** |Public
**Links** |https://nyc.maps.arcgis.com/home/item.html?id=9163b04952354da2bf748abe1788e985
**Tags** |CSCL Pub


## Data Quality and Specifications

|     |     |
| --- | --- |
**Horizontal Coordinate System** |New York State Plane Coordinates, Long Island East Zone, NAD83, US foot ([epsg:2263](https://spatialreference.org/ref/epsg/2263/))
**Spatial Coverage** |New York City, NY
**Positional Accuracy** |Varies 
**Features Captured** |See feature classes listed below

----

## Feature Classes 

| Feature Type | Name | Description |
| ---|---|---|
|**Feature Dataset**|CSCL|The CSCL feature dataset is a collection of the following features and relationship classes: Centerline, Milepost, Node, NonStreetFeature, Rail, ReferenceMarker, Shoreline, Subway, CenterlineHaveAddresses, CenterlineHaveNames.|
|**Points**|[AddressPoint](./Metadata_AddressPoint.md)|A data model that represents the actual addresses present in the field. |
| |[CommonPlace](./Metadata_PointsOfInterest.md)|A point feature dataset representing locations of various points of interest within the boundaries of New York City, such as schools, churches, parks, and museums.|
| |FerryLanding|The ferry landing feature class represents publicly accessible points where passenger-carrying ships dock to load and unload passengers based on a published schedule. |
| |MilePost|The milepost feature class represents small signs placed along limited-access arterials, such as highways, bridges, and tunnels. These signs indicate the exact distance from a designated reference point, typically the starting point of the arterial.|
| |NamedIntersection|The named intersection table associates nodes (intersections) that have names in New York City.|
| |Node|The node feature class represents the points where multiple linear features in CSCL intersect (a topological junction). It is used to assign values to intersections and to create other CSCL feature classes, such as virtual intersections.|
| |RailStation|Locations of all rail stations within New York City.|
| |ReferenceMarker|The reference markers feature class represents state-maintained reference markers in New York City. These markers are small signs placed systematically at intervals of one-tenth of a mile along state-maintained roads and highways.|
| |SubwayStation|Locations of all subway stations within New York City. |
| |TollBooth|New York City's tollbooth locations. |
|**Lines**|[Centerline](./Metadata_StreetCenterline.md)|Centerline is a single line representation of New York City streets containing address ranges and other information such as traffic directions, road types, segment types.|
| |NonStreetFeature| A single-line representation of non-street features. The subtypes of NonStreetFeature include:1) Census_block 2) District_Boundary 3) Election_District 4) Other 5) Physical_Non_ST_Feature 6) Pier_Outline 7) School_District. |
| |Rail|A single line representation of New York City railroads containing route and other information. |
| |Shoreline|A single line representation of New York City shorelines. |
| |Subway|A single line representation of the New York City subway system. |
|**Polygon**|AssemblyDistrict|New York State assembly district boundaries for the City of New York. It is extracted by dissolving combined appropriate fields in atomic polygons.|
| |Borough|A polygon representation of New York City boroughs. |
| |BusinessImprovementDistrict|Business improvement district (BID) name and geographic boundaries. |
| |CensusBlock2000|Census blocks for the 2000 US census. These boundary files are derived from the US Census Bureau's TIGER project and have been modified by dissolving combined appropriate fields in atomic polygons. |
| |CensusBlock2010|Census blocks for the 2010 US census. These boundary files are derived from the US Census Bureau's TIGER project and have been modified by dissolving combined appropriate fields in atomic polygons. |
| |CensusBlock2020|Census blocks for the 2020 US census. These boundary files are derived from the US Census Bureau's TIGER project and have been modified by dissolving combined appropriate fields in atomic polygons. |
| |CensusTract2000|Census tracts for the 2000 US census. These boundary files are derived from the US Census Bureau's TIGER project and have been geographically modified to fit the New York City base map. Because some census tract are under water not all census tracts are contained in this file, only census tracts that are partially or totally located on land have been mapped in this file. |
| |CensusTract2010|Census tracts for the 2010 US census. These boundary files are derived from the US Census Bureau's TIGER project and have been geographically modified to fit the New York City base map. Because some census tracts are under water not all census tracts are contained in this file, only census tracts that are partially or totally located on land have been mapped in this file. |
| |CensusTract2020|Census tracts for the 2020 US Census. These boundary files are derived from the US Census Bureau's TIGER project and have been geographically modified to fit the New York City base map. Because some census tracts are under water not all census tracts are contained in this file, only census tracts that are partially or totally located on land have been mapped in this file. |
| |CityCouncilDistrict|The city council districts are the result of the recent redistricting process, which takes place every ten years to reflect population changes reported in the 2020 Census. These geographies were redrawn by the New York City Council Redistricting Commission. |
| |CommunityDistrict|Community Districts are mandated by the city charter to review and monitor quality of life issues for New York City neighborhoods. It is extracted by dissolving combined appropriate fields in atomic polygons. |
| |Complex|Complex is a polygon representation of New York City complexes including colleges, hospitals, rail yards, parks, commercial centers, and other govermental buildings campuses. |
| |CongressionalDistrict|US House of Representatives Congressional District boundaries for the City of New York. These district boundaries represent the redistricting as of the US Census 2020. |
| |ElectionDistrict|New York City Board of Elections election districts for the City of New York. These district boundaries represent the redistricting as of the US Census 2020. It is extracted by dissolving combined appropriate fields in atomic polygons. |
| |FireCompany|The service area boundaries for New York City's fire companies. |
| |HealthArea|The boundaries for New York City's health areas.|
| |HealthCenterDistrict|The boundaries for New York City's health center areas. |
| |HistoricDistrict|The boundaries of New York City's historic districts are defined by the Landmarks Preservation Commission. |
| |HurricaneEvacuationZone|New York City's hurricane contingency plans are based on six evacuation zones. Hurricane evacuation zones are areas of the city that may be inundated by storm surge or isolated by storm surge waters. There are six zones, ranked by the risk of storm surge impact, with Zone 1 being the most likely to flood. In the event of a hurricane or tropical storm, residents in these zones may be ordered to evacuate. |
| |MunicipalCourtDistrict|The New York City Municipal Court boundaries. |
| |Neighborhood|An NYC Neighborhood is a projection area created from census tracts within New York City's 55 PUMAs (Public Use Microdata Areas). These areas were designed for population projections from 2000 to 2030, with each having at least 15,000 people in 2000 to improve accuracy. The boundaries may not match historical neighborhoods, and the names are not definitive. |
| |NYPDPrecinct|The service area boundaries for New York City's police precincts. |
| |SchoolDistrict|The current NYC school district boundaries. It is extracted by dissolving combined appropriate fields in atomic polygons. |
| |StateSenateDistrict|New York State senate district boundaries for the City of New York. |
| |ZipCode|The boundaries for New York City’s ZIP Codes.|
|**Tables**|ALTSEGMENTDATA|Stores "alternative" data for CSCL centerline, rail, and shoreline segments. |
| | FEATURENAME |Stores the names of common places and rail/subway features. It is used to associate one or more names with a CSCL common place point, complex, rail, or subway feature. |
| | StreetName |The StreetName table stores street names. The street name is parsed into seven component parts according to National Emergency Number Association (NENA) standards. |
|**Relationship Classes**|The CSCL feature dataset includes 2 [ESRI Relationship classes](https://pro.arcgis.com/en/pro-app/latest/help/data/relationships/geodatabase-relationship-class-fundamentals.htm) to manage the associations between objects in one feature class or table and objects in another. |<ul><li>CenterlinesHaveAltAddresses</li><li>CenterlinesHaveNames</li></ul> |


