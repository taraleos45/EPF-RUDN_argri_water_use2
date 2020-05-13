This project developed for the Geospatial Programming class of Spring 2020, an international collaboration between two universities, 
EPF of France https://www.epf.fr/ and RUDN of Russia http://www.rudn.ru/


I'm a french student in an aeronautic ans space majorand I'm creazy about these subject. This project is made this the help of our instructor
Naci Dilekli (github link: https://github.com/ndilekli/)


This project is established into the global warming situation using Python and arcpy. Water will be a rare good for human, indeed water is the main ressource for
farmers (70% of water use over the world). But in agriculture, the over consuption is enivitable in particular in developping countries.
To reduce this over consuption, the project help the farmer to know if it's necessary to use water.  Using a weather API, the code make a 
raster of rain amount over France every 3h and compile all data over 48h. The final raster makes possible to know the soil state and if water is needed.
(red areas are where the soil is humid because of rain)

![Annotation 2020-05-05 115417](https://user-images.githubusercontent.com/23176004/81821749-8629a100-9532-11ea-8164-99b9e6be960c.png)

We can also have acces to the 3h weather condition past with ArcGIS and the tool IDW raster. 

![Annotation 2020-05-05 121709](https://user-images.githubusercontent.com/23176004/81822126-03551600-9533-11ea-9b69-4956412a1903.png)

How to have the final raster ?

First, download the gdb file with the fishnet and coordinates of all point to get the weather condition, download also the cvs file to get the
coordinates for the python code. For the code it's the projectAgri file.

Then install arcpy module (import arcpy) and install pyowm module for the API (use pip install pyowm by running the command as admin)
Login to the openWeatherMap site to get your own API key and write it in the code. 

Then check the file directory in the code and do not change the database, use the Dorianpro.gdb file, the code will update the file with new weather conditions.

Here the logic of the code to get the final raster (run the 4th cell):
![image](https://user-images.githubusercontent.com/23176004/81823043-27652700-9534-11ea-866d-42cecf318bd3.png)

To have the final answer, run finalanswer function with the localisation of the field and the nearest city. The code tell you if water is needed

You can check the ppt file with the final presentation, presented at the end of the project. Today the project is at the begining and need to be
more accurate with more point and an IDW raster more accurate. Any advice will be greatfull for my project (send it at dorian.boitard@gmail.com).

Thank you for your interest

Dorian
