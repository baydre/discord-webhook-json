# Telex-Discord Integration

This project provides a configuration for integrating Telex messages with a Discord channel using Discord webhooks.

## Overview

The integration routes Telex messages to a specified Discord channel by making use of Discord webhooks. This allows for simple and efficient message forwarding without the need for scheduled tasks.

## Configuration

The configuration for this integration is defined in the `discord-webhook.json` file. Below is a breakdown of the fields in the JSON file:

- **data**: Contains the main configuration data.
  - **date**: Contains the creation and update dates.
    - **created_at**: The date when the configuration was created.
    - **updated_at**: The date when the configuration was last updated.
  - **descriptions**: Contains descriptive information about the application.
    - **app_name**: The name of the application.
    - **app_description**: A brief description of what the application does.
    - **app_logo**: A URL to the application's logo.
    - **app_url**: The URL to the application's main page.
    - **background_color**: The background color used in the application's interface.
  - **is_active**: A boolean indicating whether the integration is active.
  - **integration_type**: The type of integration (e.g., output).
  - **key_features**: A list of key features of the integration.
  - **integration_category**: The category of the integration (e.g., Email & Messaging).
  - **author**: The author of the integration.
  - **settings**: A list of settings required for the integration.
    - **label**: The label for the setting.
    - **type**: The type of the setting (e.g., text).
    - **required**: A boolean indicating whether the setting is required.
    - **default**: The default value for the setting.
  - **target_url**: The URL to the source code or repository of the integration.
  - **tick_url**: A URL for a tick or status check (currently set to "null").

## Usage

To use this integration, you need to configure the `discord-webhook.json` file with the appropriate settings and deploy the application to your desired environment.

## Author

This integration was developed by [Baydre](https://github.com/baydre). You can find the source code and more information on the [GitHub repository](https://github.com/baydre/telex_discord_integration).

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
