# photos2geojs2
Simple tool to convert georeferenced images into a collection of points in GeoJSON

This tool does generally the same thing as https://github.com/briangkatz/gps-photos-to-geojson, but it does not rely on huge 3rd party tools like QGIS. All you have to install are the following dendencies: Pillow and geojson.

## Install

* Install Python 3.x
* Download `photos2geojs.py` (or clone this repository)
* ``` pip install Pillow geojson ```

## Or download photos2geojs2_x64.exe for Windows

## Usage

The tool takes all the JPEG files in one folder and creates a GeoJSON containing FeatureCollection of Points, where each point represents the location of one photo. To simply identify the individual point, the image's file name is saved an "file" property of each point.

* ``` python2geojs.py ```
* the `photos.geojson` file will appear in your working directory
* you may add custom properties, example `photos2geojs2_x64.exe --props prop=lalala,album=spring,test="hello world"`

Check the `photos.geojson` file in this repository to have an idea what it creates.
