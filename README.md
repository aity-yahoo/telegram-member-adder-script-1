# Telegram Member Adder Script

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/sabnam777/telegram-member-adder-script/blob/main/LICENSE)

This is a Python script for adding members to a Telegram group automatically. It utilizes the Telegram Bot API to perform the member addition process.

## Features

- Add multiple members to a Telegram group automatically.
- Supports adding members from a CSV file.
- Customizable delay between member additions.
- Easy setup and configuration.

## Prerequisites

- Python 3.6 or higher
- `python-telegram-bot` library

## Installation

1. Clone the repository:

   ```shell
   git clone https://github.com/sabnam777/telegram-member-adder-script.git
   
2.Install the required dependencies:

    pip install -r requirements.txt 
   
## Configuration
Create a new Telegram Bot and obtain the API token. You can follow the official BotFather documentation for detailed instructions.

Rename the config.example.ini file to config.ini.

     [Telegram]
     api_token = YOUR_TELEGRAM_API_TOKEN
     group_id = YOUR_TELEGRAM_GROUP_ID

    [General]
     delay = 5  # Delay in seconds between member additions
     Open config.ini in a text editor and provide the necessary details:   

## Usage
Prepare a CSV file containing the member details. The CSV file should have a header row with the columns: name, phone, username.

Run the script:
      ` python telegram_member_adder.py --file members.csv`
Replace members.csv with the actual name of your CSV file.

The script will start adding members to the specified Telegram group. The progress and any errors encountered will be displayed in the console.
