# Selector releases

Builds and the Sparkle appcast for [Selector](https://github.com/Erikemmer/Selector),
a Mac-only photo culling app. Selector's source stays in the private repo;
only finished builds and the update feed live here, so anyone can install
or update the app without needing access to the source.

## Installing

1. Download the latest `.dmg` from [Releases](../../releases).
2. Open it and drag Selector into Applications.
3. **First launch, before a Developer ID signature exists:** the build is
   ad-hoc signed, not notarized, so Gatekeeper will refuse a plain double-click
   ("Selector is damaged and can't be opened" or similar). Right-click (or
   Control-click) the app in Applications and choose **Open**, then confirm
   in the dialog that appears. This step is only needed once per version;
   it goes away once the app is signed with a Developer ID and notarized.

## Updates

Selector checks this repo's `appcast.xml` for new versions (`Selector ▸
Check for Updates…`). Automatic checking is on by default; nothing installs
without confirming first.

## What's here

- `appcast.xml` — the stable update feed.
- `appcast-beta.xml` — release-candidate builds, for anyone who opted into
  pre-releases.
- Release assets (`.zip` and `.dmg`) attached to each GitHub release.
