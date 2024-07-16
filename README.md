# Amazon Coupon Analysis

This repository contains the analysis and visualization of coupon acceptance data from Amazon. The goal is to distinguish between customers who accepted a driving coupon versus those that did not.

## Context
Imagine driving through town and a coupon is delivered to your cell phone for a restaurant near where you are driving. Would you accept that coupon and take a short detour to the restaurant? Would you accept the coupon but use it on a subsequent trip? Would you ignore the coupon entirely? What if the coupon was for a bar instead of a restaurant? What about a coffee house? Would you accept a bar coupon with a minor passenger in the car? What about the weather? Would weather impact the rate of acceptance? What about the time of day?

Obviously, proximity to the business is a factor on whether the coupon is delivered to the driver or not, but what are the factors that determine whether a driver accepts the coupon once it is delivered to them? How would you determine whether a driver is likely to accept a coupon?

## Overview

The goal of this project is to use what you know about visualizations and probability distributions to distinguish between customers who accepted a driving coupon versus those that did not.

## Data

This data comes to us from the UCI Machine Learning repository and was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios including the destination, current time, weather, passenger, etc., and then asks people whether they will accept the coupon if they are the driver. Answers given that the users will drive there “right away” or “later before the coupon expires” are labeled as “Y = 1”; and answers “no, I do not want the coupon” are labeled as “Y = 0”. There are five different types of coupons -- less expensive restaurants (under $20), coffee houses, carry out and take away, bars, and more expensive restaurants ($20–$50).

## Deliverables

Your final product should be a brief report that highlights the differences between customers who did and did not accept the coupons. To explore the data you will utilize your knowledge of plotting, statistical summaries, and visualization using Python. You will publish your findings in a public-facing GitHub repository as your first portfolio piece.

## Data Description

Keep in mind that these values mentioned below are average values.

The attributes of this data set include:

1. User attributes
   - Gender: male, female
   - Age: below 21, 21 to 25, 26 to 30, etc.
   - Marital Status: single, married partner, unmarried partner, or widowed
   - Number of children: 0, 1, or more than 1
   - Education: high school, bachelors degree, associates degree, or graduate degree
   - Occupation: architect & engineering, business & financial, etc.
   - Annual income: less than $125000, $125000 - $249999, $250000 - $374999, etc.
   - Number of times that he/she goes to a bar (e.g., less than 1, 1 to 3, 4 to 8, greater than 8)
   - Number of times that he/she goes to a coffee house (e.g., less than 1, 1 to 3, 4 to 8, greater than 8)
   - Number of times that he/she goes to a restaurant with a value of the expense less than $20 per person (e.g., less than 1, 1 to 3, 4 to 8, greater than 8)
   - Number of times that he/she goes to a restaurant with a value of the expense less than $50 per person (e.g., less than 1, 1 to 3, 4 to 8, greater than 8)
2. Contextual attributes
   - Driving destination: home, work, or no urgent destination
   - Location of user, coupon, and destination: we provide a map to show the geographical location of the user, destination, and venue, and we mark the distance between each two places with time of driving. The user can make the decision if the venue is on the way to his/her destination
   - Weather: sunny, rainy, or snowy
   - Temperature: 30F, 55F, or 80F
   - Time: 10AM, 2PM, or 6PM
   - Passenger: alone, partner, kid(s), or friend(s)
3. Coupon attributes
   - Time before it expires: 2 hours or one day

## Summary of Findings
- Drivers who are regular bar-goers and are socially active, as indicated by having adult passengers or being younger than 30, are more likely to accept bar coupons.
- This tendency is stronger among those who are not widowed and have established habits and preferences for socializing at bars.
- Older drivers with frequent bar visits may also exhibit a higher acceptance rate due to potentially higher disposable income and greater interest in bar-related activities.
- However, lower-income drivers who frequently visit cheap restaurants show a relatively lower acceptance rate, indicating different priorities or preferences, suggesting a need for tailored marketing strategies for this demographic.

## Getting Started

To get a local copy of the project up and running, follow these simple steps.

### Prerequisites

Make sure you have Python installed on your local machine. You can download it from [python.org](https://www.python.org/).

### Installation

1. Clone the repo
   ```sh
   git clone https://github.com/stirelli/amazon-coupon-analysis.git

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

### Next Steps and Recommendations
- Further analysis could be conducted on other coupon types to see if similar patterns hold.
- Implement targeted marketing strategies based on the findings to increase coupon acceptance rates.
- Explore additional demographic factors that might influence coupon acceptance.
