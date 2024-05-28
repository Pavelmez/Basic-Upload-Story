# Basic Upload Story

Basic Upload Story is an Android application built using Kotlin that allows users to upload stories to the [Dicoding Story API](https://story-api.dicoding.dev/v1#/). The app provides several features to enhance user experience, including location pinning, secure login, database storage, detailed story views, animations, custom views, unit tests, and custom map styling.

## Features

- **Upload Stories**: Upload stories to the Dicoding Story API with ease.
- **Pinpoint Location**: Use maps to pinpoint the location of the story.
- **Save Login Token**: Securely save login tokens using preferences.
- **Save Story List**: Store story lists using a database with remote mediation.
- **Story Details**: Click on a story to view more detailed information.
- **Animations and Custom Views**: Enjoy animations and custom views, especially for short passwords.
- **Unit Tests**: Ensure the app functions correctly with comprehensive unit tests.
- **Custom Maps JSON**: Customize the map styling using a custom JSON file.

## Installation

To run this project, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/StoryApp.git
   cd StoryApp
   ```
2. Open the project in Android Studio.
3. Let Gradle sync and build the project.
4. Connect an Android device or start an emulator, then run the app.

## Usage

- **Uploading a Story**: On the main screen, navigate to the upload section, fill in the story details, select the location, and click the upload button.
- **Viewing Stories**: The main screen displays a list of stories. Click on any story to view detailed information.
- **Map Integration**: Stories with locations will be marked on the map. Click on a map marker to view the corresponding story details.

## Development

### Prerequisites

- Android Studio
- Kotlin

### Configuration

1. **API Configuration**:
   - Update the `baseUrl` in your network configuration to `https://story-api.dicoding.dev/v1/`.

2. **Map Configuration**:
   - Place your custom maps JSON file in the `res/raw` directory.
   - Load the custom JSON in your map configuration code.

3. **Maps API Key**:
   - Add your Google Maps API key to the `local.properties` file:
     ```properties
     MAPS_API_KEY=your_google_maps_api_key
     ```

### Dependencies

The project uses several libraries, including:

- [Retrofit](https://square.github.io/retrofit/) for networking
- [Glide](https://bumptech.github.io/glide/) for image loading
- [Room](https://developer.android.com/training/data-storage/room) for local database
- [Google Maps](https://developers.google.com/maps/documentation) for map functionality
- [ViewModel and LiveData](https://developer.android.com/topic/libraries/architecture/viewmodel) for state management
- [Coroutines](https://kotlinlang.org/docs/coroutines-overview.html) for background tasks

### Project Structure

- **retrofit**: Contains the Retrofit API service for uploading and fetching stories.
- **data**: Contains the repository pattern for data handling.
- **db**: Contains the Room database and DAO interfaces.
- **view**: Contains the UI components like Activities, Fragments, and ViewModels.
- **utils**: Utility classes and helper functions.

## Contributing

Feel free to contribute to this project by submitting a pull request. Please follow the standard GitHub flow:

1. Fork the repository.
2. Create a feature branch.
3. Commit your changes.
4. Push to the branch.
5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [Dicoding Story API](https://story-api.dicoding.dev/v1#/)
- [Retrofit](https://square.github.io/retrofit/)
- [Glide](https://bumptech.github.io/glide/)
- [Room](https://developer.android.com/training/data-storage/room)
- [Google Maps](https://developers.google.com/maps/documentation)
- [ViewModel and LiveData](https://developer.android.com/topic/libraries/architecture/viewmodel)
- [Coroutines](https://kotlinlang.org/docs/coroutines-overview.html)
