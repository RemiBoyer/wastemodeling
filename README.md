# Waste modeling tools
For people and org who collect and treat the massive amount of garbage produce by our societies

## Concept and history
When you have to organize the waste collection and the waste treatment of a territory, you have to :
* estimate the waste production,
* find one or many efficient way of manage the processes to collect and treat
* submit your proposed solutions to all stakeholders (your boss, the local authority, inhabitants and the workforce)
* Choose the right way to do
* Implement this on the field with final success and intermediary ridiculous failure (leading to some cool war stories to brag with your children)
* Monitor the daily routine
* Evaluate and go back the first step (continious improvement)

This work is derived from my first big job as civil servant and from an another worl in a now defunct SaaS startup.
As my work was along the way massively funded by public money, I feel today the need of giving back (on my free time, so I don't know if this repository will be useful someday).

## Needs
### You must gather and make computable an accurate knowledge of your territory
* Relevant data > fresh data > big data 
* Don't forget trends to tackle the freshness problem
* Accuracy is a sin I had (and I think I still have it)

### You must measure today waste
How do you know ?

### You must have some hypothesis for your future master plans
Do you want to :
* have a workforce ?
* collect each adress on a door to door route or do you want to ask inhabitants to brig their garbage in dedicated places ?

## Solution
### The waste production modeling
* The purpose is to estimate the weight and the volume of the waste
* for each material: Annual Production = ( (Number of Person x annual material reject per person) + the famous organization estimator + the famous "popping waste" estimator
* At the glance, linear models with magical ratio extracted from data describing the current state
* Complicated and complex refinement will be fin

### The waste collection modeling
* The purpose is to estimate the feasability and the cost of a **collect** setup (given in parameter) 
* You will define your collect setup through :
  * means (workforce, trucks, pipelines, boxes and bins, ...)
  * geospatial and time definition : area, various zone, collect point, picking point, work duration, weekly planning, ...)
* You will simulate the waste collection process, in a simplified manner
* Given the simulation, you will compute performance indicator to describe the outcome (as a "loosy forecast")
* Given the knowledge provided by your modeling, you will find bottleneck and you will make new model, optimizers, to find the best scenario

You can read more about the waste collection modeling [on the collect page](./collect.md)

### The waste treatment modeling
* The purpose is to estimate the feasability and the cost of a **treatment** setup (given in parameter) 
* You will define your treatment setup through :
  * means (workforce, factories, processes (digestion, incineration, ...)
  * geospatial and time definition : area, various zone, treatment point, destination for second life of materials) ...
* You will simulate the waste treatment process, in a simplified manner
* Given the simulation, you will compute performance indicator to describe the outcome (as a "loosy forecast")
* Given the knowledge provided by your modeling, you will find bottleneck and you will make new model, optimizers, to find the best scenario
