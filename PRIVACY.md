---
layout: default
---

# Porsuk privacy policy

Updated: October 1, 2026. Scope: local project version 1.0.2 (7).

## Local account and app data

The project's documented Sign in with Apple flow stores the Apple user identifier, display name and email if Apple provides them. Favorites and user-added campsite photos, reviews and information suggestions are documented as local device data; they are not shared with other users by the documented local flow.

Settings > Delete Account clears the local session, favorites and local contributions on this device. Removing the app removes local app data.

## Location

Location permission is used when you choose nearby sorting. The documented local flow does not sell location data or use it for advertising.

## Campsite data and optional photos

Porsuk includes a bundled campsite catalog compiled from open sources, offline imports and manual review. Bundled source data is separate from your personal app data.

The project also supports an optional HTTPS backend photo proxy. If a deployment enables it, opening eligible campsite details may request a photo from that configured backend and its photo provider. This is separate from local user-added photos. The request identifies the campsite, and the network service can receive normal connection metadata, such as an IP address. The iOS app is configured without a Google Maps API secret; provider credentials belong on the backend.

Whether the proxy or other server-backed functionality is enabled in the currently distributed app has not been verified in this update. This policy describes the documented local project and optional configuration.

## Contact and external services

Links, sign-in providers and email use their respective external services. Information voluntarily sent by support email or public GitHub issues is handled by those services.

Privacy questions: **emircanby@gmail.com**.
