## Project Notes

# November 4th, 2026

- Plan the project and create the research question
- Find a dataset to use for the project

Question: How does Spotify's AI DJ (DJ X) impact overall reviews of the streaming service on the Google Play Store?
Dataset Link: https://www.kaggle.com/datasets/ashishkumarak/spotify-reviews-playstore-daily-update 

- The dataset has a usability rank of 10.00 on Kaggle, but I am going to check the data types, values, etc
1. Created the dataframe
2. Checked the data types for each column and checked for null values
   - Didn't get rid of the null values in the "reviewCreatedVersion" column because the version of the app and the date the review was written align with one another
3. Deleted the "thumbsUpCount" column because it's not needed for the analysis, and the "appVersion" column because it contains the same information as the "reviewCreatedVersion" column
4. Double checked the range of dates and the rating counts to make sure they matched the information given on Kaggle

- Starting the analysis
1. Loaded the clean dataset
2. Scanned the "content" column for rows containing the string "DJ" (both uppercase and lowercase)
3. Read the reviews and noticed some reviews don't correlate with DJ X feature (part of the noise in the data)
4. Found the count for each rating based on the selection of reviews containing the keyword
5. Created a bar chart to visualize the counts
   - 1 star and 5 star ratings have the highest counts, meaning afterthoughts regarding the function are mixed
