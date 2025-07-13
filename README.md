# API-DATA-EXTRACTION-FOOTBALL-API-
A simple Python script that calls the Football API to retrieve the Premier League’s top scorers for the 2023 season. It shows how to configure headers, parameters, make an HTTP GET request, check the response status, and print the raw JSON result.

### Prerequisites
- Python 3.6 or higher
- requests library


** API ENDPOINT ** 
The script uses the following URL: ```https://v3.football.api-sports.io/players/topscorers?league=39&season=2023```

** Headers **
Include your RapidAPI key and host in the request headers: 
```headers = {
    'x-rapidapi-key': '<YOUR_API_KEY>',
    'x-rapidapi-host': 'v3.football.api-sports.io',
    'Accept': 'application/json'}```


### How it Works

- The script builds the request by combining the URL, headers, and parameters.
- It calls requests.get(...) to send the HTTP GET request.
- It checks response.status_code for a 200 OK status.
- If successful, it prints “API Connection Successful” and then dumps the raw JSON payload.
- If not, it prints a simple error prompt


### Next Steps

- Parse the JSON response with response.json() and extract specific fields (e.g., player names, goals).
- Add error handling for network failures or unexpected JSON structures.
- Store results in a CSV or database for further analysis.
- Visualize the top scorers using a charting library such as Matplotlib, excel or Seaborn.
