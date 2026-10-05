Swift Ship Tracker

Swift Ship Tracker is a mobile application designed to help users track ships and monitor their locations in real time. The application provides an easy-to-use interface for viewing ship details, tracking movement, and checking important voyage information.

 Features

Track ships in real time

View the current location of a ship

Display ships on an interactive map

Search for ships by name or identification number

View ship details and voyage information

Monitor ship routes and movement

Refresh tracking information

Simple and responsive mobile interface

Technologies Used

Swift — Primary programming language

SwiftUI / UIKit — User interface

MapKit — Map and location visualization

Core Location — Location-related functionality

REST API — Fetching ship and tracking data

Xcode — Development environment

 Project Structure
SwiftShipTracker/
├── App/
│   └── SwiftShipTrackerApp.swift
├── Models/
│   └── Ship.swift
├── Views/
│   ├── ContentView.swift
│   ├── ShipListView.swift
│   ├── ShipDetailView.swift
│   └── MapView.swift
├── ViewModels/
│   └── ShipViewModel.swift
├── Services/
│   └── ShipAPIService.swift
├── Resources/
│   └── Assets.xcassets
└── README.md

Getting Started
Prerequisites

Make sure you have:

macOS

Xcode

Swift

An iOS simulator or physical iPhone

Access to the required ship-tracking API

Installation

Clone the repository:

git clone https://github.com/your-username/SwiftShipTracker.git


Open the project in Xcode:

cd SwiftShipTracker
open SwiftShipTracker.xcodeproj


Configure your API credentials if required.

Select an iOS simulator or connected device.

Build and run the application using ⌘ + R.

API Configuration

The application requires a ship-tracking API to retrieve live vessel information.

Store API credentials securely rather than committing them directly to the repository.

Example:

struct APIConfig {
    static let baseURL = "https://api.example.com"
    static let apiKey = "YOUR_API_KEY"
}


Note: Replace the example API URL and key with the API used by your project.

📱 How It Works

The user opens the Swift Ship Tracker application.

Available ships are retrieved from the tracking API.

Ship positions are displayed on the map.

Users can search for a specific vessel.

Selecting a ship displays additional information such as:

Ship name

IMO/MMSI number

Current position

Speed

Course

Destination

Vessel status

The application periodically refreshes the ship's position.

Example Ship Data
{
  "name": "Ocean Explorer",
  "mmsi": "123456789",
  "latitude": 13.0827,
  "longitude": 80.2707,
  "speed": 12.5,
  "course": 180,
  "destination": "Chennai",
  "status": "Under Way"
}

Privacy & Security

API keys should not be hardcoded in production builds.

Do not commit sensitive credentials to Git.

Request only the location permissions required by the application.

Follow the privacy policy and terms of the selected ship-tracking API.

Testing

Run the project's unit and UI tests from Xcode:

Product → Test


The project should include tests for:

API requests

Ship data parsing

Search functionality

Map annotations

View model behavior

Future Improvements

Ship arrival/departure notifications

Favorite ships

Custom tracking zones

Historical ship routes

Multiple map styles

Port information

Dark mode

Improved real-time tracking

Voyage statistics

Contributing

Contributions are welcome!

Fork the repository.

Create a feature branch:

git checkout -b feature/new-feature


Commit your changes:

git commit -m "Add new feature"


Push the branch:

git push origin feature/new-feature


Open a Pull Request.

License

This project is licensed under the MIT License.

See the LICENSE file for more information.

Author

Your Name
