

### Overview:
Create a tool that allows the Curator to select a nationality, artist, and minimum year of creation and display their earliest work.

![Image](https://github.com/user-attachments/assets/b5575520-defe-4de8-8ee5-a1c80370ce7d)

[![Watch Demo](https://github.com/user-attachments/assets/e7c11eb2-1077-491f-9f9a-fc3aedae67f8)

#### Objectives:
* Clean the artwork data by looking up the artist(s) for each piece and extracting it's date of creation.

	- Look up the Artist for each artwork by using the ConstituentID field
	- Create a CleanDate column that extract the first 4 numeric characters from each Date
	- Clean the OnView column by removing the “MoMA” prefix and quotation marks

* Create dependent dropdown lists for nationality and artist, and display their number of artworks and their earliest & latest work on display.
	- Create a dropdown list with artists’ Nationality in alphabetical order
	- Create a second, dependent dropdown list with the Artists for the selected nationality
	- Calculate the number of Artworks on display for the selected artist
	- Return the CleanDate for the earliest and latest artwork on display for the selected artist


* Return additional information on the selected artist's earliest work after a certain date, along with the image of the artwork itself
	- Return the Title, CleanDate, Medium, Dimensions, Classification, Department, DateAcquired, ImageURL, and OnView for each of the selected artist’s artworks
	- Create a new data validation rule where the user can type in the Min Year to filter the selected artist’s work by
	- Incorporate the Min Year into the filter criteria for the artwork returned
	- Filter and transpose the list so that you only show the details for their earliest artwork
	- Set the ImageURL to display the artwork inside of a cell
