A couple of notes: 

* Data for 2018 only goes through June. There is another data set for the full year. It provides some different information, but the IDs are different. I can match events based on date timestamp of the incident, but I'm not sure how consistently I'd be able to do so. Not sure the additional data is worth it. https://data.cityofnewyork.us/Public-Safety/Fire-Incident-Dispatch-Data/8m42-w767


Feature Engineering ideas: 

* Calculate response time -- done
* Calculate distance to nearest fire station -- done
* Calculate incident day of week -- To be completed (maybe identify trends)
* Are there other data sets we can bring in? Maybe inspired by Aditya's blog post? 
* Weather data? 

Analytic Questions: 

* Identify fireboxes (as representations of the regions of the city) where incidents are most likely to occur. High, Medium, Low Risk. This is similar to the "inspection prioritization" problem. I just don't think we have some of the other data (building condition data) that is described in the article. 

* Predict the response time (or may total incident duration) based on location, distance to fire station, number of units responding (or any other available features). 

* Identify when incidents are most likely to occur to inform staffing decisions at fire stations.
* Need to see if we can cluster
