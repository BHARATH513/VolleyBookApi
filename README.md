# VolleyBookApi
This app that leverages the OpenLibrary API to search books and display cover images. 
### Main-Screen
![Screenphone1](https://user-images.githubusercontent.com/48553566/54358830-485b8f00-4687-11e9-9f51-1367cf52951d.png)

## Overview
#### In this app following things are done
1. Fetch the books from the [OpenLibrary](https://developers.google.com/apis-explorer) Search API in JSON format
2. Parse the JSON data for each of the books into BookModel objects
3. Build an array of BookModel objects and create an Adapter for those books
4. Set the adapter for the books to a RecyclerView to display the data on screen
#### The following components in this app:
1. BookModel - Model object responsible for encapsulating the attributes for each individual book
2. BookAdapter - Responsible for mapping each Book to a particular view layout
3. MainActivity - Responsible for fetching and deserializing the data and configuring the adapter
4. DetailActivity - Responsible for display the fetched data on the details screen for the book

### Background task:
1. In this app to use the Volley background task (this is a third party task). This task is parsing the JSON data configure into
   the MainActivity.java file
   
   Use the dependencies:
   
   implementation 'com.android.volley:volley:1.1.1'

#### URL
Push the book api url in MainActivity
  
  String url=&lt;Book Api Url Address&gt;;
  
#### Suggested:

1. Show ProgressBar before each network request
2. Add a detail view to display more information about the selected book from the list

### Libraries:

[Picasso](https://square.github.io/picasso) - For remote image loading
