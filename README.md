# Spotify Clone Music Application

## Overview
This project is a **Spotify Clone** built using **React** and the **Spotify Web API**. It allows users to log in with their Spotify account, browse and play music, create playlists, and manage their library.

## Features
- **User Authentication**: Login using Spotify OAuth.
- **Browse Music**: Search and explore songs, albums, and artists.
- **Play Music**: Stream music directly from Spotify.
- **Create Playlists**: Add and remove songs from playlists.
- **Control Playback**: Play, pause, and skip tracks.

## Technologies Used
- **Frontend**: React, React Router, Tailwind CSS
- **Backend**: Node.js, Express.js (if applicable)
- **API Integration**: Spotify Web API
- **State Management**: Context API / Redux (Specify which one is used)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/spotify-clone.git
   cd spotify-clone
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Set up environment variables:
   - Create a `.env` file in the root directory.
   - Add the following variables:
     ```env
     REACT_APP_SPOTIFY_CLIENT_ID=your_spotify_client_id
     REACT_APP_SPOTIFY_REDIRECT_URI=http://localhost:3000/callback
     ```

4. Start the development server:
   ```bash
   npm start
   ```

## Spotify API Authentication
- You need to register your application on the [Spotify Developer Dashboard](https://developer.spotify.com/dashboard/applications).
- Set the redirect URI to `http://localhost:3000/callback`.



## API Endpoints

### 1. Get User Profile
```http
GET https://api.spotify.com/v1/me
```
- **Response**: User details including name, email, and profile picture.

### 2. Search for Music
```http
GET https://api.spotify.com/v1/search?q={query}&type=track,artist,album
```
- **Response**: List of matching tracks, artists, and albums.

### 3. Get User’s Playlists
```http
GET https://api.spotify.com/v1/me/playlists
```
- **Response**: List of user-created playlists.

