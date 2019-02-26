# ArcGIS Online Feature Service Security Scan
This python script is intended to be used to scan an ArcGIS Online organization for feature services shared publicly.  The script will attempt to access the public feature services that are identified and determine if any editing capabilities are allowed.  A listing of these feature services and corresponding editing capabilities are output to a report in HTML format.
# Requirements
* Python (both 2.7 and 3.x are supported)
* An ArcGIS Online organization domain name (ex. sample.maps.arcgis.com)
* An ArcGIS Online organization id (required if your organization does not allow anonymous access) - This can be obtained by examining the URL of any hosted-feature service published to ArcGIS Online.  The part of the URL path between `services.arcgis.com/` and `/arcgis/rest/services` is the id that is needed.
# Instructions
1. Download the repository ZIP file.
2. Execute the python script on a machine with Internet access. The following arguments are optional and can be included when executing the script:
```
   -h,-?, --help                         Shows help message
   -i ORGID, --orgid ORGID               Organization ID
   -n ORGNAME, --orgname ORGNAME         Organization domain name (ex. sample.maps.arcgis.com)
   -o OUTPUTDIR, --outputdir OUTPUTDIR   Ouput directory
```
