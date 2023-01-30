# deeplearning-decadalworldeconomy
Deep learning for forecasting decadal world economy

Wang, T., Beard, R., Hawkins, J., & Chandra, R. (2023). Recursive deep learning framework for forecasting the decadal world economic outlook.
https://arxiv.org/abs/2301.10874

# project (Forecast next decade's GDP using DL model)

Time series forecasting project for multiple country GDP data using
additonal economic variables.

## Data

Raw datasets can be found inside the directory [Year data P](Year data P).
Each country inside its own directory.
Originally downloaded from pennworld [ADD A LINK HERE]()

## Baseline Models

The Vector Autoregression (VAR) models can be found inside the [VAR directory](VAR).

Each country is executed from its own notebook.


## Deep Learning Models

The series of deep learning models are created and tested for all countries inside the 
Notebook: **shuffled 53**. These models take 5 time steps of input and produce 3 steps
of output
  
The Notebook **multi parallel** uses the predicted data in a recursive manner to predict 
GDP growth rate until 2030


### Instructions

TianYi: I am adding some files and documenting here what I have done to reproduce your results
please correct anything that I have gotten wrong

1. Ensure you have [Jupyter installed](https://jupyter.org/install)


2. Install required additional python packages (Note this can take a while):
```
pip install -r requirements.txt
```

3. Launch the Notebook [shuffled53.ipynb](shuffled53.ipynb)
```
jupyter notebook shuffled53.ipynb
```
 
4. Run all the cells in the Notebook. The overall analysis and plots of each model for each country
will be placed inside the [results](results) directory.


5. Run the Multi parallel notebooks for the long term forecast
```
jupyter notebook multi\ parallel.ipynb
```



