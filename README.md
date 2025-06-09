# UsedCarPrice
What drives the Price of  Car?
A dataset of used vehicles from Kaggle was used with 426,000 cars to perform a regression analysis to provide sugestions to the client (used car dealer).
## Introduction

The goal is to understand what factors make a car more or less expensive. The results of the analysis provides clear recommendations to a client -- a used car dealership -- as to what consumers value in a used car.  The data contains variety of vehicles with the following features:

* region 
* price  
* year
* manufacturer 
* model 
* condition 
* cylinders 
* fuel 
* odometer
* title_status 
* transmission 
* VIN 
* drive 
* size 
* type 
* paint_color
* state   

The application of regression models was used to come up with insights that help guide a client.

## Technology Used

* python
* Jupyter Notebook
* sklearn libraries within python
* Matplotlib for charts and images
* pyvin a library that correlates a vehicle vin number to features

## Approach

Data was cleaned to remove outliers and unnecessary columns and null values.  Vehicles were then separated into categories of the following:

* Pickup
* Coupe
* SUV
* Sedan
* Convertible
* Truck
* Hatchback
* Wagon
* Van
* Mini-Van
* Offroad
* Bus
          
The models applied on the above vehicle types were Linear Regression, Ridge Regression, and Lasso Regression.

Examples of regression models on each vehicle type:

![image](https://github.com/user-attachments/assets/7d42baba-0191-4aa4-88e4-8c865f379c50)

Example of regression analysis:

![image](https://github.com/user-attachments/assets/6d789585-a661-40d2-9038-818f19e1d1f3)

![image](https://github.com/user-attachments/assets/bf6ba57e-af96-4447-926c-4d2fe8f148a2)

![image](https://github.com/user-attachments/assets/618a0b14-8a08-4aca-b2bd-01766aec202c)



## Suggestions to the client

a) The main features that impact the price of the vehicle are the vehicle age and the odometer reading. Pickups, Vans, Mini-Vans, and Offroad vehicles seem to depreciate the fastest with age. Convertibles and buses seem to be impacted more by the odometer reading. Additional top three features that impact price:

-Pickups: Transmission, size, and fuel type
-Vans: Model, transmission and size
-Mini-Vans: Fuel type, transmission, and drive
-Offroad:  Model, State, and size
-Sedans: Model, transmission, and fuel type
-Convertibles: Fuel type, Model, and transmission
-Trucks: Model, age, and transmission
-Hatchback: cylinders, fuel type, and drive
-Wagon: transmission, model, and fuel
-Bus: transmission, model, and cylinder
-SUV: Model, transmission, and fuel type
-Coupe: Fuel type, transmission, and drive

Maintaining the appropriate inventory of the vehicles based on the important features that impact the price will help sell the vehicles at a higher price. Vehicle age and odometer reading are the key features overall. Trucks have the best correlation of odometer reading to the price.

b) There is a more reliable price prediction based on the available inventory for hatchbacks, vans, pickups, convertibles, trucks, and minivans which may suggest faster sales cycles.

c) Pricing on new unknown inventory can be better predicted for wagons, hatchbacks, and sedans.

d) The next steps will be to fine tune the appropriate attributes within the features that impact the pricing.
