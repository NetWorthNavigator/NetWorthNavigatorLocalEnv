# Project Setup Guide

This guide will walk you through setting up the project environment, including the Plaid Quickstart and Supabase instances.

## Initial Setup

1. **Run the Automation Script**: Begin by running the `./setup_env` script from your terminal. This script setup_envs the initial setup process.

    ```bash
    ./setup_env
    ```

2. **Configure Plaid Quickstart**:
    - After the initial run of `./setup_env`, you need to configure the Plaid Quickstart environment.
    - Navigate to the `./plaid-quickstart/.env` file.
    - Enter your `PLAID_CLIENT_ID` and `PLAID_SECRET` in the respective fields within the `.env` file.

3. **Run the Automation Script Again**: With the Plaid Quickstart configured, run the `./setup_env` script once more to finalize the setup.

    ```bash
    ./setup_env
    ```

## Accessing Plaid

- **Plaid Quickstart Frontend**: Access the frontend interface at [http://localhost:3000](http://localhost:3000).
- **Plaid Quickstart Backend**: The backend services are available at [http://localhost:5000](http://localhost:5000).

## Accesing Supabase

- **Accessing Supabase**: You can access the Supabase instance through port `8000`. Use the following URL to connect:

    ```
    http://localhost:8000/rest/v1/
    ```

- **Authentication**: To authenticate your requests, include a header with the key `apikey` and your API key as the value.

    - The service role API key (required for authentication) can be found in the `./supabase/docker/.env` file.

## Conclusion

Following these steps should set up your local development environment with access to both Plaid Quickstart and Supabase services. Ensure you have the necessary credentials and API keys configured as described above to interact with these services successfully.