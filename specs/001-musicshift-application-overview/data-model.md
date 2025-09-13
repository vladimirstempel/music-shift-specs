# Data Model: MusicShift Application

This document defines the key entities for the MusicShift application.

## User
Represents a registered user of the application.

**Attributes**:
- `id`: Unique identifier for the user.
- `email`: User's email address.
- `password`: Hashed password for the user.
- `google_id`: Optional Google ID for users who sign up with Google.
- `created_at`: Timestamp of when the user was created.

## Connection
Represents the authentication link to a music service (Spotify, YouTube Music).

**Attributes**:
- `id`: Unique identifier for the connection.
- `user_id`: Foreign key to the `User` entity.
- `platform`: The music service platform (e.g., 'spotify', 'youtube-music').
- `access_token`: Access token for the platform's API.
- `refresh_token`: Refresh token for the platform's API.
- `expires_at`: Timestamp of when the access token expires.
- `created_at`: Timestamp of when the connection was created.

## Transfer
Represents a transfer job, including configuration, progress, and results.

**Attributes**:
- `id`: Unique identifier for the transfer.
- `user_id`: Foreign key to the `User` entity.
- `source_platform`: The source music service platform.
- `destination_platform`: The destination music service platform.
- `status`: The current status of the transfer (e.g., 'pending', 'in-progress', 'completed', 'failed').
- `config`: JSON object containing transfer configuration options.
- `created_at`: Timestamp of when the transfer was created.
- `completed_at`: Timestamp of when the transfer was completed.

## Playlist
Represents a user's playlist on a music service.

**Attributes**:
- `id`: Unique identifier for the playlist on the source platform.
- `name`: Name of the playlist.
- `description`: Description of the playlist.
- `track_count`: Number of tracks in the playlist.

## Track
Represents a single music track.

**Attributes**:
- `id`: Unique identifier for the track on the source platform.
- `title`: Title of the track.
- `artist`: Artist of the track.
- `album`: Album of the track.
- `isrc`: International Standard Recording Code (ISRC) of the track.
