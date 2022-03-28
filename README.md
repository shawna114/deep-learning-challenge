# deep-learning-challenge
## 1. Overview: 
Using my knowledge of TensorFlow, I designed a neural network to create a binary classification model that can predict if an Alphabet Soup–funded organization will be successful based on the features in the given dataset. Considerations included how many inputs there should be, and determining the number of neurons and layers in the model. I then compiled, trained, and evaluated my binary classification model to calculate the model’s loss and accuracy.

## 2. Results
My final optimized model did not meet > 75% accuracy despite making several attempts to adjust dataset and model parameters. Despite not meeting goal accuracy, my final model outperformed my initial model.


### Data Preprocessing
* Target Variable: The 'IS_SUCCESSFUL' column
* Model Features: All dummy variables created from original columns
* Variables that are neither targets or features: 'NAME' and 'EIN' columns
### Compiling, Training, and Evaluating the Model
<b>How many neurons, layers, and activation functions did you select for your neural network model, and why?</b>
For my optimized model, I used Keras Tuner (results shown below).
   ![Image1](https://github.com/shawna114/deep-learning-challenge/blob/main/Resources/Images/KerasTuner.png)
    
<b> Were you able to achieve the target model performance? </b>
No, I wasn't able to achieve target model performance.
     
<b>What steps did you take to try and increase model performance?</b> I completed the following steps in attempts to improve performance:
* Removed 'ASK_AMT' column
* Adjusted buckets (this didn't impact numbers significantly, so I changed back to original)
* Tested 'swish' for activation (changed back to relu after running Keras Tuner)
* Tested the addition of hidden layers (adjusted to 6 after running Keras Tuner)
* Tested increasing epochs to 100 (adjusted to 20 after running Keras Tuner)
* Utilized Keras Tuner to select ideal hyperparameters

## 3. Summary: 

Overall, I was able to improve the model's performance, despite not meeting the target goal. If I were to continue troubleshooting the model I would look deeper into the data to identify if there were any outliers that may be throwing the model off and also look into alternate activation options.
