# Splitwise Clone

A Flutter-based application inspired by Splitwise to manage expenses and boost productivity. This project is structured with state management using the BLoC pattern and includes features like onboarding, registration, login, and a splash screen.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Screens](#screens)
- [State Management](#state-management)
- [Setup](#setup)
- [Dependencies](#dependencies)
- [Folder Structure](#folder-structure)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This project is a clone of the popular expense management app Splitwise. It aims to provide a seamless and efficient way to manage expenses with a clean and intuitive user interface. The app is built using Flutter and Dart, with a focus on modularity and scalability.

## Features

- **Splash Screen**: A welcoming splash screen with navigation to the onboarding screen.
- **Onboarding**: A multi-step onboarding process to introduce the app's features.
- **Login and Registration**: User authentication with login and registration screens.
- **Form Validation**: Input validation for email, name, and password fields.
- **State Management**: Managed using the BLoC pattern for scalable and maintainable state handling.

## Screens

### Splash Screen

Displays the app logo and transitions to the onboarding screen after a delay.

### Onboarding Screen

A series of pages explaining the app's features with an option to skip or navigate to the registration screen.

### Login Screen

Allows users to log in with their credentials.

### Registration Screen

Allows users to register with their details. Validates inputs like name, email, and password.

### Home Screen

The main screen of the app where users can manage their expenses.

## Screenshots

Here are some screenshots of the app:

### Splash Screen
![Splash Screen](https://github.com/iPrakharV/splitwise_clone/blob/main/assets/screenshots/Simulator%20Screenshot%20-%20iPhone%2015%20Pro%20Max%20-%202024-06-06%20at%2018.17.28.png)

### Onboarding Screen
![Onboarding Screen ](https://github.com/iPrakharV/splitwise_clone/blob/main/assets/screenshots/Simulator%20Screenshot%20-%20iPhone%2015%20Pro%20Max%20-%202024-06-06%20at%2018.17.22.png)


## State Management

The app uses the BLoC (Business Logic Component) pattern for state management. This pattern helps in separating business logic from UI components, making the app more modular and easier to maintain.

### BLoC Components

- **SplashScrBloc**: Manages the state of the splash screen.
- **OnBoardingBloc**: Manages the state of the onboarding screens.
- **RegisterFormBloc**: Handles the state and validation of the registration form.

## Setup

To run this project locally, follow these steps:

1. **Clone the repository**

    ```bash
    git clone https://github.com/iPrakharV/splitwise_clone
    ```

2. **Navigate to the project directory**

    ```bash
    cd splitwise_clone
    ```

3. **Install dependencies**

    ```bash
    flutter pub get
    ```

4. **Run the app**

    ```bash
    flutter run
    ```

## Dependencies

- **flutter_bloc**: For state management using the BLoC pattern.
- **equatable**: For value equality in Dart objects.
- **dots_indicator**: For page indicators in the onboarding screens.
- **meta**: For annotations used in the BLoC pattern.

## Folder Structure

The project follows a structured folder organization:
lib/
|– core/
|   |– util/
|– res/
|   |– app_colors.dart
|   |– app_images.dart
|   |– app_imports.dart
|   |– app_strings.dart
|   |– app_styles.dart
|– screens/
|   |– authenticate/
|   |   |– login/
|   |   |   |– login_screen.dart
|   |   |– register/
|   |   |   |– register_screen.dart
|   |   |   |– domain/
|   |   |   |– presentation/
|   |– home/
|   |   |– presentation/
|   |– welcome_onBoard/
|   |   |– onBoard/
|   |   |   |– bloc/
|   |   |   |   |– onBoarding_bloc.dart
|   |   |   |   |– onBoarding_event.dart
|   |   |   |   |– onBoarding_state.dart
|   |   |   |– presentation/
|   |   |   |   |– onBoarding_screen.dart
|   |   |– splash/
|   |   |   |– bloc/
|   |   |   |   |– splash_scr_bloc.dart
|   |   |   |   |– splash_scr_event.dart
|   |   |   |   |– splash_scr_state.dart
|   |   |   |– splash_screen.dart
|– ui/
|   |– components/
|   |   |– app_form_field.dart
|   |– widgets/
|   |   |– image_widgets.dart

## Contributing

Contributions are welcome! Please fork the repository and use a feature branch. Pull requests are accepted.

1. **Fork the project**
2. **Create your feature branch**

    ```bash
    git checkout -b feature/your-feature-name
    ```

3. **Commit your changes**

    ```bash
    git commit -m 'Add some feature'
    ```

4. **Push to the branch**

    ```bash
    git push origin feature/your-feature-name
    ```

5. **Open a pull request**

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.