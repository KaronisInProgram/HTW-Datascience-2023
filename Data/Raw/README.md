# Information

Each folder hold the raw Information to its topic.
All Information are present as csv or xlxs files.

The Folder "Covid" is a special case  where it is an submodul of the repository of the [RKI Covid Repository](https://github.com/robert-koch-institut/SARS-CoV-2-Infektionen_in_Deutschland).

## Sources

- [Covid](https://github.com/robert-koch-institut/SARS-CoV-2-Infektionen_in_Deutschland) (see above)
- [Covid-Counteractions](https://www.corona-daten-deutschland.de/dataset)
  - File: [Bundesland_Oberkategorie](https://www.corona-daten-deutschland.de/dataset/massnahmen_oberkategorien_bundeslaender)
- [Emission overviews by sector](https://www.umweltbundesamt.de/sites/default/files/medien/361/dokumente/2023_03_15_em_entwicklung_in_d_ksg-sektoren_pm.xlsx)
- [Emission overviews by type of gas](https://www.umweltbundesamt.de/sites/default/files/medien/361/dokumente/2023_03_15_em_entwicklung_in_d_ksg-sektoren_pm.xlsx)
- [Geographic](https://www.destatis.de/DE/Themen/Laender-Regionen/_inhalt.html)
  - File: [AuszugGV2QAktuell](https://www.destatis.de/DE/Themen/Laender-Regionen/Regionales/Gemeindeverzeichnis/Administrativ/Archiv/GVAuszugQ/AuszugGV2QAktuell.html)
- [Gueter-Personenverkehr](https://www.destatis.de/DE/Themen/Branchen-Unternehmen/Transport-Verkehr/_Grafik/_Interaktiv/gueter-personenverkehr.html)
- [PM10](https://www.umweltbundesamt.de/daten/luft/luftdaten)
  - File: Each File is generated with an URL lik this:

    "https://www.umweltbundesamt.de/api/air_data/v2/measures/csv?date_from=2016-01-01&time_from=12&date_to=2016-12-31&time_to=12&data%5B0%5D%5Bco%5D=1&data%5B0%5D%5Bsc%5D=3&lang=de"
    
 - [Passenger traffic](https://ec.europa.eu/eurostat/databrowser/explore/all/transp?lang=de&display=list&sort=date)

    Each File contains the information of 1 year.
