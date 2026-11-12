# FuzzyCritter
A private, browser-based classroom sound companion built for Rawafid students.

## Use
Serve this folder over HTTPS (or localhost). No build command or dependencies. For Netlify select this repository, leave the build command empty, and set publish directory to `.`.

Choose a koala, cat, bear, or bunny, then choose Quiet work or Partner talk and a session length. Start and allow microphone access. Calibrate for five seconds at the desired classroom volume, then adjust the target if needed. The 0–100 meter is relative microphone intensity, not calibrated decibels. Devices and microphone placement affect readings.

Thirty cumulative seconds below the target earns one star, up to five per session. Earned progress is never removed. Teacher talking, Pause, breathing breaks, calibration, and hidden tabs suspend session timing and rewards. Resume explicitly after returning to a hidden tab. Finish stops microphone access and shows the session summary. Projector view hides teacher settings. Demo uses simulated audio, with no microphone.

Names, colors, and session results are held in memory and clear on reload. No audio recordings, uploads, accounts, analytics, or student data. Use a pet name rather than a student's name. Microphone permission requires HTTPS or localhost. A blocked or missing microphone has a demo fallback.

## Development
Run `python3 -m http.server 8000` and open http://localhost:8000. Files: index.html, style.css, app.js. No external assets or network dependencies. Original CSS characters and visual design. Supports narrow screens, keyboard navigation, and reduced-motion preferences.
