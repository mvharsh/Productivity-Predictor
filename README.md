# Productivity Predictor for Garment Manufacturing

The garment industry is highly labor-intensive and relies significantly on the productivity of its employees to meet global demands. Effective prediction of employee productivity can help garment manufacturing companies optimize their processes, allocate resources efficiently, and improve overall performance.

## Objective

The primary goal of this project is to develop a predictive model that estimates the actual productivity of garment employees based on various factors related to the manufacturing process. This model will assist decision-makers in forecasting productivity and making informed operational decisions.

## About Dataset

This dataset includes important attributes of the garment manufacturing process and the productivity of the employees, which have been collected manually and validated by industry experts.

## Attribute Information

- **date:** Date in MM-DD-YYYY
- **day:** Day of the Week
- **quarter:** A portion of the month. A month was divided into four quarters
- **department:** Associated department with the instance
- **team_no:** Associated team number with the instance
- **no_of_workers:** Number of workers in each team
- **no_of_style_change:** Number of changes in the style of a particular product
- **targeted_productivity:** Targeted productivity set by the Authority for each team for each day
- **smv:** Standard Minute Value, it is the allocated time for a task
- **wip:** Work in progress. Includes the number of unfinished items for products
- **over_time:** Represents the amount of overtime by each team in minutes
- **incentive:** Represents the amount of financial incentive (in BDT) that enables or motivates a particular course of action
- **idle_time:** The amount of time when the production was interrupted due to several reasons
- **idle_men:** The number of workers who were idle due to production interruption
- **actual_productivity:** The actual % of productivity that was delivered by the workers. It ranges from 0-1

## Deliverables

- A cleaned and preprocessed dataset ready for modeling.
- A comprehensive report on exploratory data analysis and feature engineering.
- A trained predictive model with detailed evaluation metrics.
- A set of actionable insights and recommendations to improve productivity.
- An intuitive interface where users can interact with the model.

## Work Flow

- Developed a **Flask application** for productivity prediction in garment manufacturing.
- Collected and validated a dataset with industry experts.
- Cleaned and preprocessed the dataset for modeling.
- Performed exploratory data analysis and feature engineering.
- Trained a **Random Forest Regressor model** to predict employee productivity.
- Utilized **XGBoost classification** for label prediction.
- Evaluated the models with detailed metrics.
- Created an intuitive user interface for model interaction.
- Deployed the application using **Docker** and **Render.com.**

## Installation

1. **Clone the repository:**
    ```sh
    git clone https://github.com/mvharsh/Productivity-Predictor.git
    cd Productivity-Predictor
    ```

2. **Install dependencies:**
    ```sh
    pip install -r requirements.txt
    ```

## Running the App Locally

1. **Run the Flask app:**
    ```sh
    python app.py
    ```

2. **Access the app:**
    - Go to `http://127.0.0.1:5000`

## Docker 

1. **Pull the Docker image:**
    ```sh
    docker pull harshinivivek/productivity-predictor:latest
    ```

2. **Run the Docker container:**
    ```sh
    docker run -p 5000:5000 harshinivivek/productivity-predictor:latest
    ```

## Render.com Deployment

1. **Deploy on Render.com:**
    - Connect your GitHub repository on Render.com and deploy the app.

## Usage

- Access the app at [productivity-predictor.onrender.com](https://productivity-predictor.onrender.com/).

## License

This project is licensed under the MIT License.
