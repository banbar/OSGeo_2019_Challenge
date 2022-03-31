# OSGeo_2019_Challenge

This tutorial is based on the [OSGeo tutorial](https://wiki.osgeo.org/wiki/Training_Material_for_2019_UN_Open_GIS_Challenge_2_-_Open_geospatial_data_and_software_for_UN_SDG_16,_Peace_justice_and_open_institutions). The libraries used within the tutorial may change over time, so in order to allow pull requests, this GitHub repo is created. Therefore, this repo complements the technical information presented in the original tutorial.

>:white_check_mark: **If you are using this plugin for scientific research, please cite the paper** <a href=https://www.int-arch-photogramm-remote-sens-spatial-inf-sci.net/XLIII-B4-2020/221/2020/>`<b>Educational Material Development on Mobile Spatial Data Collection Using Open Source Geospatial Technologies </b></a>

## Software Used

* PostgreSQL (Postgres) 11.5 is used to create the database that would store the collected data. PostGIS 2.5.3 extension is used to handle spatial data.
* QGIS 3.10 is used to create the project based on the data stored in the Postgres.
* QField 1.2.0 is used for mobile data collection and editing.
* Syncthing is used to synchronize collected photos.
* NodeJS 12.13.1 is used to visualize the collected data on the web.
* Visual Studio Code 1.41.0 is the Integrated Development Environment for developing the JavaScript code.
* Git is a version control system that is required to deploy the web based application.


## Prequisite Work
1. Install the aforementioned software.
2. Open a Heroku account.
3.

```PostgreSQL
create table tree_type
(name_en character varying(30),
 name_tr character varying(30),
 constraint tree_types_pkey primary key (name_en))

insert into tree_type(name_en, name_tr) values
('Oak', 'Meşe'),
('Pine', 'Çam'),
('Plane Tree', 'Çınar')
```
