# Mapping_Earthquakes

Module 13



Basic Project Plan
Purpose
The purpose of this project is to visually show the differences between the magnitudes of earthquakes all over the world for the last seven days.

Tasks
To complete this project, use a URL for GeoJSON earthquake data from the USGS website and retrieve geographical coordinates and the magnitudes of earthquakes for the last seven days. Then add the data to a map.

Approach
Your approach will be to use the JavaScript and the D3.js library to retrieve the coordinates and magnitudes of the earthquakes from the GeoJSON data. You'll use the Leaflet library to plot the data on a Mapbox map through an API request and create interactivity for the earthquake data.

Now that you have an overview of the project plan, let's set up a Mapbox account and get the API token you'll need to create geographical maps.

Background
Basil and Sadhana like how you created your earthquake map with two different maps and the earthquake overlay. Now, Basil and Sadhana would like to see the earthquake data in relation to the tectonic plates’ location on the earth, and they would like to see all the earthquakes with a magnitude greater than 4.5 on the map, and they would like to see the data on a third map.

What You're Creating
This new assignment consists of three technical analysis deliverables. You will submit the following:

Deliverable 1: Add Tectonic Plate Data
Deliverable 2: Add Major Earthquake Data
Deliverable 3: Add an Additional Map
! https://github.com/Dybondzy/Mapping_Earthquakes/blob/main/index.html
! https://github.com/Dybondzy/Mapping_Earthquakes/blob/main/challenge_logic.js

Files
Use the following links to download the Challenge starter code.

Download the tectonic plate starter code. (Links to an external site.)

Download the major earthquake chart starter code. (Links to an external site.)

Deliverable 1: Add Tectonic Plate Data (35 points)
Deliverable 1 Instructions
Using your knowledge of JavaScript, Leaflet.js, and geoJSON data, you’ll add tectonic plate data using d3.json(), add the data using the geoJSON() layer, set the tectonic plate LineString data to stand out on the map, and add the tectonic plate data to the overlay object with the earthquake data.

Follow the instructions below and the numbered comments in the starter code to complete Deliverable 1.

Create a new folder on your Mapping_Earthquakes repository and name it "Earthquake_Challenge."

Copy the folders and files from your Earthquakes_past7days branch and add them to the Earthquake_Challenge folder. The folder should have this structure:

Earthquake_Challenge folder
index.html
! https://github.com/Dybondzy/Mapping_Earthquakes/blob/main/index.html

static
css
style.css
! https://github.com/Dybondzy/Mapping_Earthquakes/blob/main/style.css

js
config.js
logic.js
! https://github.com/Dybondzy/Mapping_Earthquakes/blob/main/logic.js


Download the tectonic_plate_starter_logic.js file, add it to your js folder, and rename it challenge_logic.js.

In Step 1, add a second layer group variable for the tectonic plate data.

In Step 2, add a reference to the tectonic plate data to the overlay object.

In Step 3, using d3.json() callback method, make a call to the tectonic plate data using the GeoJSON/PB2002_boundaries.json data from this GitHub repository (Links to an external site.) for the tectonic plate data. You’ll need to log into GitHub to access the GeoJSON data.

Inside the d3.json() method do the following:

Pass the tectonic plate data to the geoJSON() layer.
Style the lines with a color and weight that will make it stand out on all maps.
Add the tectonic layer group variable you created in Step 1 to the map, i.e., .addTo(tectonicPlates) and close the geoJSON() layer.
Next, add the tectonic layer group variable to the map, i.e, tectonicPlates.addTo(map).
Finally, close the d3.json() callback.
Start your Python server and launch the index.html file and confirm that your map with the earthquake and tectonic plate data is similar to the following image.

Your final map should look similar to the following image:

Deliverable 1 Requirements
You will earn a perfect score for Deliverable 1 by completing all requirements below:

The tectonic plate data is added as a second layer group (10 pt)
The tectonic plate data is added to the overlay object (10 pt)
The d3.json() callback is working and does the following: (10 pt)
The tectonic plate data is passed to the geoJSON() layer
The geoJSON() layer adds color and width to the tectonic plate lines
The tectonic layer group variable is added to the map
The earthquake data and tectonic plate data displayed on the map when the page loads (5 pt)
Deliverable 2: Add Major Earthquake Data (50 points)
Deliverable 2 Instructions
Using your knowledge of JavaScript, Leaflet.js, and geoJSON data, you’ll add major earthquake data to the map using d3.json(), and a color and set the radius of the circle based on the magnitude of earthquake, and add a popup marker for each earthquake that displays the magnitude and location of the earthquake using the GeoJSON layer, geoJSON().

Download the major_eq_starter_logic.js file and add it to your js folder. Look over the starter code and use it as a template to modify your challenge_logic.js file that you used to add the tectonic plate data in Deliverable 1.

Follow the instructions below that refer to the steps in the major_eq_starter_logic.js file and make the changes to your challenge_logic.js file to complete Deliverable 2.

In Step 1, add a third layer group variable for the major earthquake data.
In Step 2, add a reference to the major earthquake data to the overlay object.
In Step 3, d3.json() callback method to make a call to the major earthquake data from the GeoJSON Summary Feed for M4.5+ Earthquakes (Links to an external site.) for the Past 7 Days.
In Step 4, use the same parameters in the styleInfo() function that will make a call to the getColor() and getRadius() functions.
In Step 5, change the getColor() function to use only three colors for the following magnitudes; magnitude less than 4, a magnitude greater than 4, and a magnitude greater than 5.
In Step 6, use the same parameters in the getRadius() function.
In Step 7, pass the major earthquake data into the GeoJSON layer and do the following with the geoJSON() layer:
Turn each feature into a circleMarker on the map
Style each circle with styleInfo() function
Create a popup for the circle to display the magnitude and location of the earthquake
Add the major earthquake layer group variable you created in Step 1 to the map, i.e., .addTo(majorEQ) and then close the geoJSON() layer.
Then, add the major earthquake layer group variable to the map, i.e, majorEQ.addTo(map), and then close the d3.json() callback.
Start your Python server and launch the index.html file and confirm that your map with the two earthquake data sets and tectonic plate data is similar to the following image.

Deliverable 2 Requirements
You will earn a perfect score for Deliverable 2 by completing all requirements below:

The major earthquake data is added as a third layer group (10 pt)
The major earthquake data is added to the overlay object (10 pt)
The d3.json() callback is working and does the following: (25 pt)
Sets the color and diameter of each earthquake.
The major earthquake data is passed to the geoJSON() layer.
The geoJSON() layer creates a circle for each major earthquake, and adds a popup for each circle to display the magnitude and location of the earthquake
The major earthquake layer group variable is added to the map
All the earthquake data and tectonic plate data are displayed on the map when the page loads and the datasets can be toggled on or off (5 pt)
Deliverable 3: Add an Additional Map (15 points)
Deliverable 3 Instructions
Using your knowledge of JavaScript and Leaflet.js add a third map style to your earthquake map.

Rubric
Follow the instructions to complete Deliverable 3.

Using the options from the Mapbox styles (Links to an external site.), add a third map style as a tile layer object to the challenge_logic.js file.
Add the map variable to the base layer object.
Start your Python server and launch the index.html file and confirm that your map is similar to the following image, where there are three map styles, and displays the two earthquake data sets and the tectonic plate data.

Deliverable 3 Requirements
You will earn a perfect score for Deliverable 3 by completing all requirements below:

A third map tile layer is created (5 pt)
The third map is added to the overlay object (5 pt)
All the earthquake data and tectonic plate data are displayed on the all maps of the webpage (5 pt)
Submission
Once you’re ready to submit, make sure to check your work against the rubric to ensure you are meeting the requirements for this Challenge one final time. It’s easy to overlook items when you’re in the zone!

As a reminder, the deliverables for this Challenge are as follows:

Deliverable 1: Add Tectonic Plate Data
Deliverable 2: Add Major Earthquake Data
Deliverable 3: Add an Additional Map
Upload the Earthquake_Challenge folder with the following folders and files to your Mapping_Earthquakes GitHub repository:

The Earthquake_Challenge folder

index.html
! https://github.com/Dybondzy/Mapping_Earthquakes/blob/main/index.html

static
css
style.css
! https://github.com/Dybondzy/Mapping_Earthquakes/blob/main/style.css

js
challenge_logic.js
! https://github.com/Dybondzy/Mapping_Earthquakes/blob/main/challenge_logic.js

A README.md that describes the purpose of the repository. Although there is no graded written analysis for this challenge, it is encouraged and good practice to add a brief description of your project.
