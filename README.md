# WGRALGO Guardians of Health &amp; Recovery

Guardians of Health &amp; Recovery is a free educational Android app from The Wealth Gap Resolution Algorithm&trade; Inc. It helps users practice health, recovery, ethics, confidentiality, and pharmacology awareness through randomized 10-question quiz rounds.

The app is fully offline, contains no ads, no analytics, no trackers, and asks for no permissions beyond what Android automatically grants.

Companion to the web concept at <https://thewealthgapresolutionalgorithm.org/guardians-of-health-recovery/>.

---

## Features

- 60+ built-in CASAC-style practice questions
- Four rotating categories: CASAC Practice, Ethics, Confidentiality, Pharmacology / Health Awareness
- Randomized 10-question rounds with shuffled answer choices
- Instant feedback after each answer, including explanation and a short learning tip
- Score tracking, category-level strengths and weak spots, and a rating on round completion
- Play Again replays a fresh randomized round
- Premium black-and-gold WGRALGO design language with green health accents
- Phone and tablet responsive layout
- Fully offline: no internet permission, no network calls
- No accounts, no ads, no analytics, no trackers

## Screenshots

Screenshots of the home, how-it-works, quiz, feedback, and round-complete screens belong in [`/screenshots`](./screenshots).

## How to install / sideload the APK

1. Download `GuardiansOfHealthRecovery-v1.0.0.apk` from the [GitHub Releases](../../releases) page.
2. On your Android device, allow installs from your browser or file manager (Settings &rarr; Apps &rarr; Special access &rarr; Install unknown apps).
3. Open the downloaded APK and tap **Install**.
4. Optional integrity check (Linux/macOS):
   ```bash
   sha256sum GuardiansOfHealthRecovery-v1.0.0.apk
   ```
   Compare the output with `GuardiansOfHealthRecovery-v1.0.0.apk.sha256` from the same release.

## How to build from source

Requires Node.js 18+, Java 17, and the Android SDK.

```bash
git clone https://github.com/WGRALGO/WGRALGO-Guardians-of-Health-Recovery.git
cd WGRALGO-Guardians-of-Health-Recovery
npm install
npx cap sync android
cd android
./gradlew assembleDebug
```

The debug APK lands at `android/app/build/outputs/apk/debug/app-debug.apk`.

### Signed release build

Release signing uses `android/keystore.properties` **or** environment variables (`GOHR_KEYSTORE_FILE`, `GOHR_KEYSTORE_PASSWORD`, `GOHR_KEY_ALIAS`, `GOHR_KEY_PASSWORD`). The keystore and its passwords are **never** committed to git.

```bash
npx cap sync android
cd android
./gradlew assembleRelease
```

Output: `android/app/build/outputs/apk/release/app-release.apk`.

## Privacy summary

- No account required
- No ads
- No analytics
- No trackers
- No cloud upload
- No data selling
- No personal health information is collected
- No quiz answers or scores are sent to WGRALGO
- The app is an offline educational health-and-recovery quiz

Full statement: [PRIVACY.md](./PRIVACY.md).

## Educational disclaimer

Guardians of Health &amp; Recovery is for educational awareness and practice only. It does not provide medical, mental health, legal, counseling, substance use treatment, crisis intervention, or professional certification advice. It does not replace official CASAC coursework, supervision, exam preparation, clinical training, or guidance from qualified professionals. If someone may be experiencing a medical emergency, overdose, withdrawal emergency, or crisis, contact emergency services or a qualified professional immediately.

## License

This project is released under the GNU General Public License v3.0. See [LICENSE](./LICENSE).

## Contributors

See [CONTRIBUTORS.md](./CONTRIBUTORS.md).
