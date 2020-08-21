# AI course project

## A. Objectives
1. Using Tensorflow, develop a feedforward neural network model for a classification or a regression problem using a pre-cleaned tabular dataset.
   1. NO time-series data, NO image data,  NO text data, only standard tabular data
   1. Data must have at least a 1000 rows and at least 3 input features (columns)
1. Compare the performance of your model with a basic single layer model. For a regression problem, your single layer model is a linear regression model, and for a binary classification problem, your single layer model is a logistic regression model.
1. Investigate "what", "how", and "why" your model makes predictions, and discuss your findings in your report.

## B. Expectations
1. You will work on your projects individually (i.e. group submissions are not allowed).
1. Reports for all phases (including the final report) must be prepared using <a href="https://www.overleaf.com/">Overleaf</a>. Non-overleaf submissions may not be graded at all. I do not provide any Overleaf templates, and you are free to use any templates you want.

## C. Phases
In each phase you are exepected to submit:
1. A link to your Colab notebook. Please test on your own (in a different browser) to make sure that anyone with the link can view your Python notebook. If I cannot access your notebook during grading you may loose points.
1. A PDF report describing your findings (downloaded from your Overleaf project).
1. A link to view your Overleaf project.

Below is the list of all phases and the outline of what you will be working on in each phase. 

### Phase I. Data analysis & preparation
1. Description of the dataset, its source, and motivation for the project
1. Visualize/Plot the distribution of each input features and discuss the range of the values (min, max, mean, median, etc.)
   - For example, plot histograms showing distribution of each input features
1. Study the distribution of the output labels
    - In case of classification, check if the data is imbalanced
    - In case of regression, check if the values are uniformly distributed or not
1. Data normalization

**What to submit?**  
a) 
b) A PDF report describing your findings  

### Phase II. Model selection & evaluation
1. Split the data into training, and validation sets
1. Compare the results of the neural network with a linear regression or logistic regression model
    - Start with a basic model and then grow your model into a multi-layered model
    - Discuss how neural network models will be selected
    - Document your performance comparison
1. Study performance difference when linear activation is used instead of sigmoid (and vice versa)
   - How does your performance change when linear activations are used instead of sigmoid, in the last neuron and all other neurons?
     ```python
     # Change 'relu' to 'linear' and 'sigmoid' in the layers below
     model = Sequential()
     model.add(Dense(9999, input_dim = len(X[0, :]), activation='relu'))
     ...
     model.add(Dense(9999, activation='relu'))
     ```
1. Plot your learning curves and include them in your report
1. Discuss what architecture (how big) you need to overfit the data
1. Discuss what architecture (how big) you do need to overfit when you have output as additional input feature
1. Evaluate your predictions (using Precision, Recall, MAE, MSE, etc.)
1. [OPTIONAL] Code a function that represents your model
   - After your model is trained, read all the weights, and build your own function/method that serves as the model
   - Verify that predictions you obtain are same as the one you obtained using your trained model

**What to submit?**  
a) A link to your Colab notebook (make sure that anyone with the link can view)  
b) A PDF report describing your findings  

### Phase III. Feature importance and reduction
1. Study feature importance by iteratively removing input features
1. Identify non-informative input features and remove them
1. Compare your feature-reduced model with the original model with all input features

**What to submit?**  
a) A link to your Colab notebook (make sure that anyone with the link can view)  
b) A PDF report describing your findings  

## 4. Address peer-review comments
* You will receive comments/reviews from at least two peers in the classroom

**What to submit?**  
a) A PDF report describing the comments you received and how you addressed them  

### Phase IV. Report
**What to submit?**   
1. A copy of your final report    
    * Your report must not be very long; 10/12 pages at most.
    * All tables and figures must be numbered and captioned/labelled.
    * Don't fill an entire page with a picture or have pictures hanging outside of the page borders.
    * It is encouraged but not required to you host your project (and report) at Github.  
    * Turn off the dark mode in Notebook before you copy images/plots (the lables and ticks are hard to see in dark mode).
1. A link to your final Notebook

~~##5. Poster presentation (final exam)~~
* Prepare a poster highlighting the problem, diagrams, your results, plots, etc.
* Poster and final report will be evaluated based on all the criteria above.
* Report and poster presentation grades will be average of (a) grades by the course instructor (b) peer grades, and (c) grades by external visitor/s from industry
* See sample-reports folder and sample-posters folder for samples

**What to submit?**  
a) A copy of your final report  
b) A link to your final Notebook

**What to bring?**  
a) A printed copy of your final report  
b) A link to your final Notebook
c) Your poster  
d) A laptop for demonstration (if needed)  

## D. Sample student projects (from previous semesters)
* EPL game result prediction by Bikash Shrestha - [report](https://github.com/badriadhikari/AI-2020spring/blob/master/sample-reports/sample-report-1.pdf)
* Prediction of housing prices by Syeda Afrah Shamail - [report](https://github.com/afrah1994/Prediction-of-Housing-Prices/blob/master/Final%20report.pdf)
* Factors in tennis by John Soderstrom - [report](https://github.com/SoderstromJohnR/CS4300Final/blob/master/Final%20Report.pdf)
* Predicting pulsar stars by Duc Ngo - [report](https://github.com/zegster/artificial-intelligence/blob/master/final_assembly/Final_Assembly.pdf)

