# Well Crafted Communications – Portfolio Management & Workflow

_A living document tracking site maintenance, updates, and configuration._

---

## 🌐 DNS Reference (Live Configuration)

| Type | Name | Data / Points To | TTL | Purpose / Notes |
|------|------|------------------|------|----------------|
| **A** | @ | 185.199.108.153 | 1 Hour | GitHub Pages server (1 of 4 official IPs) |
| **A** | @ | 185.199.109.153 | 1 Hour | GitHub Pages server |
| **A** | @ | 185.199.110.153 | 1 Hour | GitHub Pages server |
| **A** | @ | 185.199.111.153 | 1 Hour | GitHub Pages server |
| **CNAME** | www | ctt1953.github.io | 1 Hour | Points www → GitHub Pages site |
| **CNAME** | _domainconnect | _domainconnect.gd.domaincontrol.com | 1 Hour | GoDaddy system record (do not remove) |
| **MX** | @ | smtp.secureserver.net (Priority 0) | 1 Hour | Primary GoDaddy mail server |
| **MX** | @ | mailstore1.secureserver.net (Priority 10) | 1 Hour | Backup GoDaddy mail server |

**Do not include:**  
- Squarespace (`ext.squarespace.com`)  
- FTP, POP, IMAP, SMTP CNAMES  
- GoDaddy forwarding (redirect loop risk)

_Last verified: November 2025_

---

## 🧭 GitHub + VS Code Workflow

| Step | Action | Notes |
|------|---------|-------|
| 1 | **Pull origin** | Always start in GitHub Desktop and pull latest repo updates. |
| 2 | **Open in VS Code** | Repository → “Open in Visual Studio Code.” |
| 3 | **Edit** | Add `workcard`, `testimonial`, or `clientlite` snippet in `index.html`. |
| 4 | **Save & Preview** | Click **Go Live** in VS Code to view changes locally. |
| 5 | **Commit Changes** | GitHub Desktop → add short, clear message (“Added testimonial for Jet Edge”). |
| 6 | **Push Origin** | Publishes site to GitHub Pages in ~1 minute. |
| 7 | **Verify Live Site** | Check both `wellcraftedcommunications.com` and `www.wellcraftedcommunications.com`. |

---

## 🧩 Snippet Reference

| Prefix | Function | Output |
|---------|-----------|---------|
| `workcard` | Adds a new portfolio card in the grid | `<div class="card">...</div>` |
| `testimonial` | Inserts client quote card | `<div class="card testimonial">...</div>` |
| `clientpage` | Full-page template for client-specific project | Complete HTML structure |
| `clientlite` | Lightweight client page template | Shorter version for quick pages |

---

## 🎨 Portfolio Update Checklist

- [ ] Add new project card using `workcard` snippet.  
- [ ] Confirm logo files in `/assets/logos/`.  
- [ ] Test layout in desktop and mobile view.  
- [ ] Commit and push updates.  
- [ ] Verify DNS table (if domain issues arise).  
- [ ] Update this Markdown file as needed.  

---

## 🧱 Local Folder Structure

---

## 🖼️ Logo Prep Guidelines

When preparing client logos for the **Trusted By** grid:

| Step | Action | Recommendation |
|------|---------|----------------|
| 1 | **File Format** | Prefer **SVG** for crisp scaling. Use **PNG (transparent background)** if SVG isn’t available. |
| 2 | **File Naming** | Use lowercase, no spaces, underscores optional. Example: `jetedge.svg`, `carlsoncaspers.png`. |
| 3 | **Dimensions** | 250–300px width; 100px height or less for consistent alignment. |
| 4 | **Color Mode** | Convert to grayscale or desaturate color logos to 80–90% opacity for visual harmony. |
| 5 | **Storage Folder** | Place all logo files in `assets/logos/` within your repo. |
| 6 | **HTML Reference** | Example snippet:  
```html
<img src="assets/logos/jetedge.svg" alt="Jet Edge Waterjets logo">
``` |
| 7 | **Testing** | Open `index.html` in VS Code → **Go Live** → verify logos appear evenly spaced. |

💡 *Tip:* You can use a free tool like [Photopea](https://www.photopea.com) or [TinyPNG](https://tinypng.com) to resize and desaturate images before upload.

---

## 🧩 Notes
- Markdown files (`.md`) display beautifully in GitHub and VS Code.  
- You can preview this file in VS Code with **Ctrl+Shift+V**.  
- For GitHub display, rename it to **`README.md`** if you want it to appear automatically when you open your repo online.  

---

**© 2025 Tom Tate | Well Crafted Communications**  
*Maintaining excellence, one card at a time.*
