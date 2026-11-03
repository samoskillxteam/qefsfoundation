# How to Add New Outreaches to the Website

The outreach showcase page (`outreach.html`) is designed to be modular and scalable. Each outreach is self-contained.

---

### Step 1: Add Media for the New Outreach
1. Create a new folder inside `images/outreach/` named after your location or mission:
   - Example: `images/outreach/gwarinpa-abuja/`
2. Place your photos and videos inside this folder.
   - Example:
     - `photo-1.jpg`, `photo-2.jpg`, ...
     - `video-1.mp4`, `video-2.mp4`, ...

---

### Step 2: Add a Quick Navigation Pill
Open `outreach.html` and locate the `<!-- Outreach Quick Navigator -->` section around line 400.
Add a new pill pointing to your outreach section ID:

```html
<a href="#outreach-gwarinpa" class="outreach-nav-pill">
    <i class="fa-solid fa-location-dot text-warning"></i>
    <span>Gwarinpa Community Outreach, Abuja</span>
    <span class="badge-accent">Outreach 02</span>
</a>
```

---

### Step 3: Duplicate the Outreach Card Block
In `outreach.html`, copy the block starting at:
`<!-- OUTREACH #01: CHIEF PALACE IJAYAPI ... -->`
down to the closing `</div>` of `.outreach-card`.

Paste it directly below Outreach 01 and update:
1. **`id` attribute**: e.g., `<div id="outreach-gwarinpa" class="outreach-card">`
2. **Title, Location, Date**:
   - Location: e.g. "Gwarinpa Village, Abuja FCT"
   - Date: e.g. "December 2026"
3. **Story & Metrics**:
   - Update the paragraph descriptions and the 4 impact counters (Beneficiaries, Packages, etc.).
4. **Media Grid & Filter**:
   - Update `data-target="gwarinpa"` on `.media-filter-nav`
   - Update `id="gwarinpa-media-grid"` on `.gallery-items`
   - Update the image `src`, `href`, video `src`, and captions.

---

### Step 4: Save & Preview
Open `http://localhost/Queen/outreach.html` (or your domain) to verify the new outreach, filter tabs, photo zoom popup, and videos.
