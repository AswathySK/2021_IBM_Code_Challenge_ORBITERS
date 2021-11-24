# 2021_IBM_Code_Challenge_ORBITERS
A number of challenges like climate change and crop diseases pose hindrance to sustainable agricultural practices which are of great significance for global crop production. To meet these challenges and warn growers of possible threat it is essential that the recommendations provided to them are efficient, correct and based on outcomes from scientific studies.

We have designed a system that can provide early disease detection in fields that are difficult to survey manually, using image processing of multispectral satellite imagery along with the best possible solutions and guidance provided to farmers by an ML model. All the farmer has to do is to enrol himself with our website ( https://aswathyskumar144.wixsite.com/agribiters/rice through which the farmer can access the form http://5526-116-68-75-149.ngrok.io/try.html ) and share with us his location and contact details.

Farmers will receive an early disease warning with the types of diseases that could possibly infest their crop area along with the fertilizers they could use to effectively prevent these diseases from occurring.

The main advantage of using satellite images is to locate vulnerable crops in larger areas that are difficult to survey manually and can be affected by more than a single crop variety. These images are acquired via Google Earth, USGS Earth Explorer and SNAP (Sentinels Application Platform). 

We have processed multispectral satellite images to locate patches of vulnerable crop land via NDVI (Normalized Difference Vegetative Index) analysis after which these areas were compared with their corresponding temperature, humidity and rainfall heat maps. This is based on the concept that diseases occur when the crops are exposed to prolonged period of certain weather conditions and different diseases need different combination of weather parameters to occur on a given crop type. Hence an early disease warning is raised for the diseases that are likely to start showing up on identified vulnerable crop area.

Next we have created an ML model that takes the same weather parameters and some additional information from farmers to predict the most optimal solution to help farmers prevent these diseases at a much earlier stage.

The dataset  used for fertilizer prediction consists of the attribute features Temperature, Humidity, Moisture, Soil Type, Crop Type, Nitrogen, Potassium, Phosphorous.The attributes Soil Type and Crop Type are categorical features and we have used One Hot Encoding to Encode these categorical features as a one-hot numeric array. The Temperature, Humidity and Moisture values are obtained from Image Processing. A Random Forest Classifier is used for the model. A random forest is a meta estimator that fits a number of decision tree classifiers on various sub-samples of the dataset and uses averaging to improve the predictive accuracy and control over-fitting. Here the parameters used for the classifier are n_estimators = 100 ,which is the number of trees in the forest ; criterion = 'gini' ,which is the function to measure the quality of a split. “gini” is for the Gini impurity ; random_state= 42, which Controls both the randomness of the bootstrapping of the samples used when building trees. The best suited fertilizer for the crop according to the habitat conditions is suggested as output by the ML Model.

INDIVIDUAL CONTRIBUTIONS:

1, Ananya KV
2, Reshma Santhosh S

Image processing:
NDVI Analysis, Heat map inference from weather data, Road to automation

3, Govind S
4, Sreelakshmi P

ML Model for fertilizer prediction (Random forest model)

5, Aswathy S Kumar

Website (HTML,Database)
