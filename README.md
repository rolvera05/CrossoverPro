# *CrossoverPro*

This application showcases an elegant and efficient simple moving average (SMA) crossover strategy for trading stocks, leveraging the power of historical data. Driven by the growing demand for effective and data-driven trading strategies, this project aims to empower users to make well-informed decisions when it comes to entering and exiting positions. By harnessing the potential of reliable technical indicators, the project allows users to capitalize on market trends with greater confidence.

To facilitate a comprehensive evaluation of the strategy's performance, the project employs a range of essential metrics. Our main metric involves short SMA/long SMA in conjunction with signal/position data to determine SMA crossovers. Other metrics include cumulative returns, sharpe ratio, and sortino ratio. By providing users with insightful and actionable information, this application serves as a valuable tool for traders seeking to optimize their investment strategies and stay ahead of the curve in today's dynamic financial markets.

---

## *Technologies*

- **Programming Language:** Python
- **Libraries:** Pandas, Numpy, Plotly, Yfinance, IPython, Voilà, Ipywidgets
- **Framework:** JupyterLab
- **Operating Systems:** Mac OS, Microsoft Windows

---

## *Installation Guide*

**First things first:**
If you don't have Python, JupyterLab, or Anaconda installed on your operating system:

-**[Install Python](https://www.python.org/downloads/)**

-**[Install JupyterLab](https://jupyter.org/install)**

-**[Install Anaconda](https://docs.anaconda.com/free/anaconda/install/index.html)**

With the Anaconda package installed, you should already have all the necessary libraries to run the main application downloaded except for yfinance and voilà. For this section, all listed commands should be executed in your operating system's terminal.

**1. Install yfinance** 
        
        pip install yfinance
To confirm yfinance installation:
    
        conda list yfinance
You should get an output that looks like this, confirming installation: 

![Screenshot 2023-05-11 at 8 49 56 AM](https://github.com/djohnst914/github_upload/assets/123714457/92e40184-b2e6-47f5-8182-9d4fc5a3cda7)

**2. Conda 'dev' Environment** - To run the main application you will need to activate a 'dev' environment in your terminal. Luckily a 'dev' environment is included with the Anaconda package, and can be activated with:

        conda activate dev

If you do not have a 'dev' environment, or wish to create a new one that will be compatible with this application, type and enter the following. You will still use the previous steps' command to activate:

        conda create -n dev python=3.7 anaconda

**3. Install Voilà** - To install voilà first activate your 'dev' environment following the 1st step of step 2 above. After, run the following. Confirm installation with 'conda list' if needed after command below:

        conda install -c conda-forge voila

**3. Other Libraries** - It was mentioned earlier that the other required libraries should already be installed with the Anaconda package. To confirm installation for these libraries, you can either use the 'conda list' command followed by the library name to confirm installation same as for yfinance listed above. Or, you can install the libraries which will either install successfully or if already installed, will result in a 'requirement already satisfied' message. Listed below are the commands to install each library if needed:
        
        pip install pandas
        pip install numpy
        pip install plotly

**5. Clone Repo** - Once you have checked off all previous installation steps, its now time to clone/download this repository onto your local machine for use. To do that, first copy the SSH keys which can be found here: 

![Screenshot 2023-05-11 at 11 58 06 AM](https://github.com/djohnst914/github_upload/assets/123714457/5b1345a7-5f71-495e-9175-72c2a43c5ed8)

Now, in your terminal cd to a location where you want this repo folder to reside. We recommend choosing your desktop as the location due to it's easy access/simple path. Once you are in your preferred current directory, enter the following:

        git clone git@github.com:rolvera05/CrossoverPro.git

Nicely done! You now are ready to utilize the code. To run the repo folder in JupyterLab for usage, simply cd to the repo folder, then type and enter:

        jupyter lab

### **IMPORTANT:** Ensure your conda 'dev' environment is activated before running the 'jupyter lab' command. Otherwise, the application will most likely result in errors when you try to run it: 

![Screenshot 2023-05-11 at 10 05 53 AM](https://github.com/djohnst914/github_upload/assets/123714457/9ade3985-91ac-4940-a429-ec157ecfadf1)


---

## *Usage*

### 1. User Input
- Once JupyterLab is open with the repo code, the first thing you will do is open the user_input.ipynb notebook. 
- Once the user_input notebook is open, under 'Kernel' in the menu bar select 'Restart Kernel and Run All Cells'.

![Screenshot 2023-05-11 at 10 24 08 AM](https://github.com/djohnst914/github_upload/assets/123714457/b90fb7ec-793c-40c4-98ed-f0c68d5541f0)

- Once the application loads, a box of inputs such as 'Ticker' and 'Strategy' will open up under the first code block. Go ahead and input your prefferred information as follows and hit the 'Submit' button. Reference image below for example:

![Screenshot 2023-05-11 at 10 23 07 AM](https://github.com/djohnst914/github_upload/assets/123714457/79a9b708-e807-4eeb-8f11-e2b534a59afd)

- To confirm upload, manually select the next block of code under 'User Inputs', followed by 'shift+enter' on your keyboard two times. You should get an output like this, confirming ticker, start/end date, and short/long window:

<img width="600" height="400" alt="Screenshot 2023-05-11 at 10 28 57 AM" src="https://github.com/djohnst914/github_upload/assets/123714457/f4b270a8-ca3a-46db-bf42-b3f7e2ba67d1">

### 2. Sourcev2 (main application)
- Once you have completed the above usage steps, in JupyterLab open the sourcev2MS.ipynb file.
- Once open, same as before, under 'Kernel' in the menu bar select 'Restart Kernel and Run All Cells'.

![Screenshot 2023-05-11 at 10 24 08 AM](https://github.com/djohnst914/github_upload/assets/123714457/b90fb7ec-793c-40c4-98ed-f0c68d5541f0)
- This will automatically run the entire application for your viewing and analyzing pleasure with your inputs from the user_input notebook
- There are a total of 5 visualizations based on the user inputs that depict SMA Crossover Signals, Cumulative Returns, and a Comparison of the selected ticker's Volatilities/Ratios for 2 different strategies offered. Reference example below:

![Screenshot 2023-05-11 at 10 41 04 AM](https://github.com/djohnst914/github_upload/assets/123714457/bcf9dfe8-e223-42eb-bcac-fc4e427c0444)

### 3. How to Manipulate Plotly Graphs
- The plotly graphs come equipped with 9 tools that can be used to meet the visualization/analyzation goals of the user. These tools are very user friendly, and can be found in the top right hand corner within the graphs. Tools include 'Download plot as a png', 'Zoom', 'Pan', 'Box Select', 'Lasso Select', 'Zoom in', 'Zoom out', 'Autoscale', and 'Reset axes'. Reference the image below for 'Download plot as a png' for example:

![Screenshot 2023-05-11 at 10 49 29 AM](https://github.com/djohnst914/github_upload/assets/123714457/0652123c-030b-4ab2-8a7e-91569637a126)

### 4. Web Application Deployment with Voilà - Great for Non-Technical Users
- In your terminal, cd to the directory where this repository was cloned/downloaded
- Enter 'pwd' - displays the complete path to the current directory
- Copy path, type 'voila', then paste path and enter

<img width="542" alt="Screenshot 2023-05-11 at 11 08 15 AM" src="https://github.com/djohnst914/github_upload/assets/123714457/021a4251-3895-48f0-adef-5a2fd7aa4ed9">

- After the web page screen loads, select file 'sourcev2MS.ipynb':
- Voilà! You are now on the main application web application
- **NOTE~** If you want to load the web application with different user inputs, repeat usage steps with new inputs.

---
## *References*
- [Plotly Usage](https://plotly.com/python/#financial-charts)
- [Plotly Crossover Chart](https://chart-studio.plotly.com/~alexjjay/21/_12-ema-26-ema-buy-sell-signal-line-signal-crossover-centerline-crossover-buysell/#/) @alexjjay
- [IPython/ipywidgets](https://www.tutorialspoint.com/jupyter/jupyter_notebook_ipywidgets.htm)

---

## *Contributors*

For any questions, comments, concerns, feel free to contact below: 

**Rosalinda Olvera Fernandez**

[GitHub](https://github.com/rolvera05) - rolvera98271@gmail.com

**Alex Valenzuela**

[GitHub](https://github.com/AlexanderValenzuela) - axvalenzuela@gmail.com  

**James White**

[GitHub](https://github.com/jswhite1992) - jswhite1992@gmail.com

**Michelle Silver**

[GitHub](https://github.com/supersilver1978) - supersilver1978@gmail.com

**Dylan Johnston**

[GitHub](https://github.com/djohnst914) - dylanhjjohnston@gmail.com


---

## *License*

This project is licensed under the MIT License. See [LICENSE](https://github.com/rolvera05/CrossoverPro/blob/main/LICENSE) file for details.