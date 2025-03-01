# Automated_TikTok_Videos

THIS PROGRAM CURRENTLY NO LONGER WORKS. READ BELOW FOR MORE DETAILS.

A Python program that automatically creates TikTok-format videos from different subreddits.

For examples, you can check this Instagram page: https://www.instagram.com/cool_reddit_things/reels/. I posted a video per day for about two months. Some of them were quite successful, with the best ones reaching around 180k views.

This project uses web scraping and the Reddit API to get information from Reddit pages. So, you will need to change the user ID and login credentials for both your Reddit account and Reddit API keys in the file if you want to try it. It uses MoviePy to edit the video with subtitles or images and Tortoise to generate the voiceover.

I stopped working on it in December 2023. With the rapid growth of AI, this means that Tortoise is either much better now, with new functionalities not used in this project, or that there are better free alternatives that I am not aware of.

You will also need a video for the background. You can either import it, which can take quite a while if the file is large, or upload the video to your Google Drive and then connect Drive to Colab. The Colab file in the repository uses the Drive option.

There are two variants of the program:
- One that retrieves Reddit stories and adds subtitles.
- One that uses AskReddit and displays the comments.
  
However, as time passes, some things may become deprecated. For example, even though it worked when I first wrote this program, as of February 28, 2025, the web scraping method I used to take screenshots no longer works due to Reddit implementing measures against it. It seems that there is no real way to bypass this. The best option to replace web scraping would be to recreate Reddit’s UI using libraries such as Pillow. This issue is especially problematic for the AskReddit version of the program, which relied entirely on screenshots.
Additionally, Whisper.cpp, which I used to generate transcripts from the audio, has changed a few things, so you will need to modify the function call as it no longer works.

Moreover, even when everything was working, there were still some issues and potential improvements worth mentioning:
- Some abbreviations were misread by the voiceover, which could be annoying.
- The text font wasn't great.
- There might be better voice options.
- Other factors affecting how polished the final video looks.
- These issues are quite noticeable when watching the videos on the Instagram page.
