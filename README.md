# REST-API-CLIENT

*COMPANY* : CODETECH IT SOLUTIONS

*NAME* : KONDAKAYALA REDDY HIMAJA 

*INTERN ID* : CT04DF358

*DURATION* : 4-WEEKS

*MENTOR* : NEELA SANTOSH

*DESCRIPTION* : 

The Java program provided is a simple weather application that fetches and displays real-time weather data for a user-specified city. It utilizes the OpenWeatherMap API to retrieve the data and parses the response using the org.json library. The program starts by importing necessary classes for handling HTTP connections, reading input, and parsing JSON. The main logic begins in the main method, where a Scanner object is created to read the city name from the user through the console. After the city name is entered, the scanner is closed to prevent resource leaks. The API key, which should be obtained from the OpenWeatherMap website, is inserted into the API URL that is dynamically constructed using the user-provided city name. The units are set to metric to return the temperature in degrees Celsius.

Next, the program creates a URL object from the API URL and establishes an HTTP connection using HttpURLConnection. It sets the request method to "GET" to indicate that it wants to retrieve data. The response from the API is read line by line using a BufferedReader and stored in a StringBuilder to form a complete JSON response string. This string is then converted into a JSONObject for easy access to nested values. The program extracts specific pieces of information from the JSON object: the country name from the "sys" object, the main weather condition and description from the first element of the "weather" array, and the current temperature from the "main" object. These values are then displayed to the user in a neatly formatted weather report.

Error handling is implemented using a try-catch block to catch any exceptions that may occur during the process, such as issues with the API URL, network problems, or JSON parsing errors. If an error is encountered, a meaningful message is printed to help the user understand what went wrong. Overall, this program is a beginner-friendly demonstration of working with REST APIs in Java. It shows how to make network requests, read data from an online source, parse JSON responses, and interact with users through the console. To make the program fully functional, the user must replace "your_api_key" with a valid API key from OpenWeatherMap. This application can be further enhanced by displaying more weather details like humidity, wind speed, or by adding a GUI interface for better user experience.

*OUTPUT* :Enter city name: Hyderabad

--- Weather Report ---
City: Hyderabad
Country: IN
Temperature: 32.5 °C
Weather: Clouds
Description: scattered clouds
 
