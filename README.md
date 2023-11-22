## Docker-Compose TileServerChache

## Installing

-   Install Docker
-   Create a new folder to store the yml file in and change into it:  `
-   mkdir TileServer && cd TileServer`
-   Load the yml:  `wget https://raw.githubusercontent.com/Montesuma80/TileServerChache/main/docker-compose.yml`
-   Edit the docker-compose.yml file if you want to change defaults. Default will work fine.
-   Enable the Admin Interface
-   Create a new folder to store TileServer data in and chagne into it:  `mkdir TileServer`
-   Start and attach to logs:  `docker-compose up -d && docker-compose logs -f`
- Login http://yourip:9000
- 
-    Get Download command from  [https://openmaptiles.com/downloads/planet/](https://openmaptiles.com/downloads/planet/)  for your region.
- -   Download file lokal
- - Upload the File in the Admin Interface and rename file to end in .mbtiles if it got named incorrectly
## Configuration
- now upload the Styles & Fonts with the Admin Interface
- [Styles.zip](https://raw.githubusercontent.com/Montesuma80/TileServerChache/main/styles.zip) 
- [Fonts.zip](https://raw.githubusercontent.com/Montesuma80/TileServerChache/main/fonts.zip) 
- [Templates.zip](https://raw.githubusercontent.com/Montesuma80/TileServerChache/main/templates.zip) 
