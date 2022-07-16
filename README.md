# GPXMaker
Tool for creating, combining, and filtering .gpx -files (or just .gpx waypoints right now..).

**Samples use .gpx -dumps from laavu.org**.

## Installation

Requires Python 3.X to be installed. Tested with 3.8.10.

Install required Python libraries:

<code>pip install -r requirements.txt</code>


## Use cases

**Use cases tested with Ubuntu**. 

With Windows, you might need to call the program like:

<code>python gpxmaker </code>


### Filtering .gpx files

Have massive .gpx -dump _hehe_, and need to filter only relevant waypoints?

<code>./gpxmaker --coordinates NorthPoint SouthPoint WestPoint EastPoint</code>

Program already has some templates for filtering waypoints. Check them from /templates -folder and use them with --template -param.

<code>./gpxmaker --template Muotkatunturi</code>

### Save waypoints/templates

Want to save coordinates as a template for future usage?

<code>./gpxmaker --name NewTemplate --coordinates NorthPoint SouthPoint WestPoint EastPoint --add template</code>

Want to save new waypoint to existing .gpx -file?

<code>./gpxmaker --name NewWaypoint --coordinates Latitude Longitude --add waypoint</code>

### Save waypoints<!--/templates -->

<!-- Want to edit existing template?

<code>./gpxmaker --name NewTemplate --coordinates NorthPoint SouthPoint WestPoint EastPoint --add template</code> -->

Want to edit waypoint in .gpx -file?

<code>./gpxmaker --name NewWaypoint --coordinates Latitude Longitude --add waypoint</code>

## Didn't find what you wanted?
More information:

<code>./gpxmaker --help</code>