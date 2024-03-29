# News App

## Overview

The News App is an Android application that provides users with the latest news articles from various sources. It follows the MVVM (Model-View-ViewModel) architecture, allowing for a clean and organized structure. The app utilizes Room for local data storage to save bookmarked news articles, and Retrofit for seamless integration with a news API.

## Features

- Browse latest news articles from multiple sources.
- Bookmark interesting articles for later reading.
- Offline access to bookmarked articles using Room database.
- Clean and organized MVVM architecture.
- Seamless integration with a News API using Retrofit.

## Architecture

The app follows the MVVM (Model-View-ViewModel) architecture, which separates the concerns of data, UI, and business logic. The key components include:

- **Model:** Represents the data and business logic. In this app, it includes entities for articles, a Room database for local storage, and a repository for managing data.

- **View:** Represents the UI components. Activities and Fragments observe data changes from the ViewModel and update the UI accordingly.

- **ViewModel:** Acts as a mediator between the Model and the View. It holds and manages UI-related data, providing a clean interface for the UI to interact with the underlying data.

## Technologies Used

- **MVVM Architecture:** Ensures a separation of concerns and a scalable, maintainable codebase.

- **Room:** A local database to store bookmarked news articles, providing offline access.

- **Retrofit:** A type-safe HTTP client for Android that simplifies API integration.

## Getting Started

Follow these steps to set up and run the News App on your local machine:

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/news-app.git
2. Open the project in Android Studio.

3. Build and run the app on an Android emulator or physical device.


## API Key

The News App requires an API key to access the news API. Obtain an API key from [News API](https://newsapi.org/) by following these steps:

1. Visit [News API](https://newsapi.org/) and sign up for an account.

2. Once registered, obtain your API key from your account dashboard.

3. Add the API key to the `API_KEY` constant in the `NewsApiService.kt` file:

   ```kotlin
   // NewsApiService.kt
   const val API_KEY = "your_api_key_here"