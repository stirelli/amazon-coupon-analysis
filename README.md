# Amazon Coupon Analysis

This repository contains the analysis and visualization of coupon acceptance data from Amazon. The goal is to distinguish between customers who accepted a driving coupon versus those that did not.

## Project Structure

- `data/`: Contains the dataset `coupons.csv`.
- `prompt.ipynb`: The Jupyter notebook with all the analysis and visualizations.
- `requirements.txt`: Lists the Python dependencies for this project.

## Context

Imagine driving through town and a coupon is delivered to your cell phone for a restaraunt near where you are driving. Would you accept that coupon and take a short detour to the restaraunt? Would you accept the coupon but use it on a sunbsequent trip? Would you ignore the coupon entirely? What if the coupon was for a bar instead of a restaraunt? What about a coffee house? Would you accept a bar coupon with a minor passenger in the car? What about if it was just you and your partner in the car? Would weather impact the rate of acceptance? What about the time of day?

Obviously, proximity to the business is a factor on whether the coupon is delivered to the driver or not, but what are the factors that determine whether a driver accepts the coupon once it is delivered to them? How would you determine whether a driver is likely to accept a coupon?

## Overview

The goal of this project is to use what you know about visualizations and probability distributions to distinguish between customers who accepted a driving coupon versus those that did not.

## Data

This data comes to us from the UCI Machine Learning repository and was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios including the destination, current time, weather, passenger, etc., and then asks the person whether they will accept the coupon if he is the driver. Answers that the user will drive there “right away” or “later before the coupon expires” are labeled as “Y = 1”; and answers “no, I do not want the coupon” are labeled as “Y = 0”. There are five different types of coupons -- less expensive restaurants (under $20), coffee houses, carry out & take away, bar, and more expensive restaurants ($20–$50).

## Deliverables

Your final product should be a brief report that highlights the differences between customers who did and did not accept the coupons. To explore the data you will utilize your knowledge of plotting, statistical summaries, and visualization using Python. You will publish your findings in a public facing GitHub repository as your first portfolio piece.

## Data Description

Keep in mind that these values mentioned below are average values.

The attributes of this data set include:
1. User attributes
    -  Gender: male, female
    -  Age: below 21, 21 to 25, 26 to 30, etc.
    -  Marital Status: single, married partner, unmarried partner, or widowed
    -  Number of children: 0, 1, or more than 1
    -  Education: high school, bachelors degree, associates degree, or graduate degree
    -  Occupation: architecture & engineering, business & financial, etc.
    -  Annual income: less than \\$12500, \\$12500 - \\$24999, \\$25000 - \\$37499, etc.
    -  Number of times that he/she goes to a bar: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
    -  Number of times that he/she buys takeaway food: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
    -  Number of times that he/she goes to a coffee house: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
    -  Number of times that he/she eats at a restaurant with average expense less than \\$20 per person: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
    -  Number of times that he/she goes to a bar: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
    

2. Contextual attributes
    - Driving destination: home, work, or no urgent destination
    - Location of user, coupon and destination: we provide a map to show the geographical location of the user, destination, and the venue, and we mark the distance between each two places with time of driving. The user can see whether the venue is in the same direction as the destination.
    - Weather: sunny, rainy, or snowy
    - Temperature: 30F, 55F, or 80F
    - Time: 10AM, 2PM, or 6PM
    - Passenger: alone, partner, kid(s), or friend(s)


3. Coupon attributes
    - time before it expires: 2 hours or one day

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

### Notes

- Ensure you have an active internet connection to fetch any additional dependencies or data if required.
- Use the virtual environment to avoid any conflicts with other projects or system-wide libraries.

## License

Distributed under the MIT License. See `LICENSE` for more information.