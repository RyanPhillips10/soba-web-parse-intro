# SoBA Web Curriculum

### Lesson 6: Into to Parse


#### Overview

For this lesson you will again be transforming data with [underscore.js](http://underscorejs.org) and injecting html into the page using [jQuery](http://jquery.com). But now we will be persisting our data using [Parse](http://parse.com), and we will be formatting our pages with [Twitter Bootstrap](http://getbootstrap.com/).

#### Instructions

Again, make sure you fork this repository to your own account and clone it like you did for the first two assignment.

Keep up the habit of branching in git, making your changes, and then merging back into your main branch. As in Assignment 4, instead of branching from main, create a "development" branch first immediately after you clone the repository, and branch from this line when you edit the individual files.

#### Editing the files

For this lesson you will only be editing index.html. The page has already been prepared for you, including links to JavaScript libraries hosted on Content Distribution Networks (CDNs). You should create an application like the one demonstrated in class that retrieves data from Parse, shows it on the page, and lets you update it.

#### The Details

Specifically, you should:

1. Create a new Application in Parse
 
2. Populate it with mock data (specifications below)

3. Create a two column web page using Twitter Bootstrap

4. The first column is a sidebar that shows the items in your Parse database

5. The second column is the main area that presents a form when you select an item in the sidebar. The form includes fields for editing the values of the object with a submit button for updating the values and saving them to Parse

#### The technologies

This lesson integrates all of the technologies we have used so far. You will employ Twitter Bootstrap to format your pages. You will use underscore.js to template parts of your page. You will use jQuery to inject the output of your templates into the DOM and to bind event handlers where appropriate. Finally, you will use Parse to manage your data backend and to retrieve and update data from the webpage.

You should use Parse's [JavaScript guide](https://parse.com/docs/js_guide) while you work on the page. In fact you should consider reading this documentation as part of your homework.

In addition you may refer to the included example.html file, which contains the contents of today's lecture. Do not just copy and paste from this file. Make sure you understand what is happening.

#### Your data set

You should create a Class in your Parse Application's Data Browser called Person. Add columns for

	firstName [String], lastName [String], age [Number], favoriteMusic [String], sex [Number:0|1]
	
Populate your Parse database with a dozen or so fictional people. When you retreive this data, you should display the name and music in the list. When you click on an item in the list, you should display a form that allows you to update all these properties.

#### Advanced

Consider using the Parse.Object.extend method to add a helper function to your Parse object for displaying sex as a string instead of 0 or 1. Refer to the Parse documentation for examples.