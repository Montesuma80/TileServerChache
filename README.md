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
### Configuration Styles
- now upload the Styles with the Admin Interface
- [Styles.zip](https://raw.githubusercontent.com/Montesuma80/TileServerChache/main/styles.zip) 

### Add required Fonts and Templates
- stop the Server with `docker compose down`
- download Fonts and Templates with wget to the first TileServer folder
- There is an Folder Templates, extraxt the templates.zip to this folder
- - [Templates.zip](https://raw.githubusercontent.com/Montesuma80/TileServerChache/main/templates.zip) 
- no go to the TilesServer folder in the TilesServer folder, there is an folder named Fonts
- Extraxt the fonts.zip into this folder
- - [Fonts.zip](https://raw.githubusercontent.com/Montesuma80/TileServerChache/main/fonts.zip) 

Now you can start the Server and check it
`docker-compose up -d`

Browser: https://tileserverurl/staticmap?style=klokantech-basic&latitude=47.263416&longitude=11.400512&zoom=17&width=500&height=500&scale=2&pregenerate=true