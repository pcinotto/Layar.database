# Layar.database
Information required for hackathon (on 9/23/2017) to improve functionality of LAYAR (tm) application for Indiana low-head dam safety. GitHub Repository includes: .PHP code for LAYAR app (Copyright 2011 by Xuan Wang; Email: xuan@layar.com, Website: http://layar.com); mySQL databse structured for use with this code; associated Config File. 
Indiana Department of Natural Resources Web Service page is available at: https://gis.in.gov/arcgis/rest/services/DNR/Indiana_LowHead_Dams/MapServer/
Data from this IDNR web service needs to be retrieved, formatted, and inserted into the existing mySQL database structure prior to the database being querried by the current PHP code so that the latest information is returned to the LAYAR server (for display on the end user's smart phone / device). This work should all occur as the layer service provider (this PHP code and mySQL database) returns AR content to the LAYAR server. 
Work flow for LAYAR application is as follows (info from the Layar developer site):
  
  A User launches Layar Reality Browser on a supported mobile device. 
  
  Layar Client will send a request to the Layar Server.
  
  Based on the request, the Layar Server will retrieve layer definitions from the publishing website (Layar). 
  
  A list of retrieved layers will be sent by the Layar Server and displayed on the Layar Client (the smart phone).
  
  The User launches a layer from this list (IN Low Head Dams).
  
  A getPOIs request is sent to the Layar Server. 
  
  The Layar Server forwards the Layer Service Provider of that layer.
  
  The layer Service Provider returns AR content based on the Developer API (getPOIs response) back to the Layar Server. 
  
  The Layar Server validates the getPOIs response and sends it back to the Layar Client. 
  
  The Layar Client displays the getPOIs response nicely to the User. 
