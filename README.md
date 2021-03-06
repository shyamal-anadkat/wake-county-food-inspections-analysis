# Predictive Analytics with Wake County Restaurant Inspections 

### AIPI510 | **Shyamal Anadkat, Christine Park, Hearsch Jariwala**

### Building a model to predict restaurant inspections with higher than average critical violations.

![image](https://user-images.githubusercontent.com/12115186/157798475-450379ac-2342-48bd-a6c8-c89332dffe04.png)


---

## Getting Started:

**The main notebook is `WakeCountyRestaurantInspectionsMain.ipynb`. This should be the one you should work on & execute. Make sure to uncomment the pip installs in the first cell to ensure you have the relevant packages installed. All the data needed to execute the notebook should be be `/data` directory. Here's more on the structure of the project:**

---
* **Final Presentation: `PresentationFinal.slides.html`**
* `/data` : preprocessed data that is being used in the main notebook
* Final Presentation Jupyter notebook:  `PresentationFinal.ipynb`
	* To convert the notebook into html artifact to render it use this command: 
	`jupyter nbconvert PresentationFinal.ipynb --to slides --TagRemovePreprocessor.remove_input_tags={\"to_remove\"}` 
	Note that the tag `to_remove` is added to code cells with plots where we want to 
* `/datasheets`: datasheets for datasets 
* `/notebooks`: all ipynb notebooks

All our data is sourced via public, authenticated APIs. We have sourced the following data: restaurant inspections, restaurant food & safety violations, weather data, proxy for crime data, yelp data around restaurants, and the official Wake County restaurant data. The respective jupyter notebooks for sourcing & processing data from the 6 datasets are within `/notebooks`: 

1. `CrimeDataAnalysis.ipynb`: Sourcing daily police incidents as proxy for crime from Wake Gov
2. `RestaurantDataAnalysis.ipynb` : Sourcing data around restaurants from Wake Gov
3. `RestaurantInspectionsAnalysis.ipynb`: Sourcing Restaurant Inspections Data from Wake Gov
4. `WeatherDataAnalysis.ipynb`: Sourcing Weather Data from NOAA
5. `YelpDataAnalysis.ipynb`: Fetching Yelp data around restaurants via Yelp Fusion search by business & phone. We are fetching by restaurant phone first and falling back to name if phone is invalid/absent on a record.
6. `YelpLIVESAnalysis.ipynb`: Fetching Yelp LIVES analysis to get the scoring grade. We did not end up using this data.
---

### Architecture:

![image](https://user-images.githubusercontent.com/12115186/157798330-44a4324f-bb88-415b-aeb5-e51a0e85f74a.png)

### Results

![image](https://user-images.githubusercontent.com/12115186/157798541-4559fa74-db63-449b-b252-2fee77546343.png)


### Evaluation

![image](https://user-images.githubusercontent.com/12115186/157798570-34141f67-1ad9-4258-ad5b-24641c109fa7.png)



*Please read ethical, privacy, and legal considerations at the bottom of `WakeCountyRestaurantInspectionsMain.ipynb`. The datasheets are within `/datasheets`*

Hope you like it! Questions/Suggestions: please reach out to sha18@duke.edu
