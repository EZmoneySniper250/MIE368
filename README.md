# Toronto Fire Truck Optimization project

### Background and Problem Statement 

The fire incident is one of the most common and dangerous disasters that threaten people’s lives. In every city, the government always spent huge amounts of human and financial resources to solve it. The project is focused on making an optimization model on finding the minimum number of the required fire trucks for each fire station that can meet daily requirements of dealing with fire incidents happening in Toronto.

Data and Methods

The team used three datasets for the project: the fire incidents data, which contains the coordinates and dates of all fire incidents; the fire station data, which contains the coordinates of all fire stations; the fire run-areas data, which contains the geometry for all fire run-service areas. All data is for the City of Toronto in 2016 and 2017, downloaded from Toronto Open Data Catalogue.

Randomness of the locations of fire incidents will be justified first. Then classifications of each fire incident to its nearest fire area will be applied, by applying distance calculation based on Pythagorean theorem. Afterwards an optimization model will be implemented to minimize the total number of fire trucks that can meet the daily demand in each centroid in 2016, with decision variables of number of fire trucks needed in each station for distribution to its responsible fire area(s) every day, objective function on minimizing the total number of fire trucks needed in 2016, and constraints on all daily fire incidents of each fire area can be encountered. Then evaluations on the model based on fire incidents coverage of 2017 will be implemented. 

#Result and Conclusion

The fire incidents are all randomly distributed, with a Pearson correlation coefficient of 0.028 in Longitudes and 0.0084 in Latitude, between the coordinates of incidents of 2016 and 2017. The optimal total number of fire trucks needed for fully coverage of incidents that happened in 2016 is 157 fire trucks, 24 stations can be removed since they do not need to store any fire trucks in the station. By removing the stations and applying the optimization fire trucks to each station, 92.84% fire incidents of 2017 can be covered. The result of the optimization model can be applied to most of the situations and maximize the efficiency of fire trucks distributions of the City of Toronto. 
