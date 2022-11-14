# Python National Weather Service API
To use in your code: `import nws` in a directory containing the `nws.py` file.

# Dependancies
The requests library can be installed using `pip install requests`.

# Methods
`jprint(json: obj) => string` Dump a JSON object to a string for easier printing. 
`get_city(number: lat, number: long) => (number, number)` Get the NWS box coordinates from a latitude and longitude.
`get_temp(number: box_x, number: box_y) => number` Get the temperature, in degrees fareneheit, of the weather station at the given NWS box coordinates.
`get_forcast(number: box_x, number: box_y) => number` Get the forecast of weather conditions within the current hour using the NWS box coordinates.
`get_date_of_forcast(number: box_x, number: box_y, int: hour_offset) => string` Get the date of the forcast at the weather station at the given NWS box coordinates and an hour offset from the current hour.
`get_hourly_forecasts(number: box_x, number: box_y) => string` Get a list of forecasts and temperatures for as many hours the NWS provides. Can be trimmed. Emoji output for some weather conditions

# Main Function
Given NWS box coordinates and an optional label, print the temperature and forcast for the current hour. 
