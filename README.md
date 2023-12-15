# tutorial_mosqlimate
This repository exemplifies how the mosqlimate platform can register your model and save predictions.


All the codes in this repo were done based on the documentation of the [Mosqlimate Project](https://api.mosqlimate.org/docs/). 

In this repo, we will train a model to predict the dengue cases in Rio de Janeiro city using the data available in the Mosqlimate Project. To achieve it, we will use a simple univariate forecast based on neural networks implemented by [Neural Prophet](https://neuralprophet.com/contents.html). 

The objective of this tutorial is to provide a complete example of how the platform can be used. After following all the steps, we will be able to see your data in the Mosqlimate/vis as shown below: 



The first step is to clone this repo in your personal GitHub account. You can see an example of cloning a repository [here](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository). 
Also, it's necessary to create an account on the [platform](https://api.mosqlimate.org/). It's straightforward; you can log in with your own GitHub account. 

After creating an account, let's start to build the model. The first step is obtaining the notebook data: `get_data_from_mosqlimate.ipynb`. 

After that, run the notebook: `train_and_gen_predictions.ipynb`. In this notebook, we will run the model and generate the predictions that will be sent to the platform. 

Now that we have created our first prediction let's register or model using the `Post model in the database.ipynb` notebook. 

Now that you have registered your model let's send the first predictions using the `post predictions.ipynb` notebook.


After sending the predictions, you will be able to visualize your predictions in the platform as shown below: 

<img width="1397" alt="Captura de Tela 2023-12-15 às 10 55 20" src="https://github.com/eduardocorrearaujo/tutorial_mosqlimate/assets/65051489/f60cdd34-f2ec-4c0b-9985-52d985dd391f">


You can also go ahead and compare your predictions with others saved on the platform. To have access to a list of the predictions associated with a geocode, click on predictions as highlighted below and select the predictions from other models: 
<img width="1390" alt="Captura de Tela 2023-12-15 às 10 57 22" src="https://github.com/eduardocorrearaujo/tutorial_mosqlimate/assets/65051489/864ea0fb-d975-4e26-a97d-1c99a9782ce9">

After that, the predictions will be shown by gray lines in the left panel. Hovering with the mouse over one will highlight them in the left panel and display the prediction interval on the right panel:
<img width="1404" alt="Captura de Tela 2023-12-15 às 10 59 37" src="https://github.com/eduardocorrearaujo/tutorial_mosqlimate/assets/65051489/52138aec-2041-421d-954d-deb6f4e0b1a6">


If you want to retrieve the predictions on the platform as dataframes, look at the `retrieve_predictions.ipynb` notebook.

