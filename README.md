# Challange 6 - Retrieving movie data with NY Times and TMDB API
-----

## Overview and agenda for data retrieval
1. Import dependencies and set up environment variables
  - requests
      - Used for importing API
  - time
      - Used for sleep time between API requests to stay within the request limit
  - load_dotenv from dotenv
      - Used to load variables to the environment
  - os
      - Imported to use the operating system for getting the environment and API
  - pandas
    - Used for all data related tasks (ex. data manipulation)
  - json
      - Used for correct formatting of the API data
  - Environment variables
    - nyt_api_key
    - tmdb_api_key

2. Access the NYT API
- Set base URL, set/add all applicable filters, and build the main URL including all filters and API key
- Review results
  - Loop through requested pages, use get request to retrieve JSON, and add sleep time to stay within API request limit
  - Convert results to DataFrame
  - Extract requested columns and keywords
  - Make a title list for easy viewing of all result headlines
3. Access the TMDB API
- Set URL, and add API key
- Create a movie list to store results
- Review results
  - Loop through requested pages, use get request to retrieve JSON, and add sleep time to stay within API request limit
  - Extract titles, genres, etc.
  - Add relevant data to a dictionary
  - Convert results to a DataFrame
4. Merge and clean data for export
- Merge the New York Times results with the TMDB results on title
- Clean DataFrame
  - Remove all unwanted characters in DF
  - Drop all unnecessary/unwanted columns
- Export data to CSV
-----
### Additional sources
#### Sources like ChatGPT, Xpert learning assistant, AskBCS, Google, Youtube, and Columbia provided tutoring were used for clarification, and debugging if/where needed.
