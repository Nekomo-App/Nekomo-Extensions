# Adding external sources

Nekomo works with external sources and extensions; this repository does not distribute or host them.

1. Find the source through its official developer or project channel.
2. Check that it supports the relevant extension ecosystem and your Nekomo version.
3. Review its permissions, publisher, and release information.
4. Follow the source developer's installation instructions and Nekomo's in-app guidance.
5. Test the source and report compatibility results with version details.

Only install software from sources you trust. Availability and installation steps may differ by ecosystem and Android version.

## Installing from inside Nekomo

Nekomo ships with no sources installed. Open **Settings > Extensions** to reach the Extensions manager, one place for:

- **Repositories and sources:** CloudStream plugins (`.cs3`) and Zangetsu scripts (`.js`). Enable, disable, update, uninstall, view details and per-provider switches.
- **Metadata APIs (built in):** AniList (main), Kitsu, MyAnimeList via Jikan, TVMaze and TMDB (needs your own key). Backups switch on automatically when the main API is down or rate-limited.
- **Automatic updates:** on or off, frequency (6 hours to 7 days), manual check, update all or one by one, and an update history that records every install, update, removal and error. A failed update keeps the previous version.
- **APK extensions (Aniyomi, Mihon):** listed separately. Nekomo never downloads, installs or updates these automatically; you install them yourself.

An **optional official repository** (free and legal sources only) can be added from the same screen with a repository URL or code. Nothing is installed until you add it and confirm the third-party-code warning, and you can remove it, with the sources it installed, at any time. Any other repository can be added manually by URL; Nekomo does not host or vouch for those.

## NEX, the companion manager

[NEX](https://github.com/Nekomo-App/NEX) (Nekomo Extension Exchange) is a separate app from the Nekomo community that manages repositories, extensions and sources for Nekomo, Mihon, Aniyomi, CloudStream and Zangetsu. It ships with no repositories, hosts nothing, and never installs silently. From NEX you can send a repository to Nekomo with one tap (Nekomo asks you to confirm), check Nekomo app updates with SHA-256 verification, and keep Mihon and Aniyomi extensions up to date. Downloads are on its [releases page](https://github.com/Nekomo-App/NEX/releases).
