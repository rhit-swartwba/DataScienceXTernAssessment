# DataScienceXTernAssessment

I used the Places API from Google to gather my data. Unfortunately, this seemed to have no information about the type of food offered by each truck. I did not want to use another API key because I did not want to overdo their usage and have to pay for them. This is my first time working with Google's paid APIs, so I wanted to ensure I use it as little as possible.

With the data I gathered, the main parsing I needed to do was with the Open-Hours. As you can see in my code, the original form came in [Monday: 2:00pm-3:00pm, Tuesday...]. I had to do some parsing - first removing the brackets, then extracting each day's value and putting it in the pandas dataset so the data would be cleanly displayed for each day of the week. This would make it easier to see Saturday and Sunday's open times for my planning.

The dataset seemed to capture most of the food trucks available in Indiana. Some seem outdated and need editing, but this was the best data gathering from the API I could manage.

Unfortunately, I was unable to use geopy and its packages to extract the longitude and latitude given the addresses of each food truck. Thus, I had to manually put them in a converter and add the coordinates to my data plan. I also used Google Maps to calculate the time and distance for each one. Given more time and not being swamped with coursework, I would research more about these APIS to automatically get the distance and details from the addresses alone. However, as it was, I picked my favorite locations and made a pandas dataframe of the plan and saved it to an excel file.

Beyond that, I used Folium to visualize the routes that I would plan for the 2-day foodie plan trip. The information is also visible by hovering over each destination point. I then saved this html file and uploaded an image of it here. In my 2 day plan, I wanted to do the least moving around as possible, and in between time the group for just enjoy each other's company and talk, or even just continue working and coding nearby. I like to keep things easy and simple for everyone and want to enjoy spending time with each other more than just food (I'm not a big food truck person). 
