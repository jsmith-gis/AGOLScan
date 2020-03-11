# ArcGIS Online Feature Service Security Scan
This python script is intended to be used to scan an ArcGIS Online organization for feature services shared publicly.  The script will attempt to access the public feature services that are identified and determine if any editing capabilities are allowed.  A listing of these feature services and corresponding editing capabilities are output to a report in HTML format.
# Requirements
* Python 3.x
* An ArcGIS Online organization domain name (ex. sample.maps.arcgis.com)
* If the organization is private (ie anonymous access is disabled), a username/password is required in order to search for any   public feature services
# Instructions
1. Download the repository ZIP file.
2. Execute the python script on a machine with Internet access. The following arguments are optional and can be included when executing the script:
```
   -h,-?, --help                         Shows help message
   -n ORGNAME, --orgname ORGNAME         Organization domain name (ex. sample.maps.arcgis.com)
   -o OUTPUTDIR, --outputdir OUTPUTDIR   Ouput directory
   -u USERNAME, --username USERNAME      Username from the organization (must be an ArcGIS account)
   -p PASSWORD, --password PASSWORD      Password
```
