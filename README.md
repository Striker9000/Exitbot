# ExitBot - Position Monitoring and Trade Exit Management Bot

## Overview
The Position Manager Bot is an automated trading system designed to manage trading positions using a variety of exit strategies. The bot monitors positions, applies configurable exit strategies, and executes trades based on predefined conditions.

## Features
- Multiple exit strategies (trailing stop, time-based, gamma/DTE-based, etc.)
- Risk management through the Risk Calculator component
- Position monitoring and real-time updates
- Configurable settings via YAML configuration
- Cross-platform support (Windows/Linux)

## Setup Instructions

### Prerequisites
- Python 3.9 or newer
- Git (optional, for cloning the repository)

### Installation

1. **Clone or download this repository**
   ```bash
   git clone [repository-url]
   cd ExitBot
   ```

### Automatic Setup (Recommended)

The easiest way to set up the Position Manager Bot on a new system is to use the provided `setup.py` script:

1. Clone or download the repository to your new machine
2. Open a terminal or command prompt in the bot directory
3. Run the automatic setup:

```bash
python setup.py
```

The setup script will:
- Create the necessary directory structure
- Set up a Python virtual environment
- Install all required dependencies
- Create default configuration files
- Generate startup scripts for both Windows and Linux

### Command Line Options

The setup script supports several command-line options:

- `--config PATH`: Specify a custom configuration file to use
- `--env PATH`: Specify a custom .env file for environment variables
- `--no-venv`: Skip virtual environment creation (if you want to manage dependencies yourself)

### Manual Setup

If you prefer to set things up manually:

1. Create the following directories if they don't exist:
   - `logs`
   - `data`
   - `db`
   - `config`

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Make sure the configuration file exists at `config/settings.yaml`

4. Create a `.env` file in the root directory with your API credentials

## Running the Bot

After setup, you can run the bot using the provided startup scripts:

- **Windows**: Double-click `start_bot.bat` or run it from the command line
- **Linux/Mac**: Run `./start_bot.sh` from the terminal

## Configuration

Before running the bot, make sure to:

1. Edit `config/settings.yaml` with your specific settings:
   - API credentials
   - Scanning interval
   - Exit strategy parameters
   - Notification settings

2. Review the `.env` file and update any environment variables

## Troubleshooting

If you encounter issues:

1. Check the log files in the `logs` directory
2. Verify your API credentials in the configuration
3. Ensure your Python version is 3.7 or newer
4. Look for any error messages in the terminal output

## System Requirements

- Python 3.7 or newer
- Internet connection for API access
- Sufficient disk space for logs and database files

## License

This software is proprietary and confidential."# Exitbot" 
