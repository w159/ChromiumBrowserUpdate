# AutoUpdateChromiumBrowser
Keeps Google Chrome up to date based on what Google has published as the latest version

Running the Auto Update script creates a scheduled task to do the following:
NOTE - The scheduled task uses a random time between 9PM and 6AM. This is to spread the network traffic and calls to the Chromium Team's dev page.

1. Creates Powershell script in C:\Utils
2. When the action runs the script it checks the Chromium Teams Dev page for what they've published as the current_stable version
3. Security Protocol is set to TLS1.2
4. Chrome, Edge, and Brave processes are stopped
5. Chrome is updated to the latest standalone enterprise version
6. The Edge and Brave updater silent commands are ran to complete their updates

The Chrome version should update to the latest version within a few minutes, depending on network speeds.
The Edge and Brave version may take up to 60 minutes to update to the latest version.
