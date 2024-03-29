[<< Back to index](/)

On this page you will have examples for Traffic Status, Route Planning and Disturbances for now. Please submit your examples so we can make this page more complete.

## Custom Lovelace Card: Traffic Status Card
The mostly used card is the [departure-card](https://github.com/hasl-platform/lovelace-hasl-departure-card) which gives you a good overview of a specific stop and the next departures from that. 

![TrafficStatusCard](https://user-images.githubusercontent.com/8133650/56198334-0a150f00-603b-11e9-9e93-92be212d7f7b.PNG)

## Advanced GUI: Route display
You can use the Route sensor to intellegently determine the next trip from one place to another. Can be perfect to always have information about the quickes travel to work for instance. It will fetch all possible travels between the two points and sort by the quickest travel time across all means of travel. The sensor can then display this information on your Lovelace display.

In this example we search for a trip between the station Mölnvik (Location 4244) and Gustavsbergs Centrum (Location 4200):

![NextTrip](https://user-images.githubusercontent.com/8133650/155983899-294650c9-4f41-417a-bcae-dc5b39e15548.png)

* Create a Route Sensor under Integrations in Home Assistant
* Configure the Route Sensor with API-key from Trafic Lab ["SL Reseplanerare 3.1"](https://www.trafiklab.se/api/trafiklab-apis/sl/route-planner-31/) and a start and end of your planned trip.
* Goto your Lovelace and create a Markdown Card, set the title to Gustavsbergs Centrum and paste in the code from [route_sensor.txt](https://hasl.sorlov.com/route_sensor.txt)
* Enjoy!

## Custom Lovelace Card: Traffic Disturbances Card
It is also common to want to have the current traffic interuptions displayed. The simplest way may be to create a Glance Card with the Traffic Status sensors in binary mode.

![Interruptions](https://user-images.githubusercontent.com/8133650/148203200-a454b236-0532-4617-bcce-8e87f2ed92d9.png)

But using the sensors mode you can use the [traffic-status-card](https://github.com/hasl-platform/lovelace-hasl-traffic-status-card) to display more information beyond the simple true or false indicators.

![Interruptions](https://user-images.githubusercontent.com/1217994/57677754-e1773980-7627-11e9-81e7-4b991a6e4dc1.png)






