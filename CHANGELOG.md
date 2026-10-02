# Changelog

## v2.0.0 — 2026-10-02
- New question bank from the latest web version: 90 questions across
  Beginner, Everyday, and Helper, plus an All Levels round; topics from
  overdose safety to ethics and boundaries; myth busters; results by topic;
  a "Need help now?" card with 911, 988, and the SAMHSA National Helpline.
- Real app look: black launch screen with the big app logo (no white box on
  Android 12+), a bigger launcher icon sized for round, squircle, and square
  shapes, solid app bar, and About / Privacy / Credits panels.
- `assets/icon.png` and `assets/splash.png` now hold this app's logo (they
  held the company seal); `tools/build-icons.py` builds every icon from it.
- Android back button asks before quitting a round, returns to the level
  picker from results, and asks before exiting.
- Phones and tablets, portrait and landscape: rotates freely, smaller
  start-screen logo on landscape phones.
- Removed the social, fundraising, and "Back to games" links from the new web
  version; a content security policy blocks all network access.
- The `INTERNET` permission that Capacitor merges in is now stripped from the
  final manifest.
- APK renamed to `WGRALGO-GuardiansOfHealthRecovery-v2.0.0.apk`, the same
  `WGRALGO-<AppName>-v<version>.apk` naming as every WGRALGO app.
- Version 2.0.0 (versionCode 200). Signed with a new key: uninstall v1.0.0
  before installing v2.0.0.
- Fixed `package.json` (it was named "spot-the-scam" with an ISC license);
  `.gitignore` now excludes keystores and secrets.
- Added GitHub Actions debug builds, a signed release workflow, and
  `tools/validate-release.sh`.

## v1.0.0
- Initial GitHub-ready Android APK release.
- Added offline health-and-recovery educational quiz.
- Added randomized 10-question rounds.
- Added CASAC Practice, Ethics, Confidentiality, and Pharmacology categories.
- Added score tracking, instant feedback, explanations, and learning tips.
- Added round complete screen with rating and weak spot review.
- Removed website navigation, social media, and fundraising bars from APK interface.
- Added GPLv3 license, privacy statement, contributors file, and README.
