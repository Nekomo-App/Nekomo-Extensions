# Supported formats and ecosystems

This page describes the external extension ecosystems Nekomo is designed to work with. It does not guarantee that every extension or version will work.

## CloudStream

- Extension package format: `.cs3`
- Extensions are maintained by their respective authors and repositories.
- Compatibility may depend on CloudStream APIs and the Nekomo integration version.

## Zangetsu

- Supports JavaScript-based source integrations.
- Source scripts may rely on APIs or runtime behavior that changes over time.
- Review source code and permissions before adding a source.

## Aniyomi

- Uses externally installed source APKs for anime/catalogue providers.
- Source compatibility can vary by app version, Android version, and upstream changes.

## Mihon

- Uses externally installed source APKs for manga providers.
- Reader behavior, content parsing, and source availability can vary.

## Metadata is separate

Catalog metadata (titles, artwork, descriptions, and tracking) should be handled independently from streaming or reading sources whenever possible. A source failing to provide metadata should not automatically prevent the app from displaying metadata from supported catalogue services.

## Version reporting

When documenting compatibility, include the Nekomo version, Android version, extension name, extension version, and date tested.

## Repository manifest (optional)

An external repository can be offered as a single JSON manifest that Nekomo reads when a user adds it. It must contain `"nekomoRepository": 1`, a `name`, and a `repositories` list of `{ "type": "cloudstream" | "zangetsu", "name", "url", "description" }`. Only script/plugin formats are handled. APK ecosystems (Aniyomi, Mihon) are never listed or installed by a manifest.
