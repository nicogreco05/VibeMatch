# 🎵 VibeMatch

A Java application that connects to the Spotify API and generates a shared playlist based on the musical tastes of multiple users.

## How it works
1. Each user logs in with their Spotify account via OAuth2
2. The app fetches their top 10 most listened tracks
3. An algorithm finds artists in common between all users
4. A blended playlist is generated with songs from those shared artists

## Tech Stack
- Java 17+
- Spotify Web API
- OAuth2 Authorization Code Flow
- Gson (JSON parsing)
- Maven

## Setup
1. Create an app on [Spotify Developer Dashboard](https://developer.spotify.com/dashboard)
2. Add `http://127.0.0.1:8080/callback` as Redirect URI
3. Add your `client_id`, `client_secret` and `redirect_uri` in `src/main/resources/config.properties`
4. Run `Main.java`

## Note
The app runs in Spotify's Development Mode — add your friends' Spotify emails in the Dashboard under User Management before they can log in.
