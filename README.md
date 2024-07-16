# Amazon Coupon Analysis

This repository contains the analysis and visualization of coupon acceptance data from Amazon. The goal is to distinguish between customers who accepted a driving coupon versus those that did not.

## Project Structure

- `data/`: Contains the dataset `coupons.csv`.
- `prompt.ipynb`: The Jupyter notebook with all the analysis and visualizations.
- `requirements.txt`: Lists the Python dependencies for this project.

## Getting Started

To get a local copy of the project up and running, follow these simple steps.

### Prerequisites

Make sure you have Python installed on your local machine. You can download it from [python.org](https://www.python.org/).

### Installation

1. Clone the repo

    ```sh
    git clone https://github.com/stirelli/amazon-coupon-analysis.git
    ```

2. Navigate to the project directory

    ```sh
    cd amazon-coupon-analysis
    ```

3. Create a virtual environment

    ```sh
    python -m venv env
    ```

4. Activate the virtual environment

    - On Windows

        ```sh
        env\Scripts\activate
        ```

    - On MacOS/Linux

        ```sh
        source env/bin/activate
        ```

5. Install the dependencies

    ```sh
    pip install -r requirements.txt
    ```

### Usage

1. Navigate to the project directory if you are not already there

    ```sh
    cd amazon-coupon-analysis
    ```

2. Open the Jupyter notebook

    ```sh
    jupyter notebook prompt.ipynb
    ```

3. Run the cells in the notebook to see the analysis and visualizations.

### Data

The dataset used in this analysis is included in the `data` directory. The main file is `coupons.csv`.

### Project Organization

- **Notebooks**: The analysis and visualizations are contained within the Jupyter notebook `prompt.ipynb`.
- **Data**: The data required for the analysis is located in the `data/` directory.
- **Dependencies**: The `requirements.txt` file lists all the Python libraries that need to be installed to run the notebook.

### Notes

- Ensure you have an active internet connection to fetch any additional dependencies or data if required.