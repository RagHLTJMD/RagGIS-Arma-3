# RagGIS-Arma-3
RagGIS(Geographic Information Service) for Arma 3. Dynamic Mapping of Arma 3 campaign areas of opreration. 

RagGIS was built to create a dynamic map for OPCOM UK's Arma 3 campaigns to supliment the intel team. It is a basic web server built using Leaflet that allows for the mapping of strategic assets.

Credit to jetelain.github.io for their work on the bringing the arma 3 maps into Leaflet

# Screenshots
![image](https://user-images.githubusercontent.com/43555809/143468199-3b77412d-4813-4b14-878a-24ad137ec756.png)
![image](https://user-images.githubusercontent.com/43555809/143468466-3392e905-d0b5-47bc-80db-59bbe11716c6.png)
![image](https://user-images.githubusercontent.com/43555809/143468480-e1f7d633-74d3-4deb-9be6-e1c4fbb3e3cb.png)

# How to use

Step 1. Clone the repo and load it into your webserver root

  NGINX - /usr/share/nginx/http
  
Step 2. select which map you want to load by changing lines 25 and 28
  ![image](https://user-images.githubusercontent.com/43555809/143469080-75148368-4027-4a99-88d2-8d3c18a957b1.png)

Step 3. Placing markers. 

How to use Markers in Leaflet
  L.marker([X CORD IN Meters, Y CORD IN Meters], {icon: ICON VAR NAME}).addTo(map);
  Example L.marker([2200, 11840], {icon: BCDO}).addTo(map);

Step 4. Adding more Unit types

Start by declaring the variable with the refrence to their icon (https://spatialillusions.com/unitgenerator/).

![image](https://user-images.githubusercontent.com/43555809/143471775-3f3ec98f-92b7-4631-bc6e-1501249a1448.png)

Then using the markers above just refrence the var name.
