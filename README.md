# VFS Auto Visa Application and Renewal Slot Acquisition Bot

A Python-based automation bot designed to streamline the visa application process by automatically checking for and booking limited visa appointment slots for various countries. This GUI tool secures available slots in real-time, reducing the manual effort involved in visa scheduling.

## Project Overview

This repository includes bots for visa application processes for:
- **Austria**: `vfsbot_austria.zip`
- **Netherlands**: `vfsbot_netherlands.zip`
- **Germany**: `vfsbot_germany.zip`

Each bot version is packaged with the required libraries and an executable file for easy use without additional installations.

## Features

- **Real-time Slot Monitoring**: Continuously checks for available visa appointment slots, booking them as soon as they are available.
- **Automated Booking**: Reduces manual intervention by automating slot acquisition, particularly helpful during high-demand times.
- **User-friendly Interface**: Each bot includes a GUI built with Tkinter for straightforward input and monitoring.
- **Notifications**: Sends Telegram notifications to alert users upon successful bookings.
- **Standalone Executable**: Packaged as `.exe` files, the bots do not require separate installations of dependencies.

## Prerequisites

- **Python 3.8.5**: Ensure Python 3.8.5 is installed for compatibility with all bot functions.
- **Telegram Bot Token**: Create a Telegram bot using [BotFather](https://core.telegram.org/bots#botfather) and obtain the bot token for notifications.
- **Chat ID**: Obtain your chat ID to receive notifications from the bot.

## Installation and Setup

1. **Extract the ZIP File**
   - Download and extract the respective ZIP file for the desired country (Austria, Netherlands, or Germany).

2. **Configure Telegram Notifications**
   - In the extracted folder, open the `config.py` file and add the following configuration:
     ```
     bot_ids: [""],            # separate with commas (,) for multiple chat ids
     bot_token: "",
     custom_message: Appointment is available.
     ```

3. **Run the Executable**
   - Locate the `.exe` file within the extracted folder and double-click to launch the application.

## Usage

1. **Launch the GUI**: Open the application and enter the required information, such as visa type and preferred dates.
2. **Start Slot Monitoring**: Click "Start Monitoring" to initiate real-time slot checks for the specified country.
3. **Automated Booking**: The bot will attempt to secure a slot as soon as it becomes available.
4. **Receive Notifications**: Get instant notifications on Telegram upon successful booking.

## Troubleshooting

- **Captcha Handling**: For some countries, manual intervention may be required to handle captchas based on the site’s security protocols.
- **Environment Variables**: If notifications aren’t working, double-check the `config.py` configurations for the Telegram bot token and chat ID.

## Additional Notes

- This bot automates repetitive tasks on publicly available appointment booking sites. Ensure usage aligns with the terms of service of each website.
- For customized deployments or scaling, consider running the bot on **AWS EC2** or similar services to maintain consistent operation.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
