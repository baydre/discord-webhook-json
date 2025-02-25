# Telex-Discord Integration

This project provides a configuration for integrating Telex messages with a Discord channel using Discord webhooks.

## Overview

The integration routes Telex messages to a specified Discord channel by making use of Discord webhooks. This allows for simple and efficient message forwarding without the need for scheduled tasks.

## Configuration

The configuration for this integration is defined in the `discord-webhook.json` file. Below is a breakdown of the fields in the JSON file:

Collecting workspace information

# Telex-Discord Integration Configuration

This document provides a detailed description of the configuration for integrating Telex messages with a Discord channel using Discord webhooks, as defined in the 

do.json

 file.

## Overview

The integration routes Telex messages to a specified Discord channel by making use of Discord webhooks. This allows for simple and efficient message forwarding without the need for scheduled tasks.

## Configuration

The configuration for this integration is defined in the 

do.json

 file. Below is a breakdown of the fields in the JSON file:

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
    - **No need for scheduled tasks**
    - **Simple message forwarding**
    - **Uses Telex Webhooks → Discord Webhooks (basic API calls)**
  - **integration_category**: The category of the integration (e.g., Communication & Collaboration).
  - **author**: The author of the integration.
  - **settings**: A list of settings required for the integration.
    - **Webhook URL**: The URL of the Discord webhook (type: text, required: true, default: "").
    - **Enable Logging**: A checkbox to enable logging (type: checkbox, required: false, default: "Yes").
    - **Retry Attempts**: The number of retry attempts (type: number, required: true, default: "3").
    - **Alert Level**: The alert level for notifications (type: dropdown, required: true, default: "Normal", options: ["High", "Normal", "Low"]).
    - **Notify Roles**: Roles to notify (type: multi-checkbox, required: false, default: "Admin", options: ["Admin", "Moderator", "User"]).
  - **target_url**: The URL to the source code or repository of the integration.
  - **tick_url**: A URL for a tick or status check (currently set to "None").
  - **endpoints**: A list of endpoints for the integration.
    - **forward_to_discord**: An endpoint to forward messages to Discord.
      - **url**: The URL of the endpoint ("/webhook").
      - **method**: The HTTP method to use (POST).
      - **headers**: The headers to include in the request.
        - **Content-Type**: "application/json".
      - **payload**: The payload to send in the request.
        - **message**: The message to forward ("{{message}}").

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Usage

To use this integration, you need to configure the `.json` file with the appropriate settings and deploy the application to your desired environment.

## Author

This integration was developed by [Baydre](https://github.com/baydre). You can find the source code and more information on the [GitHub repository](https://github.com/baydre/telex_discord_integration).

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
