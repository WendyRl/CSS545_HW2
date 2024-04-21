# Document containing Various Approaches to Storage Management with Pros and Cons:
For our Fridge Partner app, we have considered several approaches to storage management on the Android platform:
## 1. Shared Preferences:
Pros: Lightweight and easy to use for storing key-value pairs, suitable for storing small amounts of data like user settings.

Cons: Limited in capacity and not suitable for storing large amounts of data or complex data structures.
## 2. Internal Storage:
Pros: Provides private storage space within the app's sandbox, ensuring data security and privacy.

Cons: Limited in capacity and not accessible to other apps or users, restricting data sharing or backup options.
## 3. External Storage (SD card):
Pros: Offers larger storage capacity and flexibility for storing media files like images or videos.

Cons: Requires additional permissions and may not always be available or accessible, depending on device configuration.
## 4. SQLite Database:
Pros: Provides a structured and efficient way to store and retrieve structured data, suitable for complex data models.

Cons: Requires more setup and management overhead compared to other storage options, may be overkill for simple data storage needs.

# App Demonstrating Storage Management:
Our Fridge Partner app demonstrates effective storage management through the following features:
## Store and Load Media Items Locally:
Users can upload images of food items to their fridge, which are then stored locally on their device.

Using Android's Internal Storage, these images are securely saved within the app's private storage space.

Upon launching the app, stored images are loaded from Internal Storage and displayed in the app's interface, providing users with quick access to their fridge inventory.

## Store and Load User Settings Locally:
User preferences and settings, such as notification preferences and default fridge settings, are stored locally using Android's SharedPreferences framework.

This allows users to customize their experience within the app, with settings persisting across app sessions.

When the app is opened, user settings are loaded from SharedPreferences and applied to the app's functionality, ensuring a personalized user experience.
