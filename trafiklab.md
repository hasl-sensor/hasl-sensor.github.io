[<<Back to index](/)

## Types of keys

This project is dependent on a number of APIs to aquire information. The APIs are mostly free but somewhat limited. Read more about that below.
We now supports using either native SL api for Stockholm, but also Resrobot for the rest of the country (and Stockholm).

If you are in Stockholm I recond using SL as it has more features, however Resrobot also provides intra-regional travel.

## SL Api keys

The project was migrated to the new key-less SL API, so there is no need in API keys for SL data anymore.


## Resrobot Free API key

First, visit [https://www.trafiklab.se/api](https://www.trafiklab.se/api) and create a free account.

They provide multiple APIs, the ones you want is
* ["ResRobot v2.1"](https://www.trafiklab.se/api/trafiklab-apis/resrobot-v21/)

When you have your API key, you're ready to add the component to your Home Assistant either via [HACS](hacs_install) or [manual](manual_install).

## Resrobot API-call restrictions and optimizations

The free `Bronze` level API is limited to 45 API calls per minute, 25.000 per 30 days. That allows for less than one call every 4 minutes but if you are using multiple sensors this is split between them and each config sensor section can contain a separate pair of api-keys.

You can also specify a binary_sensor that perhaps is turned off when no-one is at home or similar to reduce the number of calls.