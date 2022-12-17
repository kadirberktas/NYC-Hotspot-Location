# NYC-Hotspot-Locations

I tried to develop WIFI network in NYC. Many people have problem about connecting any wifi network. NYC is really big that's way I tried to maximize to wifi network with this project. When I was there, I could not connect to WIFI and I had many problem of this situation.

We can see those datas on map with Power BI.
![ek1](https://user-images.githubusercontent.com/78299757/208173702-a9758f79-11ae-48e0-b569-70300a00d78e.png)

But first we need to know wireless router range and distance;

![ek2](https://user-images.githubusercontent.com/78299757/208182020-5daad478-e84d-4d1b-bcf5-37818d2a2c62.png)
https://www.geckoandfly.com/10041/wireless-wifi-802-11-abgn-router-range-and-distance-comparison/

We can understand the wireless going up to 200 meters. We will base 200 meters. We can understand if is it enough or not to wifi devices in nyc.

If we find the closest wifi devices with python;
#
import pandas as pd

data=pd.read_csv("NYC_Wi-Fi_Hotspot_Locations (1).csv")

data.sort_values("Latitude")
#
//We can get sample according to minimum latitude of 5 wifi devices //
![ek5](https://user-images.githubusercontent.com/78299757/208243325-25995dc8-c1d2-45c0-8b89-edbc68651050.png)

Those five point far away like 8 miles, so it should have been 40 wifi devices but that part has just 5 wifi devices.(We were base 200 meters for wifi distance for each wifi device.

We can say, it active for %12.5 part of NYC. So I think they need to improve that.

