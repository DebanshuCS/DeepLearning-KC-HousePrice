# DeepLearning-KC-HousePrice

The objective is to implement deep learning. 

I loaded the classification data, partitioned it based on requirements, trained it using neural networks and the results are plotted. I have used various network structures with various number of nodes in each hidden layers. 

The layers are analyzed based on various networks. Tensor flow has been used to train and use the deep neural networks.

Using Tensorflow, I have implemented sequential model which basically is appropriate for a plain stack of layers where each layer has exactly one input tensor and one output tensor.

A model with too little capacity cannot learn the training dataset meaning it will underfit, whereas a model with too much capacity may memorize the training dataset, meaning it will overfit or may get stuck or lost during the optimization process.

So, Added layer with 8 nodes and used 50% dropout to avoid overfitting in the model. One point to remember here is, Increasing the number of layers provides a short-cut to increasing the capacity of the model with fewer resources, and modern techniques allow learning algorithms to successfully train deep models.

Compiled the model with ADAM optimizer,This optimization algorithm is a further extension of stochastic gradient descent to update network weights during training. Unlike maintaining a single learning rate through training in SGD, Adam optimizer updates the learning rate for each network weight individually. 

And used MSE loss function, To calculate the MSE, you take the difference between your model's predictions and the ground truth, square it, and average it out across the whole dataset.

### loss graph:
![download](https://user-images.githubusercontent.com/118846871/212354256-3cd48305-bd4c-48b7-a149-6d579d8be58a.png)

## Dataset used: 
**kc_house_data.csv**

## Feature Columns:

id - Unique ID for each home sold

date - Date of the home sale

price - Price of each home sold

bedrooms - Number of bedrooms

bathrooms - Number of bathrooms, where .5 accounts for a room with a toilet but no shower

sqft_living - Square footage of the apartments interior living space

sqft_lot - Square footage of the land space

floors - Number of floors

waterfront - A dummy variable for whether the apartment was overlooking the waterfront or not

view - An index from 0 to 4 of how good the view of the property was

condition - An index from 1 to 5 on the condition of the apartment,

grade - An index from 1 to 13, where 1-3 falls short of building construction and design, 7 has an average level of construction and design, and 11-13 have a high quality level of construction and design.

sqft_above - The square footage of the interior housing space that is above ground level

sqft_basement - The square footage of the interior housing space that is below ground level

yr_built - The year the house was initially built

yr_renovated - The year of the house’s last renovation

zipcode - What zipcode area the house is in

lat - Lattitude

long - Longitude

sqft_living15 - The square footage of interior housing living space for the nearest 15 neighbors

sqft_lot15 - The square footage of the land lots of the nearest 15 neighbors
