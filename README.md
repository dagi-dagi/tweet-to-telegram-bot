README file 

## Twitter to Telegram Bot**

# Stayin' Informed with the Tweet Avalanche!  ➡️ 

This Python bot bridges the gap between Twitter and Telegram, seamlessly delivering tweets from your favorite accounts straight to your designated Telegram channel.

## Key Features:**

- ## Real-time Monitoring:** Scans Twitter accounts for new tweets (including replies, optionally) like a tireless detective.
- ## Telegram Delivery:** Delivers fresh tweets to your Telegram channel at lightning speed, keeping you in the loop.
- ## Dynamic Management:** Add, remove, or delete usernames from the monitored list using convenient Telegram channel commands.
- ## Daily Reports:** Provides daily summaries (at noon) of the number of tweets retrieved for each user.

## Prerequisites:**

- ## Python 3:** The programming language that powers the magic.
- ## Required Libraries:** Install them using `pip install` to join the party:
    - `telebot` (communicates with Telegram)
    - `tweepy` (interacts with Twitter)
    - `pymongo` (stores data in a MongoDB database)
    - `schedule` (ensures timely execution)
    - (and a few other helpful ones)
- ## Telegram Bot Token:** Obtain it from the BotFather settings (keep it confidential!).
- ## MongoDB Connection String:** Where the bot stores its information.

## Authentication Update (Important):**

Twitter recently discontinued unauthorized scraping, necessitating user authorization. Previously, the bot used Nitter's guest tokens.

To authorize and acquire the bot's session:

1. Refer to the Signing In — Tweety 1.0.9.6 documentation: [https://mahrtayyab.github.io/tweety_docs/basic/singing-in.html](https://mahrtayyab.github.io/tweety_docs/basic/singing-in.html) for step-by-step instructions on signing in using Tweety.
2. Generate an authenticated session file named `session.tw_session`.

## Rate Limiting Caution:**

Be mindful of Twitter's rate limits. Consider introducing longer scan intervals or using multiple Twitter accounts (with separate sessions) to distribute the load.

## Getting Started (Easy as Pie!):**

1. Install the required libraries using `pip`.
2. Clone or download the code.
3. Replace placeholders in the code with your information:
    - `API`: Your Telegram bot token (strictly confidential!)
    - `ID`: Your Telegram channel ID (where tweets will be sent)
    - `URL`: Your MongoDB connection string (for secure data storage)
4. Generate the `session.tw_session` file using the provided Tweety documentation link.
5. Run the script from the command line:

   ```bash
   python twitter_to_telegram.py
   ```

## Telegram Channel Commands (Be the Boss!):**

- `/start`: Initiates the bot (use it once initially).
- `/help`: Confused? This command displays all available commands.
- `/add <@username>`: Adds a new Twitter account to the monitored list.
- `/rem <@username>`: Removes a username from the list (you can add it back later).
- `/del <@username>`: Permanently deletes a username from the list.
- `/ls`: Lists all currently monitored usernames.
- `/replies {true/false}`: Includes (true) or excludes (false) replies in the monitoring.

## Additional Notes:**

- The script leverages multi-threading for efficient tweet monitoring and Telegram communication.
- It employs MongoDB as a robust database for storing user and tweet information.
- Scheduled reports and data checks ensure smooth operation.

## Disclaimer:**

Rate-limited accounts cannot access Twitter. Use an account not intended for regular activity. Feel free to customize the code.

## For further assistance:**

- Reach out to `dawitneri888@gmail.com` if you have questions or encounter issues.
- Open an issue in the GitHub repository.

## Credits:**

This project is a creation of Dawit Neri.
## Support:**

If you encounter any issues or have any questions, feel free to reach out to dagimalemu59@gmail.com or open an issue in the GitHub repository.
