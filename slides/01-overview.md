---
title: "What is Layman and how it works"
theme: moon
highlightTheme: tomorrow-night-bright
verticalSeparator: <!--v-->
---
## What is Layman and How it Works

### Jiří Kozel

Workshop 4

<small>Big and Open Data and Innovative Hubs in Agriculture, Transport and Rural Development
<br/>
<br/>
Czech University of Life Sciences, Prague
<br/>
<br/>
January 29, 2020
</small>

---
## About Me

* 15 years of work experience in the field
* started at Masaryk University
  * GIS specialist
  * software developer
  * system analyst
  * leader of GIS group @ Institute of Computer Science

<!--v-->
## About Me

* full-time **freelancer** since 2016 
  * maitainer of OpenMapTiles for 2 years
  * BrnoUrganGrid
  * technical leader of GIS4DIS project
  * Layman

<!--v-->
## About Me

* geospatial data
* data modeling, analysis, and processing
* web systems
* maps
* automation and optimization

---
## What is Layman?

Ask <span style="text-decoration: line-through;">Google</span> DuckDuckGo! 

<!--v-->
## Jake Layman

![Jake Layman](img/jake-layman.jpeg)

<!--v-->
## layman

> someone who is **not a professional** in a given field

<small>from Wikitionary</small>

<!--v-->
## So the Layman is not so famous...
### ...yet! 

---
## What is Layman?
- web service for publishing geospatial data online through REST API
- developed since 2018 as part of Databio and Sieusoil projects
- written in Python, published under GNU-GPL license at GitHub
- [https://github.com/jirik/layman](https://github.com/jirik/layman)

<!--v-->
## How Layman Works?
1. Input
    * vector data in **GeoJSON** or **ShapeFile** format
    * cartographic style  in OGC Styled Layer Descriptor or Symbology Encoding format
2. **<span style="color: orange">Layman's Magic</span>**
3. Output
    * standardized OGC APIs
      * Web Map Service
      * Web Feature Service
      * Catalogue Service

---
## Layman Key Features
Layman supports two main models of geospatial data:

- **Layer** is created from combination of vector data (GeoJSON or ShapeFile) and visualization (SLD or SE style).

- **Map** is collection of layers described in JSON format. Also known as **map composition**.

<!--v-->
## Layman Key Features
There are **multiple client applications** for communication with Layman through its REST API:

- simple web client shipped with Layman
- QGIS desktop client
- HSLayers library

<!--v-->
## Layman Key Features
Layman`s **security system** uses two well-known concepts: authentication and authorization.

<p style="text-align: left; margin-bottom: 0">Common configuration</p>

- **authentication** based on widely used OAuth2 protocol
- **authorization** ensuring that only owner of the data may edit it.

<!--v-->
## Layman Key Features
- Large data files can be easily uploaded from browser thanks to chunk upload.
- Asynchronous processing ensures fast communication with REST API.
- Processing tasks can be distributed on multiple servers.

<!--v-->
## Layman Key Features
- Layman stands on the shoulders of widely used programs like Flask, PostgreSQL, PostGIS, GDAL, GeoServer, Celery, and Redis.

---
## WARNING!
### The presentation is going to be <span style="color: orange;">technical</span>!