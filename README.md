</p>
<h1 align="center">
  Eagle-AI-GUI
</h1>
 <h3 align="center">
  GUI for Machine-Learning Algorithms
</h3>
 
</p>
<br>
<p align="center">
  <a>
    <img src="./eagle2.png"/>
  </a>
  </p>
<br>

## Intended audience
  This application is made for learners to visualize how changing different hyper-parameters could affect accuracy of the model.
  This applications is can also be used for selecting the base model of a large project
  
## Installation
  **Step-1:** Download and extract the files
  
  **Step-2:** <a href='https://uoa-eresearch.github.io/eresearch-cookbook/recipe/2014/11/26/python-virtual-env/'>Create a virtual enviroment</a>(optional)
  
  **Step-3:** open the path where files are extracted in terminal
  
  **Step-4:** type *pip install -r requirements.txt* and hit enter in terminal
  
  **Step-5:** type *python main.py* and hit enter to start the application
  
# Note->In windows application may show not responding, just leave it idle for few seconds  
  
## Usage Guide
* <ins>**Linear Regression**</ins>

  **Sample file is in samples/Linear Regression directory**
  
  
  **Step-1:** This is first screen that will appear when the program is executed, load in your Training set, DEV set and Test set and press initialize.
  
    <a>
    <img src="./img/1.png" width="300" height ="300"/>
  </a>
  
    **Note->**
    * **You must load in only .csv, .xls or .xlsx file** 
    * **Columns of the file uploaded will be used as parameters(features)**
    * **Column of one is added by the application and it should not be present in original file**
    * **It is considered a good practice to have different test and Dev(cross validation) set but same file can be uploaded in both**
    * **Normalization is applied automatically by the application**

    
    
  **Step-2:** After Initialization this screen will appear, from the dropdown list choose "Linear Regression" fill in the *hyper parameters* than
    press *START TRAINING*.
    
    <a>
    <img src="./img/2.png" width="500" height ="200"/>
    </a>

    **Progress Bar below "START TRAINING" button denotes the progress in model training.**
    
    **Step-3:** After the training is finished a pop-up message will appear stating the successfull completion of model training. 
    
    To save the model press *SAVE MODEL* this will export three files one containing parameters and other two containing normalization factors
    
    <a>
    <img src="./img/3.png" width="500" height ="200"/>
    </a>
 
* <ins>**Logistic Regression**</ins>
 
  **Sample file is in samples/Logistic Regression directory**
  
  **Step-1:** *Same as in Linear Regression*
  
  **Note->**
    * **You must load in only .csv, .xls or .xlsx file** 
    * **Columns of the file uploaded will be used as parameters(features)**
    * **Column of one is added by the application and it should not be present in original file**
    * **It is considered a good practice to have different test and Dev(cross validation) set but same file can be uploaded in both**
    * **Normalization is applied automatically by the application**
    * **Multi-Class classification is not supported(currently) so y column should have only zeros or one**
    
  **Step-2:** After Initialization this screen will appear, from the dropdown list choose "Logistic Regression" fill in the *hyper parameters* than
    press *START TRAINING*.
    
    <a>
    <img src="./img/4.png" width="500" height ="200"/>
    </a>
    
   **Step-3:** After the training is finished a pop-up message will appear stating the successfull completion of model training. 
    
    To save the model press *SAVE MODEL* this will export three files one containing parameters and other two containing normalization factors
    
    <a>
    <img src="./img/5.png" width="500" height ="200"/>
    </a>
    
* <ins>**Deep Neural Network**</ins>
  **Sample file is in samples/Deep Neural Network directory**
  
  **Step-1:** *Same as in Linear Regression*
  
  **Note->**
    * **You must load in only .csv, .xls or .xlsx file** 
    * **Columns of the file uploaded will be used as parameters(features)**
    * **Column of one is added by the application and it should not be present in original file**
    * **It is considered a good practice to have different test and Dev(cross validation) set but same file can be uploaded in both**
    * **Normalization is applied automatically by the application**
    * **Multi-Class classification is not supported(currently) so y column should have only zeros or one**
    * **Currently only a three layered neural network is supported**
    
  **Step-2:** After Initialization this screen will appear, from the dropdown list choose "Logistic Regression" fill in the *hyper parameters* than
    press *START TRAINING*.
    
  **Note->**
    * **optimizer takes in value *gd* for Gradient Descent, *momentum* for GD+momentum and *adam* for Adam optimization.**
    * **hyper parameter *Beta* is for momentum optimization with default value=0.9(leave it empty for other optimizations)**
    * **hyper parameters *Beta1* and *Beta2* are for Adam optimization with default value=0.9,0.999(leave it empty for other optimizations)**
    * **example for layer input *5,2,1* last layer(output layer) should be 1 and each layer should be seperated by comma**
    
    
    <a>
    <img src="./img/6.png" width="500" height ="200"/>
    </a>
    
  **Step-3:** After the training is finished a pop-up message will appear stating the successfull completion of model training. 
    
    To save the model press *SAVE MODEL* this will export three files one containing parameters and other two containing normalization factors
    
    <a>
    <img src="./img/7.png" width="500" height ="200"/>
    </a>
