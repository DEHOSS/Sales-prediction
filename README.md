<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->

<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->



<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
<!-- [![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![project_license][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url] -->






<!-- ABOUT THE PROJECT -->
## About The Project

Dataset
The dataset is available for download on the course website.
Dataset Description:
Here’s a description of the columns based on their names:
• Store id: A unique identifier for each store in the dataset.
• RetailType: The category or type of retail store (e.g., grocery, clothing,
electronics).
• Stock variety: Refers to the range or variety of products offered by the
store (e.g., basic, extended, premium).
• DistanceToRivalStore: The distance from this store to its nearest rival
store.
• RivalOpeningMonth: The month when a rival store opened in proximity
to the store.
• RivalEntryYear: The year when a rival store entered the market or opened
near the store.
• ContinuousBogo: Likely indicates whether a ”Buy One Get One” (BOGO)
offer is currently active (possibly a binary or numeric flag).
• ContinuousBogoSinceWeek: The number of weeks since the continuous
BOGO offer was initiated.
• ContinuousBogoSinceYear: The year when the continuous BOGO offer
started.
• ContinuousBogoMonths: The total duration (in months) for which the
continuous BOGO offer has been active
• DayOfWeek: The day of the week (e.g., Monday, Tuesday, etc.) when the
sales data was recorded.
• Date: The specific date on which the sales data was collected.
• Sales: The total sales made by the store on the given day.
• NumberOfCustomers: The number of customers who visited the store on
the given day.
• Is Open: A binary indicator (e.g., 1 for open, 0 for closed) that specifies
whether the store was open on that day.
2

• BOGO: A flag indicating whether a ”Buy One Get One” (BOGO) offer
was active on the given day (e.g., 1 for active, 0 for not active).
• Holiday: A binary indicator (e.g., 1 for holiday, 0 for non-holiday) to
indicate whether the day was a recognized holiday.


project steps
1. Load Dataset:
• Read the training data from CSV file, selecting relevant columns.
Consider that some columns may not be useful for your analysis and
can be omitted.
2. Load and Merge Store Data:

• Read the stores data from another CSV file to get additional infor-
mation about each store.

• Combine the training and store data based on the store id column
to create a comprehensive dataset.
3. Train & test Data:
• Please divide 70% of the training examples into the training set and
use the remaining 30% as the test set. Select the first 70% of the
examples in chronological order, as we aim to evaluate our models
on their ability to extrapolate to dates beyond the training range.
4. Preprocess Data:
• Replace the missing values in the ’DistanceToRivalStore’ column with
the median of the existing values, and set the remaining missing
values to zero. Feel free to modify this for better approaches if you
prefer.
• Extract ’Year’, ’Month’, ’Day’, and ’WeekOfYear’ from the ’Date’
column, then remove the ’Date’ column. Utilize the pd.to datetime
function and its attributes for easy handling.

• Remove the ’Customers’ column since it is not available during test-
ing.

• Standardize the features using StandardScaler to ensure all features
have a similar scale.
5. Prepare Data for Modeling:

• Separate the features (X) and the target variable (y), which is to-
tal sales.

6. Train and Evaluate Model:
• Train two models: Linear Regression and Random Forest Regressor
and evaluate their performances on the test data.
7. Feature Selection & Importance:
• Utilize feature importance from the Random Forest model. 


<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Contact

Your Name - Hossein Dehghani - h.deh1383@ggmail.com

Project Link: https://github.com/DEHOSS/IMBD-film-KNN-recommender

<p align="right">(<a href="#readme-top">back to top</a>)</p>


[Svelte-url]: https://svelte.dev/
[Laravel.com]: https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white
[Laravel-url]: https://laravel.com
[Bootstrap.com]: https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white
[Bootstrap-url]: https://getbootstrap.com
[JQuery.com]: https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white
[JQuery-url]: https://jquery.com 
