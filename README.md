# Flutter Auth0 Demo

This is a demonstration project showcasing how to integrate Auth0 authentication into a Flutter application.

## Features

- **Login**: Secure user authentication using Auth0 Universal Login.
- **Profile**: Displays user profile information (Name, Picture) after successful login.
- **Logout**: Securely logs out the user.

## Configuration

The project is currently configured with the following Auth0 credentials in `lib/main.dart`:

- **Domain**: `dev-ounhkbcasrqbxhav.us.auth0.com`
- **Client ID**: `NAlnsuAXMhqwCKXtqF7TcrUtDVDRR3Gw`
- **Scheme**: `flutterdemo`

> **Note**: For a production application, it is recommended to use environment variables or a configuration file to manage these credentials securely.

## Getting Started

### Prerequisites

- Flutter SDK installed
- Android/iOS development environment set up

### Installation

1.  **Clone the repository:**

    ```bash
    git clone <repository-url>
    cd flutterdemo
    ```

2.  **Install dependencies:**

    ```bash
    flutter pub get
    ```

### Running the App

Run the application on your preferred emulator or device:

```bash
flutter run
```

## Code Structure

- **`lib/main.dart`**: Contains the main application logic, including:
    - `MyApp`: The root widget setting up the theme and home page.
    - `HomePage`: Manages the authentication state (`isBusy`, `_credentials`, `auth0` instance).
    - `Login`: Widget displaying the login button.
    - `Profile`: Widget displaying user details and the logout button.

## Dependencies

- [auth0_flutter](https://pub.dev/packages/auth0_flutter): The official Auth0 Flutter SDK.
