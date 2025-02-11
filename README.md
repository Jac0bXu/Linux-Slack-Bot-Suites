# Linux-Slack-Bot-Suites

## Overview
The Linux-Slack-Bot-Suites is a collection of tools designed to enhance the management and monitoring of Linux systems through Slack. This suite includes various submodules that provide functionalities such as remote terminal access, system monitoring, and automated scheduling for Slack channels.

## Submodules

### 1. [slack-linux-terminal](https://github.com/Jac0bXu/slack-linux-terminal)
A remote terminal access solution that allows users to control a Linux machine through Slack messages. This tool is particularly useful for:
- Remote server management when SSH access is blocked or unavailable.
- Quick system checks without needing to log in via SSH.
- Team collaboration on system administration tasks.
- Emergency access when traditional remote access methods fail.

**Key Features:**
- Execute any Linux terminal command through Slack messages.
- Real terminal-like experience with username@hostname:path$ formatting.
- Directory navigation support (cd command maintains state).
- Command output formatted in code blocks for readability.
- Built-in 15-second timeout protection against hanging commands.
- Logs all commands and their outputs for accountability.

**Installation:**
1. Clone the repository.
2. Install dependencies: `pip install -r requirements.txt`.
3. Create a `.env` file with the necessary Slack tokens and channel IDs.

### 2. [rasPiLoadSlack](https://github.com/Jac0bXu/rasPiLoadSlack)
A comprehensive monitoring system designed specifically for Raspberry Pi devices that need constant supervision. This tool is essential for:
- Maintaining 24/7 Raspberry Pi servers.
- Preventing system failures through early warning.
- Monitoring critical Pi-based services.
- Remote temperature and resource management.
- Automatic failure detection and notification.

**Key Features:**
- Real-time CPU, memory, and disk usage monitoring.
- CPU temperature tracking with overheating alerts.
- Process monitoring (specifically tracks mission-critical processes).
- Automatic failure detection and instant Slack alerts.
- Network connectivity monitoring with downtime alerts.
- Scheduled status updates for regular health checks.

**Installation:**
1. Install dependencies: `pip install -r requirements.txt`.
2. Create a `.env` file with the necessary Slack tokens and channel IDs.

### 3. [signUp](https://github.com/Jac0bXu/signUp)
An automated scheduling system designed for managing recurring time slots in Slack channels. Specifically built for:
- Managing weekly volunteer schedules.
- Coordinating recurring team meetings.
- Organizing office hours or support slots.
- Handling regular resource booking.
- Automating attendance tracking.

**Key Features:**
- Posts weekly schedule templates automatically.
- Customizable time slots for Thursday and Friday.
- Thread-based response system for organization.
- Emoji reaction-based sign-up system.
- Automatic setup and cleanup slot assignment.
- Persistent schedule tracking.

**Installation:**
1. Install required packages: `pip install -r requirements.txt`.
2. Create a `.env` file with the necessary Slack tokens and channel IDs.

## Usage
Each submodule can be run independently based on the specific needs of the user. Ensure that the required environment variables are set in the `.env` files for proper functionality.

## License
This project is licensed under the MIT License. See the LICENSE file for more details.