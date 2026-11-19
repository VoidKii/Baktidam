# Bhakti Dham 🙏

A calm, temple-inspired naam-jap counter. Speak a devotional name and the counter advances toward 1,000.

## Run it
Open `index.html` in a modern browser, or enable GitHub Pages:
1. Open repository **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select **main** and **/ (root)**, then Save.

## Voice recognition
The site uses the browser's built-in Web Speech API (`SpeechRecognition` / `webkitSpeechRecognition`). Voice recognition availability varies by browser and device; current Chrome-based browsers are the best first try. Microphone access requires HTTPS or localhost and user permission. Browser speech recognition may send audio to the browser provider's speech service; this site has no custom audio backend.

Recognized phrases are matched against a starter list of common devotional names in Hindi and English. It is not a general-purpose Sanskrit/Hindi speech understanding model. Add more terms in `chantTerms` in `index.html` if desired.

The count is stored in this browser's localStorage on this device. It is not synced between devices.
