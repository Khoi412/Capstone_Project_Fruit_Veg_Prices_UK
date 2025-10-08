# ![CI logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)

# Project Summary 

- Fruit & Veg Prices in the UK (2017-2022)
- The UK's Horticulture sector saw it's home-produced vegetables value grow from approx £1.5 Billion in 2017 to £1.8 Billion in 2022 and it's fruits produce from £920 Million in 2021 to £1,046 Billion in 2022. 

# Dataset Content

- Data is source from Kaggle https://www.kaggle.com/datasets/datota/fruit-and-vegatable-prices-in-uk-2017-2022

- Total entries: 9,647 rows and 6 columns

- Timeframe: 2017–2022

- Dataset includes information about fruit and veg, what type and pricing over a 5 year period


|           | category           | item        | variety          | date         | price      | unit | 
|-----------|--------------------|-------------|------------------|--------------|------------|------|
|0          | fruit              |      apples |bramleys_seedling |2022-03-11    |  2.05      |  kg  |
|1          | fruit              |      apples |coxs_orange_group |2022-03-11    |  1.22      |  kg  |
|2          | fruit              |      apples |  egremont_russet |2022-03-11    |  1.14      |  kg  |
|3          | fruit              |      apples |         braeburn |2022-03-11    |  1.05      |  kg  |
|4          | fruit              |      apples |             gala |2022-03-11    |  1.03      |  kg  |
|...        |   ...              |         ... |              ... |       ...    |   ...      | ...  |
|9642       | cut_flowers        | alstromeria |           indoor |2017-11-03    |  0.27      | stem |
|9643       | cut_flowers        |chrysanthemum|     indoor_spray |2017-11-03    |  0.22      | stem |
|9644       | cut_flowers        |      lillies|         oriental |2017-11-03    |  0.70      | stem |
|9645       | cut_flowers        |    narcissus|           indoor |2017-11-03    |  0.06      | stem |
|9646       | pot_plants         |     cyclamen|            13_cm |2017-11-03    |  0.75      | unit |

[9647 rows x 6 columns]


# Buisness Requirements

- A fictional international business conglomerate has an interest in the fresh produce sector in the food industry business in the UK. The client has requested that a data analyst analyse the dataset of fruits and vegetable prices and determine:

1. To identify the optimal season to procure and sell fresh produce.

2. Monitor price volatility to inform purchasing and inventory decisions.

3. Compare variety-level pricing (e.g., types of apples).


# Hypotheses and Validation

- Hypothesis 1:
    - On-season produce is significantly cheaper than off-season
    - Validation: Compare mean prices grouped by Season.

- Hypothesis 2:
    - Off-season fruit and veg produce has a high volatile price
    - Validation: Use Standard deviation prices grouped by Season.

- Hypothesis 3:
    - Some varieties of the same fruit and veg are cheaper than it's other variants
    - Validation: Group by variety and compare mean and std pricing. 


## How to use this repo

1. Use this template to create your GitHub project repo. Click the **Use this template** button, then click **Create a new repository**.

1. Copy the URL of your repository to your clipboard.

1. In VS Code, select **File** -> **Open Folder**.

1. Select your `vscode-projects` folder, then click the **Select Folder** button on Windows, or the **Open** button on Mac.

1. From the top menu in VS Code, select **Terminal** > **New Terminal** to open the terminal.

1. In the terminal, type `git clone` followed by the URL of your GitHub repository. Then hit **Enter**. This command will download all the files in your GitHub repository into your vscode-projects folder.

1. In VS Code, select **File** > **Open Folder** again.

1. This time, navigate to and select the folder for the project you just downloaded. Then, click **Select Folder**.

1. A virtual environment is necessary when working with Python projects to ensure each project's dependencies are kept separate from each other. You need to create your virtual environment, also called a venv, and then ensure that it is activated any time you return to your workspace.
Click the gear icon in the lower left-hand corner of the screen to open the Manage menu and select **Command Palette** to open the VS Code command palette.

1. In the command palette, type: *create environment* and select **Python: Create Environment…**

1. Choose **Venv** from the dropdown list.

1. Choose the Python version you installed earlier. Currently, we recommend Python 3.12.8

1. **DO NOT** click the box next to `requirements.txt`, as you need to do more steps before you can install your dependencies. Click **OK**.

1. You will see a `.venv` folder appear in the file explorer pane to show that the virtual environment has been created.

1. **Important**: Note that the `.venv` folder is in the `.gitignore` file so that Git won't track it.

1. Return to the terminal by clicking on the TERMINAL tab, or click on the **Terminal** menu and choose **New Terminal** if no terminal is currently open.

1. In the terminal, use the command below to install your dependencies. This may take several minutes.

 ```console
 pip3 install -r requirements.txt
 ```

1. Open the `jupyter_notebooks` directory, and click on the notebook you want to open.

1. Click the **kernel** button and choose **Python Environments**.

Note that the kernel says `Python 3.12.8` as it inherits from the venv, so it will be Python-3.12.8 if that is what is installed on your PC. To confirm this, you can use the command below in a notebook code cell.

```console
! python --version
```

## Deployment Reminders

* Set the `.python-version` Python version to a [Heroku-22](https://devcenter.heroku.com/articles/python-support#supported-runtimes) stack currently supported version that closest matches what you used in this project.
* The project can be deployed to Heroku using the following steps.

1. Log in to Heroku and create an App
2. At the **Deploy** tab, select **GitHub** as the deployment method.
3. Select your repository name and click **Search**. Once it is found, click **Connect**.
4. Select the branch you want to deploy, then click **Deploy Branch**.
5. The deployment process should happen smoothly if all deployment files are fully functional. Click the button **Open App** at the top of the page to access your App.
6. If the slug size is too large, then add large files not required for the app to the `.slugignore` file.
