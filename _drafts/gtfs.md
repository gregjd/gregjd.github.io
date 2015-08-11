The problem with GTFS transit mode categories
------



One of the largest problems we have with the way we talk about transit is that we focus our language on technology instead of service. This is true both in the United States and in many other countries.

One of the most important and surprising things I've learned from Jarett Walker is the importance of language around transit. For example, the usage of the term "line" versus "route" (link).


GTFS's choice of modes emphasizes distinctions that largely don't matter, while glossing over those that really do.


The GTFS mode categories (`route_type`) are [as follows](https://developers.google.com/transit/gtfs/reference?hl=en#routestxt):
0 - Tram, Streetcar, Light rail. Any light rail or street level system within a metropolitan area.
1 - Subway, Metro. Any underground rail system within a metropolitan area.
2 - Rail. Used for intercity or long-distance travel.
3 - Bus. Used for short- and long-distance bus routes.
4 - Ferry. Used for short- and long-distance boat service.
5 - Cable car. Used for street-level cable cars where the cable runs beneath the car.
6 - Gondola, Suspended cable car. Typically used for aerial cable cars where the car is suspended from the cable.
7 - Funicular. Any rail system designed for steep inclines.


GTFS has a category for Subway/Metro. This is great... except that a subway-like service could really be operated on at least four other mode categories: light rail (Los Angeles light rail), train (many servies in and around Tokyo), bus (genuine bus rapid transit), and gondola/funicular (Wuppertal Schwebebahn)[https://en.wikipedia.org/wiki/Wuppertal_Suspension_Railway].



Basically, this terminology focuses on form instead of function. Imagine if we classified roads according to surface material. Yes, it's true that dirt and gravel roads are likely to be minor roads. But what about concrete versus asphalt? Material doesn't tell you if it's a minor residential street or a major expressway, and also doesn't convey whether it's car-only, pedestrian/bike-only, or something in between.


So we've got four categories of modes that





Why is this so problematic for GTFS in particular? Because it means transit agencies _across the world_ are being forced to define their services in terms that aren't very useful, which limits the utility of what can be done with the data, reinforces the general public's discussion of transit in terms of technology instead of service, and reinforces stereotypes about different transit technologies.

On that last point, Google Maps establishes a visual hierarchy of transit by showing different stops at different zoom levels; if you're zoomed close enough, you see all modes, but zoom out and bus stops disappear, then streetcar/light rail stops, then subway stops. Furthermore, if you click to show transit, lines are given a thickness based on mode instead of frequency. What we end up with is a map that equates once-an-hour buses with those that run every 6 minutes, and mixed-traffic streetcars with subway-like light rail. This is a huge impediment to changing the public's understanding of transit service.

[show images - zoom, line thickness]

For contrast, check out the new map for San Francisco transit:


As Jarett Walker pointed out in [his post], the beauty of this map is _not_ up close --- though it's great at that level too --- but rather that you can see the structure of the system at a faraway glance, due to line thickness based on frequency (and red color for faster Rapid and Metro lines). This is the kind of service-based understanding that we need to move toward.




Reinforces
SEPTA's "everything that runs on rails" map. Most of the map is taken up by Regional Rail lines, most of which run once an hour off-peak are nearly useless for intra-city transit (despite the fact that several of them operate entirely within the city).




This post or the other one?

Problematic - "enhanced bus" or "train on wheels"
basically casts the term "bus" (without qualification) as synonymous with a low quality of service.