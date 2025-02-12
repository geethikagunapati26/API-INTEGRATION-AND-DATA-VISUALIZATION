# API-INTEGRATION-AND-DATA-VISUALIZATION

COMPANY:CODTECH IT SOLUTIONS

NAME:GEETHIKA GUNAPATI

INTERN ID:CODHC134

DOMAIN:PYTHON PROGRAMMING

DURATION:25TH JAN 2025 TO 25TH FEB 2025

### Description 

This Python script retrieves weather data for a user-specified city using the OpenWeatherMap API, extracts key weather metrics, and visualizes them using a bar chart. Below is a breakdown of the resources, libraries, and techniques used:


 Resources Used:
1. OpenWeatherMap API 
   - The script fetches real-time weather data from the OpenWeatherMap API.
   - The API key (`API_KEY`) is required for authentication and is retrieved from an environment variable (for security).

2. Requests Library (`requests`)
   - Used to send an HTTP GET request to the OpenWeatherMap API.
   - Handles potential connection errors with exception handling (`try-except`).

3. JSON Handling (`json`)  
   - The response from the API is in JSON format.
   - The script extracts specific weather parameters such as temperature, humidity, wind speed, and weather conditions.

4. Matplotlib (`matplotlib.pyplot`) 
   - Used to create a bar chart visualizing the extracted weather data.
   - Bars represent temperature, "feels like" temperature, humidity, and wind speed.
   - Values are displayed on top of each bar for better readability.

5. OS Module (`os`) 
   - Fetches the API key from an environment variable instead of hardcoding it in the script.
   - This enhances security by preventing accidental exposure of sensitive credentials.



 Key Features of the Code:
 User Input Handling 
   - The script prompts the user to enter a city name.

 API Request & Error Handling 
   - Uses `requests.get()` to fetch data.
   - Implements `response.raise_for_status()` to check for failed API requests.
   - Uses exception handling (`try-except`) to catch and handle network errors.

 Data Extraction & Processing  
   - Extracts city name, country code, temperature, humidity, wind speed, and weather description.
   - Converts temperature to Celsius directly via API (`units=metric`).

 Data Visualization 
   - Generates a bar chart to compare weather parameters.
   - Uses different colors for better distinction.
   - Displays numeric values above each bar.

 Security Best Practices
   - The API key is fetched from an environment variable instead of hardcoding it.

 Possible Enhancements:
🔹 Support for multiple cities in one execution.  
🔹 Use of a GUI (e.g., Tkinter or PyQt) for better user experience.  
🔹 More visualization options (line chart, pie chart, etc.).  
🔹 Allow users to choose between Celsius and Fahrenheit.  



# SAMPLE OUTPUT


Enter a city name: Bengaluru

Weather Data for Bengaluru, IN
Temperature: 28.52°C
Feels Like: 29.00°C
Humidity: 65%
Wind Speed: 4.1 m/s
Weather: Clear (clear sky)

# BARCHART VISUALIZATION


A blue bar for Temperature (28.52°C)
A green bar for Feels Like Temperature (29.00°C)
An orange bar for Humidity (65%)
A purple bar for Wind Speed (4.1 m/s)


# OUTPUT:
