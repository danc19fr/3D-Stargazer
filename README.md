# 3D-Stargazer
Android app to show distance to stars in 3D

Overview
	The purpose of this app is to visualize the stars in three dimensions.
	It is for exploring the sky and learning the relationship between brightness and distance.
	It is not a planetarium type app, nor a game, but somewhere in between.

Hardware
	Android phone or tablet

Programming environment
	Programming will be done in Android Studio, using Kotlin and/or Java.
	The project will managed and archived in GitHub.
	User name:	danc19fr
	Repository:	3D-Stargazer

User Interface

Home screen: sky image
	Up on screen is always to the north.
	Show stars to apparent magnitude 6.5.
	Touch screen
		Swipe (2 axes) and pinch to scroll 3 variables, selected on the setup screen.
		Short tap a star to open a window with star data. 
		Long tap anywhere to switch to setup screen.
	Mouse
		Drag (2 axes) and scroll wheel to scroll 3 variables, selected on the setup screen.
		Left button tap at a star to open a window with star data. 
		Right button to switch to setup screen.
	Scroll variables
		pan: rotate viewpoint horizontally, in RA (horizontal mouse drag or swipe)
		tilt: rotate viewpoint vertically, in DEC (horizontal mouse drag or swipe)
		zoom: change magnification (mouse scroll wheel or pinch)
		warp: move viewpoint in the direction of the center of the screen (scroll wheel or pinch)

Setup screen
	Buttons
		Home
			Set viewpoint back to Earth
		3D mode
			Mono
			3D anaglyph
			3D parallel
			3D cross-eye
		Select scroll wheel / pinch function
			zoom
			warp
	Home screen settings
		show star names
		show constellation lines
		show constellation names
		show RA and DEC at screen center

Files
	constellationship.txt*
		Table of constellation lines, indexing into
		Source: Github.com/stellarium/skycultures/modern/constellationship.fab
	
	constellation_names.eng.txt*
		English names of constellations
		Source: Github.com/stellarium/skycultures/modern/constellation_names.eng.fab

	display.ods
		Spreadsheet showing algorithms to display stars as filled circles without borders.
		Includes calculations for apparent magnitude and color.
	
	Field of View.ods
		Spreadsheet showing algorithms for rotation and translation including 3D viewpoint offsets.
	
	Modules.txt
		List of program modules. These may be implemented as objects, methods, or functions.
	
	star_table.csv
		Table of stars with names, positions, brightness, and color.
		Source: Github.com/astronexus/HYG-Database/hygdata_v3.csv*
		This was imported and modified in spreadsheet hygdata_v3.ods*
		starcolor.ods* was used to explore color representation.
	* not included in repository
