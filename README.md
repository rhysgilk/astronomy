Rhys Gilkenson
Astronomy 9
Final Project

Included is a link to my final project for astronomy 9. It is a website that allows the user to learn about the solor system! Features include searching for planets, stars and other bodies within the galaxy. It will also allow the user to view a random body and learn data about it, including:
	French Name
	English Name
	Mass
	Density
	Discovered by and date (if applicable)
If a picture is found, then it is displayed to the user.

The home page of the website displays information from the Astronomy Picture of the Day and information about it for the user to learn about.


This website was made possible through the use of various APIs including the following:
	https://apod.nasa.gov/apod/astropix.html - Astronomy Picture of the Day
	https://api.le-systeme-solaire.net/en/   - The Solar System OpenData
	https://images.nasa.gov                  - NASA Image and Video Library

The APOD API allowed for the image of the day to be pulled from the website database as a JSON object which was then parsed and displayed on the webpage.

The Solar System OpenData database pulled from 287 bodies throughout the solar system at random and returned the data as a JSON object which includes the following data:
	Unique ID
	Name
	English Name
	isPlanet (returns true if it is a planet)
	Moons
	Semimajor Axis
	Perihelion
	Apheion
	Eccentricity
	Inclination
	Mass
	Volume
	Density
	Gravity
	Escape
	Radius
	Dimensions
	Sideral Orbit
	Sideral Rotation
	Around Planet
	Discovery Name
	Discovery Data
	Alerternative Name
I pulled only a few data points from a returned body object, however, a practical application for this website is looking up information about a particular body in the solar system and using the data to computer calculations, like its orbit. The discovery page will display if a body is a planet and will display the discovery information if available.

The NASA Image and Video Library API has a built in search feature which will return a href link to an image, or series of image results for that given search. I was unable to return the best result, so I just displayed the first image result of a given search and displayed it on the website. Because the Solar System OpenData database did not return an image with a given JSON body object, I had to integrate this additional API to add the image to the display page, since without it, the page would be fairly empty. Many of the bodies that are within the previous API database will not return an image in this API database, unfortunately, so it will display a "no image found" message in that case.

In addition to this data display, the website has been customized and stylized to reflect a simplified version of "cosmic colors". Furthermore, the website is fully responsive to all browser sizes and is mobile friendly. There is also a built in JQuery effect to fade in an out of the two different web pages. A header is featured at the top of each page as a navigation tool to switch between the two pages.

I had many more plans for this final project, but unfortunately I was unable to fullfil many of those goals because of the given COVID-19 situation making it difficult to get as much work done as I planned to. Also I do not have the resources for the code that I would have liked to have at home. The additional goals for the project would have been to add in additional information about the bodies by calculating them using the data provided and equations that we learned throughout the semester. I also wanted to include an additional page with more information about the solar system if possible.

Attached is a PDF That contains the code used for both pages of the website. Thank you so much for viewing my final project and I have thoroughly enjoyed this class. It wouldn't have been possible without the work from the class's awesome TA, Max and professor Ginsburg!