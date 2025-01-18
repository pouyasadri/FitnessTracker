# 📱 FitnessTrackerApp

FitnessTrackerApp is an iOS application built using 🐦 Swift and 🖼️ SwiftUI. It integrates seamlessly with 🍎 HealthKit to display step counts and calories burned for the current day. The app follows the 🛠️ MVVM (Model-View-ViewModel) architecture to ensure a clean, maintainable, and efficient codebase.

## ✨ Features

- 🍎 HealthKit Integration: Reads step count and active energy burned data from the user's HealthKit store.

- ⏱️ Real-Time Data: Displays today's step count and calories burned dynamically.

- 🎨 Simple UI: A user-friendly interface with intuitive visualizations.

- 🔐 Authorization Management: Effortlessly handles HealthKit authorization requests.

- 🔄 Refresh Functionality: Enables users to manually refresh their fitness data.

## 📋 Prerequisites

Ensure you have the following before running the project:

- 🖥️ Xcode 14.0 or later installed.

- 📱 An iPhone running iOS 15.0 or later.

- 🍎 A HealthKit-compatible device (or a physical iPhone).

- 🍎 HealthKit enabled in your app's capabilities.

## 📥 Installation

- 🛠️ Clone the Repository

```bash
  git clone https://github.com/your-username/FitnessTrackerApp.git
  cd FitnessTrackerApp
```

- 🖼️ Open the Project

Open FitnessTrackerApp.xcodeproj in Xcode.

Set your team and bundle identifier in the project settings.

Enable the HealthKit capability in the Signing & Capabilities tab.

- ▶️ Run the App

Select a physical device (HealthKit does not work on the simulator).

Build and run the project.

## 🛠️ How It Works

1. 🍎 HealthKitManager

Manages HealthKit authorization and data fetching.

Utilizes HKStatisticsQuery to retrieve step count and active energy burned data.

2. 🛠️ FitnessTrackerViewModel

Acts as the intermediary between the HealthKitManager and the ContentView.

Manages the app state and provides data to the UI using @Published properties.

3. 🎨 ContentView

Displays the app's user interface.

Dynamically updates based on HealthKit authorization and fetched fitness data.

Includes buttons for requesting authorization and refreshing data.

## 📂 Project Structure
```bash
FitnessTrackerApp/
├── 🩺 HealthKitManager.swift      # Handles HealthKit integration
├── 🛠️ FitnessTrackerViewModel.swift # ViewModel for managing app state
├── 🎨 ContentView.swift           # Main user interface
├── 🚀 FitnessTrackerAppApp.swift  # Entry point for the app
```

## 🕹️ Usage

- 🔐 Authorize HealthKit:

When the app launches, it prompts you to authorize HealthKit access.

Tap the "Authorize HealthKit" button if prompted.

- 👀 View Fitness Data:

After authorization, the app displays today's step count and calories burned.

- 🔄 Refresh Data:

Tap the "Refresh Data" button to fetch the latest fitness data from HealthKit.

## 🤝 Contributing

- 🪝 Fork the repository.

- Create your 🌟 feature branch: git checkout -b feature/YourFeature.

- Commit your ✏️ changes: git commit -m 'Add some feature'.

- Push to the branch: git push origin feature/YourFeature.

- Open a 🚪 pull request.

## 🙏 Acknowledgments

Built with 🐦 Swift, 🖼️ SwiftUI, and 🍎 HealthKit.

Special thanks to Pouya Sadri for development.

## 📞 Contact

For any questions or suggestions, please contact:

- 📧 Email: pouya.sadri@example.com

- 🐙 GitHub: Pouya Sadri

- ▶️ YouTube: 🎥 Watch the Tutorial

