# Changelog

## Week 1
- Cloned repo; set up a VS Code notebook (`data_exploration.ipynb`) on Python 3.11.5.
- Pulled NHTSA owner complaints through the public API for 12 US-market cars,
  summarized top complaint categories and an engine/power train share (`data/car_summary.csv`).
- Chose the car list from the hero cars of The Fast and the Furious (2001), 2 Fast 2 Furious (2003)
  and Tokyo Drift (2006). 3 of the 15 were never sold in the US, so NHTSA has no data on them.
- Found that NHTSA data is noisy: in the RSX 2002 sample, 73 of 93 complaints passed a VIN/text check
  and 20 did not. Plan: label match confidence instead of deleting.
- Tested NHTSA's bulk file for mileage. Only about 4 in 10 rows had one, so we dropped mileage.
- Parked: complaints per 10,000 sold, severity of engine issues, age at incident.

### Feedback incorporated
- Professor: focus on the data and the model's recommendations, not the front end.
  Change: the 90s-website chat UI is now an optional stretch goal.