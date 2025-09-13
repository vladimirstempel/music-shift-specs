# Quickstart: MusicShift Application

This document provides a quickstart guide to testing the MusicShift application based on the user stories.

## Prerequisites
- The application is running.
- You have valid credentials for Spotify and YouTube Music.

## Testing Scenarios

### Scenario 1: Transfer a playlist
1.  **Register and Log in**: Register a new user and log in to the application.
2.  **Connect Services**: Connect your Spotify and YouTube Music accounts.
3.  **Select Playlist**: Navigate to the transfer page and select a playlist from your Spotify account.
4.  **Start Transfer**: Click the "Transfer" button to start the transfer process.
5.  **Monitor Progress**: Observe the transfer progress on the progress monitoring page.
6.  **Verify Completion**: Once the transfer is complete, verify that the playlist has been created on your YouTube Music account with the correct tracks.

### Scenario 2: View Transfer History
1.  **Complete a Transfer**: Follow the steps in Scenario 1 to complete a transfer.
2.  **Navigate to History**: Navigate to the transfer history page.
3.  **Verify History**: Verify that the completed transfer is listed in the history with the correct status and details.

### Scenario 3: Handle Failed Transfers
1.  **Select a playlist with an unmatchable track**: Find or create a playlist that contains a track that you know does not exist on YouTube Music.
2.  **Start Transfer**: Start the transfer of this playlist.
3.  **Verify Completion Summary**: After the transfer is complete, view the completion summary and verify that the unmatchable track is listed as a failed item.
