[<<Back to index](/)

## Location IDs

To get data about a specific stop for depatures or other sensors you will need to have a Location ID. Location IDs are NOT interchangeable between SL and ResRobot.
Location search is integrated into sensor setup flow, so you don't need to do anything else.
But if you are curious there are ways to get these ids via developer tools.

## Resrobot API 

The IDs you get here is only for use with the Resrobot sensors.

1. Start a browser window and go to the Developer Tools in Home Assistant
1. Navigate to the Actions tab
1. Select the `rr_find_location` action, enter your [API key](trafiklab) for ["ResRobot v2.1"](https://www.trafiklab.se/api/trafiklab-apis/resrobot-v21/) and a search string. Click Perform Action.
1. Look in the response data below and get the `id` for your specific location. Do not use `longId`. Currently addresses are NOT supported.

## Resrobot alternative
You can also get a list of all of the stop [here](https://raw.githubusercontent.com/TekniskSupport/home-assistant-resrobot/master/stops.txt)

## SL API 

The IDs you get here is only for use with the SL sensors.

1. Start a browser window and go to the Developer Tools in Home Assistant
1. Navigate to the Actions tab
1. Select the `sl_find_location` action and a search string. Click Perform Action.
1. Look in the response data below and get the `id` for your specific location.