# HTW-Datascience-2023

This Repository is for the Data-Aggregation/-Preparation/-Analysis of the Datacience modul from HTW (2023).

## Information (Overview)

In the Folder "Notebooks" are Jupyter-Notebooks that create normalized Data in "Data/Output/*".
In "Data" are the raw Inforamtion that are used to prepare the Data, as well the output for the files that are created when the notebooks are executed.

## Used Tools and Libaries

Here is a short list of the used Tools and Libarys.

### Tools

- [Conda](https://docs.conda.io/projects/conda/en/stable/) (with [Anaconda](https://www.anaconda.com/) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html))
- [Jupyter](https://docs.jupyter.org/en/latest/start/index.html)

### Libaries

- [Pandas](https://pandas.pydata.org/getting_started.html)

### Description of Output

Here is a Description of the normalized output.

#### Covid

| Characteristic    | Description                                                                                                                   |
|:-----------------:|:----------------------------------------------------------------------------------------------------------------------------- |
| Bundesland        | The federal state this record is mapped to.                                                                                   |
| Meldedatum        | Represents the date when the case was registered.                                                                             |
| Refdatum          | Represents the date when the case was happening.                                                                              |
| AnzahlFall        | Sum of all cases for the tuple (Bundesland, Meldedatum) or (Bundesland, Refdatum) decided by which of the dates is present.   |
| AnzahlTodesfall   | Sum of all Death for the tuple (Bundesland, Meldedatum) or (Bundesland, Refdatum) decided by which of the dates is present.   |
| AnzahlGenesen     | Sum of all healed for the tuple (Bundesland, Meldedatum) or (Bundesland, Refdatum) decided by which of the dates is present.  |

The Output ist split in 2 Files. One with the tuple (Bundesland, Meldedatum) ond one with (Bundesland, Refdatum). The above decriped field contains all information of both outputs.

#### Covid-Counteractions

| Characteristic                                            | Description                                                                |
|:---------------------------------------------------------:|:-------------------------------------------------------------------------- |
| Bundesland                                                | The federal state this record is mapped to.                                |
| Datum                                                     | The date when an Action could be active or inactive.                       |
| Kontaktbeschränkung Privatpersonen im privatem Raum       | Measure: Restriction of contact with private individuals in private spaces |
| Kontaktbeschränkung Privatpersonen im öffentlichen Raum   | Measure: Restriction of contact with private individuals in public spaces
| Weiterführende Schulen                                    | Measure for secondary schools
| Grundschulen                                              | Measure for elementary schools    
| Kitas                                                     | Measure for daycares
| Öffentliche Events & Veranstaltungen Indoor               | Measure: Public Events & Events Indoor    
| Öffentliche Events & Veranstaltungen Outdoor              | Measure: Public Events & Events Outdoor    
| Kultur- & Bildungseinrichtungen                           | Measure for cultural & educational institutions  
| Groß- & Einzelhandel                                      | Measure for wholesale & retail     
| Gastronomie                                               | Measure for gastronomy
| Dienstleistungen & Handwerk                               | Measure for services & crafts  
| Einrichtungen des Nachtlebens                             | Measure for nightlife establishments   
| Beherbergung                                              | Measure for accommodation
| Sport Indoor                                              | Measure for Sport Indoor
| Sport Outdoor                                             | Measure for Sport Outdoor
| Reisebeschränkung Inland                                  | Measure for travel restriction inland
| Reisebeschränkung Ausland                                 | Measure for travel restriction abroad  
| Arbeitsplatzbeschränkung                                  | Measure for job restriction 
| Ausgangsbeschränkung                                      | Measure for exit restriction
| Kapazitätsbeschränkung im öffentlichen Verkehr            | Measure: Capacity limitation in public transport 

#### PM10

| Characteristic    | Description                                                                      |
|:-----------------:|:-------------------------------------------------------------------------------- |
| Bundesland        | The federal state this record is mapped to.                                      |
| Datum             | The date the PM10 value was measured.                                            |
| Stationscode      | An unique code for the station.                                                  |
| Stationsumgebung  | Description of the surrounding (regieon) of the station.                         |
| Art der Station   | Description how the station is installed.                                        |
| Messwert*         | The measured value (microgram in cubic meters) as the daily average of 24 hours. |

"Stationsumgebung" has the options of:

- "städtisches Gebiet" means that this station is inside a city
- "vorstädtisches Gebiet" means that this station is in the suburban region of a city
- "ländliches Gebiet" means that this station is outside of a city

"Art der Station" has the options of:

- "Hintergrund" means that this station not near streets or other busy places installed
- "Industrie" means that this station is near or in an industry installed
- "Verkehr" means that this station is near or on a street installed


#### Emission-overviews-by-sector

| Characteristic    | Description                                                                                                                   |
|:-----------------:|:----------------------------------------------------------------------------------------------------------------------------- |
| Sektor            | Total thousands of tons of CO2 emissions by economic sector.                                                                  |
| Energiewirtschaft | Represents the number of thousands of tons of CO2 emissions in the energy economy.                                            |                   
| Industrie         | Represents the number of thousands of tons of CO2 emissions in the industrie.                                                 | 
| Gebäude           | Represents the number of thousands of tons of CO2 emissions in the building sector.                                           |
| Landwirtschaft    | Represents the number of thousands of tons of CO2 emissions in the agricultural sector.                                       |
| Abfallwirtschaft und Sonstiges | Represents the number of thousands of tons of CO2 emissions from the waste management sector and the rest.       |

#### Emission-overviews-by-type-of-gas

| Characteristic    | Description                                                                                                                   |
|:-----------------:|:----------------------------------------------------------------------------------------------------------------------------- |
| Gesamtemissionen  | Total thousands of tons of greenhouse gas emissions for the year in question.                                                 |
| Kohlendioxid      | Thousands of tons of kohlendioxide emissions for the year in question.                                                        |                   
| Methan            | Thousands of tons of methan emissions for the year in question.                                                               | 
| Lachgas           | Thousands of tons of nitrous oxide emissions for the year in question.                                                        |
| F-Gase            | Thousands of tons of F-Gases emissions for the year in question.                                                              |


#### Fluggastverkehr

| Characteristic    | Description                                                                                                                   |
|:-----------------:|:----------------------------------------------------------------------------------------------------------------------------- |
| Time              | Total thousands of tons of greenhouse gas emissions for the year in question.                                                 |
| Europäische Union | Total passenger traffic in the European Union for the year in question.                                                       |            
| Deutschland       | Total passenger traffic in Germany for the year in question.                                                                  | 


#### Gueter-Personenverkehr

| Characteristic    | Description                                                                                                                   |
|:-----------------:|:----------------------------------------------------------------------------------------------------------------------------- |
| Jahr              | Year of traffic flow measurement.                                                                                             |
| Personenverkehr   | Data for personal vehicle traffic, the amount of which is indicated in passenger kilometers.                                  |            
| Gueterverkehr     | Data for truck traffic, the value of which is indicated in passenger kilometers.                                              | 
