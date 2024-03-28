# Backend Developer Challenge

Attached [DEBRV_DEHAM_historical_routes.csv](./DEBRV_DEHAM_historical_routes.csv) contains sea routes extracted from AIS data. These are the routes between ports of Hamburg and Bremerhaven in Germany.

The file contains the following columns:
* route_id - some arbitrary route id
* from_seq - sequence number of the route origin
* to_seq - sequence number of the route destination
* from_port - route origin
* to_port - route destination
* leg_duration - trip duration in milliseconds
* count - number of observations in the route
* points - an array of vessel observations from GPS where observation is [longitude, latitude, timestamp in epoch milliseconds, actual vessel speed in knots]

There is also a [DEBRV_DEHAM_historical_routes.geojson.json](./DEBRV_DEHAM_historical_routes.geojson.json) GEOJSON file that you can use to visualize the routes. 
You can use https://geojson.io to load the file online

Please write a Java or Go program that will calculate the most "representative" route between two ports.
Result should be stored in GeoJSON format, so can be easily visualized on the map.

PS. Please publish the solution to your GitHub and invite us to review it.
