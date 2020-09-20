# Collect modeling

## Summary, stories about truck capacity, maps, route planning 
Here, you will find a conceptual model of :
* collect schema
* collect process
[Territory](./territory.md) and [Production](./production/md) are defined elsewhere.

### collect schema
* Collect abstract schemas are defined as a datamodel with UML Classes
* Collect schemas templates and examples are defined as preconfigured datamodel, classes, objects and enum.

### collect process
* Computation is defined with UML Activity or Sequence.

## In practice : many models
### Sizing macro (macro approach)
Based on the territory and on the "collect schema" scenario, "Sizing macro" :
* Create a spatial segmentation of the territory seen as a collection of points (adresses with waste production)
* Compute the sizing with the macro algorithm refined by adresses properties
* Compute performance indicators

### Sizing with adresses (micro approach, points on map)
Based on the results of "Sizing macro", "Sizing with points" :
* Create a spatial segmentation of the territory seen as a collection of points (adresses with waste production)
* Compute the sizing with the macro algorithm refined by adresses properties
* Compute performance indicators

### Sizing with routes (micro approach, edges on map, first estimator of travel time computed from maps and real trafic data)
Based on the results of "Sizing with adresses", "Sizing with routes" :
* Create a spatial segmentation of the territory seen as a collection of segments (streets)
* Compute the sizing
* Compute performance indicators

### Route planning optimisation
Based on the results of "Sizing with routes", "Route planning" :
* create itinerary and route planning for each "Sizing result"
* Recombine and iterate overs results to improve the global equilibrium
* Compute performance indicators
