# AR Desk Pet — concept + prototype

**Concept:** point your phone at a marker on your desk, a small creature pops up on top of it. Tap the screen to feed it — it pulses, spins, and levels up (grows, changes color) every 5 feeds. No app install, runs straight in the phone browser.

**Why it's fun:** zero setup for the person testing it beyond "print this marker and open this link" — instant payoff, tactile (feeding), collectible progression (levels/colors).

**Tech:** single HTML file, A-Frame + AR.js (marker-based), Web Audio for feedback beeps. No 3D model files, no build step.

## Test it on your phone (camera needs HTTPS, so pick one)

1. **Glitch (fastest):** go to glitch.com → New Project → Hello Webpage → replace `index.html` with the contents of `ar-desk-pet.html` → open the live link on your phone.
2. **Netlify Drop:** go to app.netlify.com/drop → drag `ar-desk-pet.html` (rename it `index.html` first) → get instant HTTPS link.
3. **GitHub Pages:**
   - Create a new public repo on github.com.
   - Upload `ar-desk-pet.html`, renamed to `index.html` (plus this README if you like), and commit.
   - Go to Settings → Pages → Source: "Deploy from a branch," branch `main`, folder `/ (root)` → Save.
   - Wait ~30–60 seconds, refresh the Pages settings page for your live URL (`https://yourusername.github.io/reponame/`).
4. Print a **Hiro marker** (search "AR.js hiro marker" or grab it from the AR.js GitHub repo `data/images/hiro.png`) and lay it flat.
5. Open the link on your phone, allow camera access, point at the marker, tap to feed.

## Where to take it next (if it lands well)
- Swap the primitive-shape pet for a low-poly GLTF model for a nicer look.
- Multiple markers = multiple pets / a "collection."
- Face-tracking version instead of marker (no printout needed) using AR.js face mode or MediaPipe.
