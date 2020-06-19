# PotHoleDetector

The Objective of the project is to save lives of people by trying to minimize accidents on the road 
Potholes are serious concern issue in our country. People find it difficult to avoid potholes while driving. We are addressing this problem by building a pothole detector system and helping the drivers know about the road conditions by alerting them through maps.

We have built an android application which uses the camera and then calculates what percentage it is a pothole and pins the location to the map.

To detect potholes present in Roads via a camera mounted to public/private vehicles and intimate the corresponding authorities for necessary act.The System updates the Geo-Location of every potholes detected to a centralized data center with the image and severity.

The data in the data center is used to analyze Road conditions for immediate and prioritized actions.The Analyzed Report Lists the potholes in the most commuted roads and helps the authorities to decide the quickness of the action.


Implementation  

Recorder video clip will be converted into image frames using open CV and will be shared to the Azure Custom vision Api to detect the Potholes. The Images with potholes prediction percentage of 50 or more will be considered and the corresponding geo-location of the image will be send to the Azure functions api. The azure function api will take care of persisting the received information into the azure sql server database. The admin can extract the data and a visualize the data with Azure Power BI reports for analytics and can group the data by Date, Location, Seviority, Most Used etc..





