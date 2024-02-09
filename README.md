Notify-App

### MainActivity.java
- This is the main activity of the application.
- It contains UI components such as EditText, Buttons, and ImageView for user interaction.
- Users can input notification text, select an image from the gallery, and send a notification.
- Permissions for sending notifications are requested dynamically if the device's SDK version is compatible.
- The `showNotification()` method constructs and displays the notification using `NotificationCompat.Builder`.

### NotificationReceiver.java
- This is a BroadcastReceiver responsible for handling actions related to notifications.
- It listens for the action "REMOVE_NOTIFICATION" and cancels the notification when received.

### SplashActivity.java
- This activity displays a splash screen when the application is launched.
- After a specified duration (2 seconds), it transitions to the MainActivity.

### Other Components
- The layout files (not provided) define the UI components and their arrangement.
- The application utilizes resources such as images (placeholders) and strings for UI elements.

### Functionality Overview
1. **Main Screen (MainActivity)**:
   - Users can input notification text and select an image from the gallery.
   - Clicking the "Show Notification" button triggers a confirmation dialog.
   - If notification data is incomplete, an alert is displayed.
   - Permissions are checked and requested if necessary for sending notifications.

2. **Notification Display**:
   - Notifications include the entered text, selected image (or default image if none), and action buttons.
   - Action buttons allow users to visit a developer's website or remove the notification.

3. **Splash Screen (SplashActivity)**:
   - A simple splash screen is displayed for 2 seconds before transitioning to the main activity.
