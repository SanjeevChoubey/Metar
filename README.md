# Metar
feature related to Metar

-Metar -command line api where user can get weather report for icao.
(.env files are not commited here, if you want to use this then setup your environment file)


-ELEPHANTSQL_URL= "<Your Elephant sql URL>"
-METAR_PATH = "https://api.checkwx.com/metar/"
-API_KEY= <Get from Metar website for your user Id>
 
 
 
 
 -- Create a table on postgresql 
  CREATE TABLE weather_metar(
   airport_id serial PRIMARY KEY,
   airport_code VARCHAR (5) NOT NULL,
   raw_text VARCHAR (500) NOT NULL
);
  
  
-how to use
- Build your project and create .exe file

-run cli command 

  - eg ./main meter VOBL
  
  - eg ./main m VOBB
  
  
  OutPut
  - it will tell you whether at your queried airport is good or bad.

