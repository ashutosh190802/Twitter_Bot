# Twitter_Bot
The primary objective of TwitBotSleuth is to tackle the increasing presence of bot accounts on social media platforms, particularly Twitter. These automated accounts can be misleading, spammy, or even malicious, making it essential to identify and differentiate them from genuine human users. TwitBotSleuth comes to the rescue by providing an efficient and accurate way to determine whether a Twitter account belongs to a bot or a real person. by leveraging machine learning and web scraping techniques. With an accuracy of 90%, this tool can effectively identify and flag suspicious accounts.

## How it Works

The Twitter bot detection web app employs a machine learning model to analyze various features of a Twitter user's account and determine the probability of it being a bot. The following features are considered for the analysis:

Default Profile: Whether the user has a default profile image.
Default Profile Image: Whether the user has a default profile image.
Favorites Count: The number of tweets the user has favorited.
Followers Count: The number of followers the user has.
Friends Count: The number of users the user is following.
Geo-Enabled: Whether the user has enabled geolocation on their tweets.
Verified: Whether the user's account is verified by Twitter.
Average Tweets Per Day: The average number of tweets posted per day by the user.
Account Age (Days): The age of the Twitter account in days.

## Getting Started

To run the Twitter bot detection application on your local machine, follow these steps:

Clone this repository to your local machine.

Make sure you have Python installed (Python 3.6 or later is recommended).

Install the required dependencies by running the following command: pip install Flask pandas numpy

Download the pre-trained machine learning model file ('model.pickle') and place it inside the 'model' directory.

Ensure you have access to Twitter's API by obtaining the necessary credentials (consumer key, consumer secret, access token, and access token secret).

Open the 'scraper.py' file and update the Twitter API credentials to enable data scraping from Twitter. This is required to fetch user information from Twitter based on the provided tweet URLs or usernames.

Run the Flask application using the following command: python app.py

The application should now be running locally. Open your web browser and navigate to 'http://127.0.0.1:8000' to access the web interface.

## How to Use

Enter the Twitter username or paste a tweet URL of the user you want to check for bot likelihood.
Click the "Check" button to initiate the bot detection process.
The application will fetch the user's information, extract relevant features, and feed them into the machine learning model.
The result will be displayed on the web interface, indicating the probability of the user being a bot.
Additionally, the application will highlight the result with different colors, giving you a quick visual indication of the bot likelihood.
Please note that the accuracy of bot detection depends on the quality and diversity of the training data used to train the machine learning model. For the best results, ensure the model.pickle file is up-to-date and trained on a diverse dataset.
