# 2021_IBM_Code_Challenge_ORBITERS
A number of challenges like climate change and crop diseases pose hindrance to sustainable agricultural practices which are of great significance for global crop production. To meet these challenges and warn growers of possible threat it is essential that the recommendations provided to them are efficient, correct and based on outcomes from scientific studies.

We have designed a system that can provide early disease detection in fields that are difficult to survey manually, using image processing of multispectral satellite imagery along with the best possible solutions and guidance provided to farmers by an ML model. All the farmer has to do is to enrol himself with our website and share with us his location and contact details.

Farmers will receive an early disease warning with the types of diseases that could possibly infest their crop area along with the fertilizers they could use to effectively prevent these diseases from occurring.

The main advantage of using satellite images is to locate vulnerable crops in larger areas that are difficult to survey manually and can be affected by more than a single crop variety. These images are acquired via Google Earth, USGS Earth Explorer and SNAP (Sentinels Application Platform). 

We have processed multispectral satellite images to locate patches of vulnerable crop land via NDVI (Normalized Difference Vegetative Index) analysis after which these areas were compared with their corresponding temperature, humidity and rainfall heat maps. This is based on the concept that diseases occur when the crops are exposed to prolonged period of certain weather conditions and different diseases need different combination of weather parameters to occur on a given crop type. Hence an early disease warning is raised for the diseases that are likely to start showing up on identified vulnerable crop area.

Next we have created an ML model that takes the same weather parameters and some additional information from farmers to predict the most optimal solution to help farmers prevent these diseases at a much earlier stage.
