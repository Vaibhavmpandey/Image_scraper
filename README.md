# Image Scraping Web Application

## Overview

This project is a **web application** built using the **Flask framework** and **Python libraries** like **BeautifulSoup** for scraping images from Google Search. Users can input a query through the web interface, and the application will download and store images related to the search term.

## Features

- **Search-based Image Scraping**: Users can enter a search query, and the app scrapes related images from Google Images.
- **Image Downloading**: The app automatically downloads and saves images into a specified directory.
- **Database Integration**: Scraped images are stored in a MongoDB database for easy management and access.
- **Web Interface**: A simple, user-friendly web interface powered by Flask.

## Tech Stack

- **Backend**: Python (Flask, BeautifulSoup, Requests)
- **Frontend**: HTML, CSS (Flask's `render_template` for HTML rendering)
- **Database**: MongoDB (for storing image data)
- **Other Libraries**: `os`, `logging`, `requests`

## Requirements

Before running the project, ensure you have the following installed:

1. **Python 3.x**
2. **MongoDB** (If running locally)
3. **Python Libraries**: Install them using the requirements file:

The key libraries include:

- **Flask**  
- **requests**  
- **beautifulsoup4**  
- **pymongo**  
- **flask-cors**  

## How It Works

- **User Input**: The user submits a search query via a form on the homepage.  
- **Scraping**: The app sends a request to Google Images, scrapes image URLs using BeautifulSoup, and downloads the images to a local directory.  
- **Saving Images**: The downloaded images are saved both locally and stored in a MongoDB database.  
- **Error Handling**: Errors are logged into a scrapper.log file for debugging.

## Troubleshooting

- **Permission Issues**: Ensure that your user has the correct permissions to write to the /images directory.
- **Blocking Issues**: Google may block repeated requests. Use a fake User-Agent in your request headers to prevent being blocked.


