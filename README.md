# tutorial_mosqlimate
This repository exemplifies how the mosqlimate platform can register your model and save predictions.


All the codes in this repo were done based on the documentation of the [Mosqlimate Project](https://api.mosqlimate.org/docs/). 

In this repo, we will train a model to predict the dengue cases in Rio de Janeiro city using the data available in the Mosqlimate Project. To achieve it, we will use a simple univariate forecast based on neural networks implemented by [Neural Prophet](https://neuralprophet.com/contents.html). 

The objective of this tutorial is to provide a complete example of how the platform can be used. After following all the steps, we will be able to see your data in the Mosqlimate/vis as shown below: 



The first step is to clone this repo in your personal GitHub account. You can see an example of cloning a repository [here](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository). 
Also, it's necessary to create an account on the [platform](https://api.mosqlimate.org/). It's really simple; you can log in with your own GitHub account. 

After creating an account, let's start to build the model. The first step is obtaining the notebook data: `get_data_from_mosqlimate.ipynb`. 

After that, run the notebook: `train_and_gen_predictions.ipynb`. In this notebook, we will run the model and generate the predictions that will be sent to the platform. 

Now that we create our first prediction let's register or model using the `Post model in the database.ipynb` notebook. 

Now that you registered your model let's send the first predictions using the `post predictions.ipynb` notebook. 



