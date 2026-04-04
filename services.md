[<<Back to index](/)

## Services and events

HASL implements some actions that can be useful for accessing data and using for automations or whatnot. Anyway, there are four services that can be used.
You can call trigger them manually using Settings -> Developer Tools -> Actions

- `sl_find_location`: Arguments `search_string`. Returns the closest stop to the search string provided. Uses the SL API.
- `sl_find_trip_id` Arguments `orig`, `dest`, `trips`, `lang`, `simplified`. Returns trips from orig to dest defined as place ids. Uses the SL API.
- `sl_find_trip_pos` Arguments `orig_lat`, `orig_long`, `dest_lat`, `dest_long`, `trips`, `lang`, `simplified`. Returns trips from oirg to dest defined as coordinates. Uses the SL API.
- `rr_find_location`: Arguments `api_key`, `search_string`. Returns the list of stops for the search string provided. Uses the Resrobot API.

Full specification available [here](https://github.com/hasl-sensor/integration/blob/master/custom_components/hasl3/services.yaml)