Using [Flat Data](https://next.github.com/projects/flat-data) to pull live-updated data from the [NASA Exoplanet Archive](https://exoplanetarchive.ipac.caltech.edu/docs/TAP/usingTAP.html). As of September 10, 2021, it includes 4,516 planets discovered outside of our solar system. There are 53 known planets orbiting 3-sun systems, like Liu Cixin's [Trisolarans](https://en.wikipedia.org/wiki/Remembrance_of_Earth%27s_Past), and 2 planets orbiting 4-sun systems: [PH1 b](https://exoplanetarchive.ipac.caltech.edu/overview/PH1b) and [30 Ari B b](https://exoplanetarchive.ipac.caltech.edu/overview/30Ari).

To view a filterable, sortable version of this data file, 👉[CLICK HERE](https://flatgithub.com/gwijthoff/exoplanets?filename=exoplanets.json)👈.

(In fact, [Flat Viewer](https://github.com/githubocto/flat-viewer) gives you this nice UI for viewing any .csv or .json data on GitHub by adding "flat" to a repository's URL, i.e. `github.com/gwijthoff/exoplanets` → `flatgithub.com/gwijthoff/exoplanets`.)

# Table Definitions

Database Column Name | Table Label | Description
---------------------|-------------|------------
`pl_name` | Planet Name | Planet name most commonly used in the literature
`discoverymethod` | Discovery Method | Method by which the planet was first identified
`disc_year` | Discovery Year | Year the planet was discovered 
`disc_refname` | Discovery Reference | Reference name for discovery publication 
`disc_locale` | Discovery Locale |  Location of observation of planet discovery (Ground or Space) 
`disc_facility` | Discovery Facility | Name of facility of planet discovery observations 
`disc_telescope` | Discovery Telescope | Name of telescope of planet discovery observations 	
`pl_orbper` | Orbital Period [days] |	Time the planet takes to make a complete orbit around the host star or system
`pl_rade` | Planet Radius [Earth Radius] | Length of a line segment from the center of the planet to its surface, measured in units of radius of the Earth
`pl_bmasse` | Planet Mass or `Mass*sin(i)` [Earth Mass] | Best planet mass estimate available, in order of preference: Mass, `M*sin(i)/sin(i)`, or `M*sin(i)`, depending on availability, and measured in Earth masses
`st_spectype` | Spectral Type | Classification of the star based on their spectral characteristics following the [Morgan-Keenan system](https://en.wikipedia.org/wiki/Stellar_classification)
`sy_snum` | Number of Stars | Number of stars in the planetary system
`sy_pnum` | Number of Planets | Number of planets in the planetary system
`sy_mnum` | Number of Moons | Number of moons in the planetary system
`cb_flag` | Circumbinary Flag | Flag indicating whether the planet orbits a binary system (1=yes, 0=no)
