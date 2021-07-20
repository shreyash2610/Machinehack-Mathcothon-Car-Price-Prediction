# Machinehack-Mathcothon-Car-Price-Prediction

Leaderboard standing: 55 out of 2400 participants

## About Data

With the rise in the variety of cars with differentiated capabilities and features such as model, production year, category, brand, fuel type, engine volume, mileage, cylinders, colour, airbags and many more, we are bringing a car price prediction challenge for all. We all aspire to own a car within budget with the best features available. To solve the price problem we have created a dataset of 19237 for the training dataset and 8245 for the test dataset.
## Dataset Description

    Train.csv - 19237 rows x 18 columns (Includes Price Columns as Target)
    Attributes
        ID
        Price: price of the care(Target Column)
        Levy
        Manufacturer
        Model
        Prod. year
        Category
        Leather interior
        Fuel type
        Engine volume
        Mileage
        Cylinders
        Gear box type
        Drive wheels
        Doors
        Wheel
        Color
        Airbags
    Test.csv - 8245 rows x 17 columns
    Sample Submission.csv -Please check the Evaluation section for more details on how to generate a valid submission 

## Skills

    Multivariate Regression
    Big dataset, underfitting vs overfitting
    Optimizing RMSLE to generalize well on unseen data

## Evaluation

### What is the Metric In this competition? How is the Leaderboard Calculated ?

    The submission will be evaluated using the RMSLE metric. One can use np.sqrt(mean_squared_log_error(actual, predicted)) to calculate the same
    This hackathon supports private and public leaderboards
    The public leaderboard is evaluated on 70% of Test data
    The private leaderboard will be made available at the end of the hackathon which will be evaluated on 100% of Test data
    The Final Score represents the score achieved based on the Best Score on the public leaderboard

### How to Generate a valid Submission File

Sklearn models support the predict() method to generate the predicted values

You should submit a .csv file with exactly 8245 rows with 1 column(Price). Your submission will return an Invalid Score if you have extra columns or rows.

The file should have exactly 1 column.

Note: Do not shuffle the sequence of the test series

Using Pandas:

submission_df.to_csv('my_submission_file.csv', index=False)
