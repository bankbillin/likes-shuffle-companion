# Likes Shuffle Companion

A local-first Opera extension and optional companion service for improving SoundCloud library playback and playlist workflows.

## Security model

SoundCloud app credentials, OAuth tokens, and user library data must never be committed. The browser extension must not contain a SoundCloud client secret. A local companion process will handle OAuth token exchange and keep secrets in Windows-protected storage. The extension will communicate only with that local process.

## Current status

- SoundCloud API app registration is pending a real public project URL and successful GitHub connection.
- No SoundCloud credentials, tokens, or account data are stored in this repository.
- Full Likes retrieval and True Shuffle playback are not yet verified.

## Feasibility gate

Before building the wider UI, verify paginated retrieval of `/me/likes/tracks` using documented OAuth, then verify track playback through documented SoundCloud playback/widget methods. Shuffle must only be called complete after every Likes page is indexed. Any unavailable, blocked, or non-playable item must be handled explicitly.

## Development

Development setup and Opera loading instructions will be added after the API and playback proof of concept is verified.
