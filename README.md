
# Chicago Electrical Energy DataHub Forecasting Project

This project aims to study, analyze, and forecast the supply and demand of electrical energy for the City of Chicago from 2020 to 2027. 
It uses a combination of OpenAI GenAI models (`gpt-4o-mini`), AutoGen, and two agent types (`CodingAssistantAgent` and `CodeExecutorAgent`) 
to automate tasks in data engineering, analysis, and forecasting.

## Project Overview

The Chicago Electrical Energy DataHub Forecasting Project involves:
1. **Data Collection & Preparation**: Generating or sourcing energy consumption data for 2020-2024.
2. **Data Analysis**: Visualizing historical energy usage.
3. **Forecasting**: Predicting energy consumption for 2025-2027.

## Project Components

1. **CodingAssistantAgent**: Generates the required code based on task descriptions.
2. **CodeExecutorAgent**: Executes generated code to produce desired outputs.

### Key Tasks

- **Data Engineering**: Collect, clean, and prepare historical energy data.
- **Data Analysis**: Plot energy usage trends for 2020-2024.
- **Forecasting**: Predict energy consumption for 2025-2027 based on historical data.

## Folder Structure

The project structure is as follows:
```
.
├── Experiment#1.ipynb          # Main notebook for agent setup and initial task definitions
├── Experiment#2.ipynb          # Supporting notebook with user-defined functions for data operations
├── energy_data_analysis        # All the code and files for experiment 2 generated by the agents (auto-generated)
├── energy_data_analysis_user_defined_functions # All the code and files for experiment 2 generated by the agents
└── README.md                   # Project documentation
```

## Setup and Installation

### Requirements

- Python 3.8 or higher
- Required Python libraries:
  - pandas
  - numpy
  - matplotlib
  - OpenAI AutoGen libraries for coding agents
  
### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/sohamvsonar/chicago-energy-forecast-using-autogens.git
    cd chicago-energy-forecast
    ```

2. Set up a virtual environment:
    ```bash
    python3 -m venv .venvautogen
    source .venvautogen/bin/activate
    ```

3. Install dependencies:
   
4. Setup the OpenAI key in the environment using .env file.

## Usage

### Step 1: Data Preparation
The `Data Engineer` role generates sample energy data from 2020 to 2024 and stores it in `chicago_energy_data.csv`. 

### Step 2: Data Visualization
The `Data Analyst` role loads the prepared data, visualizes it, and saves the plot as `chicago_energy_consumption.png`.

### Step 3: Forecasting
The `Data Scientist` role forecasts energy consumption for 2025-2027 and saves the plot as `chicago_energy_forecast.png`.

### Running the Project

Open `Experiment#1.ipynb` in Jupyter Notebook, which includes:
1. **Agent Setup**: Initializes agents for code generation and execution.
2. **Task Execution**: Loops through defined tasks for each agent role.

### Visualizing Results

Generated visualizations can be accessed directly from the project directory:
- `chicago_energy_consumption.png`: Historical energy consumption plot.
- `chicago_energy_forecast.png`: Forecasted energy consumption plot.

## Contributions

Contributions are welcome. Please submit a pull request with a clear description of your changes.