Setup Instructions:

  Install required dependencies:

  Run in bash terminal:

    pip install python-telegram-bot

  Replace placeholders in the code:

        YOUR_BOT_TOKEN → Your bot's token

        CHAT_ID → Your supergroup ID (must start with -100)

        BASE_DIR → Path to your media folder

    Verify the following:

        The bot is added to the supergroup as an administrator

        Forum mode (Topics) is enabled in the group

        The specified paths exist and are readable

    Launch the bot:

Run in bash terminal:

    python bot.py

Implementation Features:

✔ Automatic topic creation for subfolders
✔ Duplicate file detection
✔ Supported formats: JPG, JPEG, PNG, MP4, MOV, AVI
✔ Logging of all operations
✔ Scan interval: 60 seconds (adjustable via CHECK_INTERVAL)
Important Notes:

⚠ Supergroup IDs must start with -100
⚠ Files in the root folder (BASE_DIR) are ignored
⚠ First run: Creates all topics + uploads all files
⚠ Subsequent runs: Processes only new files
⚠ Database is saved in media_bot.db
