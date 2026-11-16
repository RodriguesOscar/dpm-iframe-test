# DPM iframe test host

Run `python3 -m http.server 8000 --bind 127.0.0.1` from this directory and open [the local preview](http://127.0.0.1:8000/).

Upload `index.html` and `styles.css` to the same directory in your static web root. The page loads DM Sans from Google Fonts and falls back to a local sans-serif font.

The **DPM iframe configuration** comment in `index.html` marks the iframe element. The iframe points to `https://dpm.ids-kiel.de/home`. The dashboard server must permit the test host origin to frame this page. The width and height attributes set the desktop footprint, and CSS constrains the width on smaller screens. The header is a visual mock-up.

Configure the host and dashboard framing policies and any consent behavior once the deployment origins are known. Verify the real embed from the deployed host.
