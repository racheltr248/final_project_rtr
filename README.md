# Final Project

## Kaggle data cleaning

Removed the following columns either because they were irrelevant to analysis or had too many null values: 
* end_date
* members
* favorites
* episode_duration
* total_duration
* approved
* created_at
* updated_at
* start_year
* real_start_date
* real_end_date
* synopsis
* background
* main_picture
* url
* trailer_url
* title_english
* title_japanese
* title_synonyms
* broadcast_day
* broadcast_time
* status

Converted start_date object to_datetime

Created clean_title.csv and clean_anime.csv

## Next steps
Use get_dummies on the following columns: 
* type
* source
* rating
* sfw
* start_season

There is an issue with the following columns being input as lists. I combined genres and themes into a keywords column, but I'm not sure what to do from here. 
* genres
* themes
* demographics
* studios
* producers
* licensors

### Possible analyses
* I'm interested in whether being an original story or a story from another medium (manga, web-comic, game, etc) impacts higher ratings
* I'm interested in whether certain studios produce more highly-rated anime
* I'm interested in the ratings and types of the most highly scored anime
* I would like to look at the genres/themes of the top-scored whatever number of anime
