# CS410 Final Project: Improved Media Content Search
University of Illinois Urbana-Champaign, Fall 2021  
Professor ChengXiang Zhai  
Team "Bae Area": Brayden Turner and Joshua Smith

## Installation
Improved Media (Music) Content Search (IMCS) runs via an interactive Jupyter Notebook supported by Python 3.7+. Download the LyricSearch.ipynb file and run the cells to import the necessary libraries, scrape lyric data from Genius, and load the model.

To only run queries without downloading the dataset and custom building a model, the simplified notebook can be used which presents a completed [Annoy](https://github.com/spotify/annoy) index and mapping/ data model which can be used to run sample queries. This also uses interactive ipywidgets for single queries. This simplified application uses [AppMode](https://github.com/oschuett/appmode), an easy-to-install open source Jupyter extension to run a notebook as a web application.

## Background
We’ve all tried to remember a song but all we have is a rough description of what the song is about or one line of a lyric we managed to catch. Many search tools for music and movies are limited to metadata such as titles, artist, actors, but not the general sentiment of lyrics and content. The goal is to return a ranked list of songs that fits the description or lyric given. This can also be extended to add tags to content like “Song from Super Bowl 40 Halftime” or “Rolling Stone top 10 movies list” to enhance descriptive search.

## Implementation
### Data Scraping
There was no central data set that contained all of the lyrics we wanted to use for our project. So what we found was a collection of the top 10,000 artists from MTV over the years contained in a csv file. We used that in conjuntion with a python module called `lyricsgenius` that allowed us to scrape Genius.com to get all of the songs and lyrics for each artist. Even with using mulitple cores on our computers it still took 12+ hours to scrape all of the artists. Once we had the lyrics for each song, we cleaned up the lyrics and made sure to seperate each line of the lyric so we could recover them individually later.

### Model


### Searching For Lyrics

## Screenshots
Interactive search app showing results for a query:
![interactive search example](https://github.com/braydenturner/CourseProject/blob/main/screenshots/interactive1.JPG)
