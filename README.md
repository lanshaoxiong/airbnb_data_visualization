# airbnb_data_visualization

### Introduction:
A map data visualization project which visualizes the information of home listings from Airbnb in Montreal. The map is divided into neighborhoods. This mainly shows the relationship of room type vs number of locations. Moreover, this shows which areas are concentrated with the listings. Other factors are also available like price, number or reviews, and rate. These, when selected, would turn our map into a choropleth one. At the bottom of the map, there are 5 radio buttons, normal, listing, price, reviews, and rate. 

#### Normal View (Marker Cluster)
In default view, the button will be selected to “Normal”. There are marker clusters on the map showing the room distribution in the entire city. When the mouse hovers inside the cluster, a convex polygon is created to show where the listings are. When it hovers on the outer portion of the pie, the number of listings of that specific room type is displayed. 

Note that the clustering is not divided into neighborhoods because we realized that there are 34 neighborhoods and it would messy to show 34 marker clusters. The division of the neighborhoods are visible (solid white border), so the user still knows which neighborhood the listing belongs to. 

If a user is interested to know the distribution of a particular neighborhood, s/he can click on that neighborhood. The map zooms in and only shows the listings of that neighborhood (marker cluster). Some neighborhoods (i.e. Le Plateau-Mont-Royal) has a great amount of number of listings. Since we also want to show how individual listings are spread out in the neighborhood, we included a filter below the radio buttons. Instead of a marker cluster, it will show points. To go back to marker cluster, user can re-select that neighborhood. If user wants to see all clusters in all neighbourhoods again, s/he needs to select filter item to “Montreal”.

The colors on the marker clusters depend on the room types, red for an entire home/apartment, green for a private room, and yellow for a shared room. When the mouse hovers on the neighborhood, the top right panel shows the listing number, average rating, average price, and average reviews of the corresponding neighborhood. Clicking into a neighborhood or a marker cluster, marker clusters will separate into smaller divisions. Then clicking on a small maker cluster, it will be divided into several nodes. Clicking on one single node, the details of the room are shown, such as room id, host id, reviews, accommodates, bedrooms, and price. 

#### Choropleth Maps
Selecting the second radio button “Listing”, the distribution of listings is shown in a choropleth map. In a choropleth map, all maker clusters are disappeared in order to gain a clear visualization. Hovering on the neighborhood, the top right panel shows the number of listings of the neighborhood. The more listings in a neighborhood, the darker are the colors. 

Furthermore, selecting the third radio button “Price”, the distribution of prices is shown in a choropleth map. Hovering on the neighborhood, the top right panel shows the average price per night of the neighborhood. The higher price in a neighborhood is, the darker are the colors. 

In addition, selecting the fourth radio button “Reviews”, the distribution of reviews is shown in a choropleth map. Hovering on the neighborhood, the top right panel shows the number of average reviews of the neighborhood. The more number of reviews in a neighborhood is, the darker are the colors. 

Finally, selecting the firth radio button “Rate”,  the distribution of rates is shown in a choropleth map. Hovering on the neighborhood, the top right panel shows the number of average satisfaction rates of the neighborhood. The higher satisfaction rate in a neighborhood is, the darker are the colors. 

Clicking a neighborhood zooms in the map and shows marker clusters of that neighbourhood. The filter (for distribution of individual listings) is disabled for this.

### how to open?
Download the whole project (css folder, geojson folder, js folder and montreal.html), and open `montreal.html`.
