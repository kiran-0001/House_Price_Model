# Research Background
## Note: This project was supervised under Dr. Elahe Javadi of the Illinois State University College of Applied Science and Technology 

> Real estate requires meticulous prediction ability from individuals involved, as especially now, in the current saturated market state, it is more important than ever to pose accurate predictions to clients. 
> My research question deals in this sector by bringing to light the effect of different optimizers on neural network prediction outputs.
> In addition, we examine how these said optimizers affect the models functionality as a whole.
***
> Regarding Optimizer Functions:
>
> - 'SGD'
> - 'Adam'
> - 'ftrl'
>
> We will be examining the above three optimizers for the purpose of this study.
***
### Neural Schema for Experiments 
>
> For each model, there will be exactly ten inputs relating to building attributes such as square footage. 
>
> In addition, there will be exactly two hidden layers  using relu activation, with thirty-two neurons each.
>
> The output layer will access the sigmoid function and will utilize one neuron.
>
> This architecture will remain constant for all experimentation.
>
>
> <img width="445" alt="HousePriceModelNueralArchitecture" src="https://user-images.githubusercontent.com/121153158/212488850-0983db89-d4b7-4c2c-911c-95eefd7fb11d.png">
***
### Procedure
> For each neural network, the variable optimizer will be changed according to the prior mentioned test optimizers. 
>
> Soon after, two graphs showcasing the effects on the model will be generated and then interpreted.
>
> The visualization will showcase the models loss and accuracy in real time as the network runs. 
***
### 'Adam'
<img width="479" alt="Adam" src="https://user-images.githubusercontent.com/121153158/212489828-acb2ce6c-048d-451e-b3a9-fba3d12312bb.png">

We see here that the model accuracy between training and validation is closely mirrored indicating an accurate model with low overfitting.
When examining model loss, we see that validation losses level off higher than training losses, indicating discrepancies with unseen data.
***

### 'SGD'
<img width="444" alt="SGD" src="https://user-images.githubusercontent.com/121153158/212490108-90675449-d461-4f94-8655-2dadb7ee46c5.png">

We see here that the model accuracy between training and validation is closely mirrored although separate slightly towards its end, this may indicate minimal overfitting.
When examining model loss, we see that training losses level off higher than validation losses, indicating discrepancies with training data.
***

### 'ftrl'
<img width="470" alt="ftrl" src="https://user-images.githubusercontent.com/121153158/212490147-47260df0-ef9a-45d3-8a0f-78d6d2e3d618.png">

Needless to say, this model does not provide discernable results for this particular purpose.
This may be due to incompatibility with the utilized dataset, and is a result of stagnation as iterations are run.
***

# Findings 
> At the conclusion of these experiments, we find that real estate agents, and individuals involved, would fare better using the ‘SGD’ optimizer for median house data predictions.
>
> This choice is favorable as, based on the data, it results in outputs that indicate lower overfitting and better predictions overall.
>
> Concerning the two other optimizers:
> - ‘Adam’ does an acceptable job with this dataset, although it outputs lower accuracies overall, which is not favorable for the purpose of the network
> - ‘Ftrl’ outputs results that are simply of no use, as the model portrays significant stagnation unacceptably low accuracies

