Analysis:

Overview:

The purpose of this analysis was to use our knowledge of deep learning to create a tool that would help the Alphabet Soup foundation select applicants with the best chance of success in their ventures. In doing so we were given a csv that contained over 34 thousand organizations that have previously received funding.

Results:

- Data Processing:
  - What variable(s) are the target(s) for your model?
    -  The target variable for my model is the "IS_SUCCESSFUL", either having a value of 1 indicating a success and a 0 indicating a non-success.
  - What variable(s) are the features for your model?
    - In this model, the "EIN" and "NAME" columns were dropped, and the remaining columns were the features for the model (APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT). 
  - What variable(s) should be removed from the input data because they are neither targets nor features?
    - The "EIN" and "NAME" variable(s) were removed. 


- Compiling, Training, and Evaluating the Model:
  - How many neurons, layers, and activation functions did you select for your neural network model, and why?
    - I used 2 hidden layers with 7 and 14 neurons in my first attempt because I wanted small numbers for my first try, for my second attempt I used 2 hidden layers with 25 and 50 neurons respectively, in my third attempt I used 3 hidden layers with 25, 50, and 75 neurons respectively and then finally ended with 4 hidden layers at 25, 50, 75, and 100 neurons. I did this because after the first attempt, I figured out the number of neurons didn't significantly impact my load times, and so for my further attempts I wanted to go up in increments of 25 until I reached 100 neurons total.
  - Were you able to achieve the target model performance?
    - I was not able to achieve the target model performance, I always hovered around 73%. 
  - What steps did you take in your attempts to increase model performance?
    - I added more hidden layers in each attempt, I also adjusted the amount of epochs down from 100 to 25, before going back up to 30, I also edited the validation split between attempts.


Summary:

