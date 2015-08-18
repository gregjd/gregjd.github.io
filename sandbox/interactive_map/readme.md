The intention of this is for people who don't know much about programming to be able to create an interactive map of Rhode Island municipalities based on a given dataset. In order to minimize development time (and also allow for easy customization), this does not involve creating a GUI.



## Directions

You'll need to make sure your data is in JSON format, as an object whose keys are municipality names (all caps) and values are objects whose keys are property names and values are property values. Here's an example:

[example]

Getting data from Excel or a CSV into this format is easy. You could certainly run a script that will do this automatically, but you can also do it through a website called [Mr. Data Converter](https://shancarter.github.io/mr-data-converter/). In the top box, paste your data. (It can take data straight from Excel, or as comma-separated or tab-separated values.) In the menu above the bottom box, select _"JSON - Dictionary."_ Your reformatted data is below!

[include screenshot]

If the data you started with was already in the right format, then you don't need to worry about converting it.


To-do: Add the rest of the directions!