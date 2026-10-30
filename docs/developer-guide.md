# Developer integration guide

This document gives high-level guidance for developers working on Nekomo integrations.

## Keep responsibilities separate

Where practical, keep these concerns independent:

- **Catalogue metadata:** titles, descriptions, artwork, identifiers, and tracking.
- **Source discovery:** finding available catalogues or providers.
- **Content resolution:** retrieving playable or readable content from a selected provider.
- **Presentation:** displaying results consistently across devices.

This separation helps the app retain useful catalogue information even when an individual source has incomplete metadata.

## Compatibility

Document the upstream ecosystem/API version, Nekomo version, Android requirements, supported features, and known limitations. Handle upstream failures gracefully and avoid assuming that every extension implements optional fields.

## Security and privacy

Treat external source responses and scripts as untrusted input. Avoid logging credentials or session data. Request only the permissions needed for the integration and validate data before displaying or processing it.
