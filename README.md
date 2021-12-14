# NYC_Taxi
Analyzing New York City Taxi Dataset

## Dataset:
You can download the NYC taxi dataset from the link http://www.andresmh.com/nyctaxitrips/ then take
a sample from it. Each row of the file after the header represents a single taxi ride in CSV format. For
each ride, we have some attributes of the cab (a hashed version of the medallion number) as well as the
driver (a hashed version of the hack license, which is what licenses to drive taxis are called), some
temporal information about when the trip started and ended, and the longitude/latitude coordinates for
where the passenger(s) were picked up and dropped off.

### We are mainly interested in each Trip's:
- Some Unique ID for the car (license)
- Pick-up location
- Pick-up time
- Drop-off location
- Drop-off time

## Problem:
We need to compute one important statistic utilization. Utilization is the fraction of time that a cab is on
the road and is occupied by one or more passengers. One factor that impacts utilization is the
passenger's destination: a cab that drops off passengers near Union Square at midday is much more
likely to find its next fare in just a minute or two, whereas a cab that drops someone off at 2 AM on Staten Island may
have to drive all the way back to Manhattan before it find its next fare.
We need to compute:

1. The average time it takes for a taxi to find its next fare(trip) per destination borough,
2. The number of trips that started and ended within the same borough,
3. The number of trips that start in one borough and ended in another one
4. 
