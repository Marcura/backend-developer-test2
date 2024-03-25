# Backend Developer Challenge

Attached [web_challenge.csv](./web_challenge.csv) contains sea routes extracted from AIS data. These are the routes between ports of Hamburg and Bremerhaven in Germany.

The file contains the following columns:
* route_id - some arbitrary route id
* from_port - route origin
* to_port - route destination
* leg_duration - trip duration in milliseconds
* points - an array of vessel observations from GPS where observation is [longitude, latitude, timestamp in epoch milliseconds, actual vessel speed in knots]

Please write a Java program that will calculate the most "representative" route between two ports.
Result should be stored in GeoJSON format, so can be easily visualized on the map.

PS. Please publish the solution to your GitHub and invite us to review it.
