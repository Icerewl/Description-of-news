# NURSU NEWS
This bot is designed to automatically retrieve trending news headlines from a specified website, scrape the corresponding articles and images, and then use the scraped data to create and upload videos to YouTube. The bot utilizes several different modules to accomplish this task.

## Functions that are used to create this bot to make it more clear:

image_downloader: This module is used to download the images associated with the scraped articles.

trend_scrape: This module is used to scrape the trending headlines from the specified news website.

paragraph_scraper: This module is used to scrape the full articles corresponding to the trending headlines.

text_to_speech: This module is used to convert the scraped articles into speech using a text-to-speech model.

rake_nltk: This module is used to extract keywords from the scraped articles.

create_videos: This module is used to merge the generated speech with the downloaded images to create a video.

os: This module is used for various file operations such as removing files after use.

re: This module is used for regular expressions to clean the scraped text.

rapid_tags: This module is used to extract hashtags from the scraped article's title.

selen_upload: This module is used to upload the created videos to YouTube.

telegram: This module is used to send status updates and error notifications to the developer.

emoji: This module is used to add emojis to the status updates.

traceback: This module is used to generate detailed error messages.

## The main function of the bot is designed to run continuously, with a built-in exception handling mechanism to catch any errors that may occur during the execution of the script. The bot starts by scraping the trending headlines from the specified news website and then storing the current headlines in a variable. It then enters a continuous loop, in which it periodically re-scrapes the trending headlines and compares the current headlines to the previous headlines. If there are any new headlines, the bot proceeds to scrape the full articles and images associated with the new headlines. It then uses the text-to-speech module to generate speech from the scraped articles, and the create_videos module to merge the speech with the images and create a video.

## The bot then uses the title of the article and the generated video to upload the video to YouTube, it also extracts hashtags from the title of the article and adds them to the video description, it also sends a status update to the developer to confirm that the upload was successful. The bot also includes error handling and status reporting functionality, so if an error occurs, the bot will send an error message to the developer and wait for a specified amount of time before trying again.

## Overall, this bot is designed to automate the process of creating and uploading videos based on trending news articles, in order to keep the developer informed and up-to-date with current events. However due to the specific functionality of this bot, i wish to keep the script and its related files private.
