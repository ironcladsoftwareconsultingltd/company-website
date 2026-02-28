# Ironclad Software Consulting – Bootstrap website

A single-page site built with **Bootstrap 5** and your existing Wix content. You can open it locally in a browser or copy it into Wix.

---

## View locally

1. Open `index.html` in a browser (double-click or drag into Chrome/Safari/Firefox), or  
2. From the project folder run:  
   `python3 -m http.server 8000`  
   then go to **http://localhost:8000**

---

## Replace your existing Wix site with this

You have two main options. Both keep your current domain (e.g. ironcladsoftwareconsultingltd.co.uk) on Wix.

---

### Option A: Embed this design (recommended)

Your Bootstrap site needs to be **online** first so Wix can load it inside an embed. Then you make that embed your homepage.

**Step 1 – Host this folder**

- **Netlify (easiest):** Go to [netlify.com](https://www.netlify.com), sign up (free), then drag and drop your **entire `ironclad-website` folder** (with `index.html`, `styles.css`, and `ironclad_software_consulting_ltd_logo.jpg` inside) onto the Netlify dashboard. You’ll get a URL like `https://something.netlify.app`.
- **GitHub Pages:** Push this folder to a GitHub repo, then in the repo go to Settings → Pages → set source to “main” and the folder (or root). You’ll get `https://yourusername.github.io/repo-name/`.
- **Vercel / other:** Same idea: connect the folder or repo and get a public URL.

**Step 2 – In Wix**

1. Open your site in the **Wix Editor**.
2. Open the **page you want to replace** (usually your homepage) or create a new page.
3. **Add** → **Embed** → **Embed a Site** (or “HTML iframe” / “Custom embed”).
4. Paste the **URL** from Step 1 (e.g. your Netlify or GitHub Pages URL).
5. Resize the embed so it fills the whole page (drag corners to full width and height).
6. **Hide the Wix header and footer** on this page (Page settings or right‑click the header/footer and hide).
7. If this page is not your homepage, go to **Settings** → **Pages** and set it as the **homepage**.
8. **Publish** the site.

Visitors will see this Bootstrap design when they go to your domain. The URL stays your Wix domain; the content is your new site in an embed.

---

### Option B: Rebuild the content inside Wix

No hosting needed. You rebuild the layout in Wix and paste the text from this project.

1. In the Wix Editor, **add sections** for: Hero, About, Services, Our Story, What we’re about, Contact, Footer.
2. Open `index.html` in a text editor and **copy the text** from each section into the matching Wix text boxes (headings and paragraphs).
3. Add your **logo** in the header (upload `ironclad_software_consulting_ltd_logo.jpg` in Wix).
4. Optional: **Settings** → **Custom Code** → add a snippet in **Head** with `<style> … </style>` and paste the contents of `styles.css` inside so colours and spacing are closer to this design.
5. Use Wix’s layout and styling to get a similar look (columns, buttons, cards).
6. **Publish**.

Result: everything lives in Wix and you can edit it there; the look will be similar but not identical to this Bootstrap version.

---

## What’s in the project

| File         | Purpose                                      |
|--------------|----------------------------------------------|
| `index.html` | Full page: structure, content, Bootstrap CDN |
| `styles.css` | Extra styling (colors, hero, cards, footer)  |
| `logo.svg`   | Old placeholder shield (replaced by your logo)       |
| `company-logo.png` | **Your company logo** – see below              |
| `README.md`  | This file                                    |

**Using your LinkedIn company logo**

1. Go to [your company page](https://www.linkedin.com/company/ironclad-software-consulting-ltd).
2. Right‑click the company logo and choose **Save Image As…**
3. Save it in this folder as **`company-logo.png`** (or `.jpg` if you prefer).
4. If you use a different filename, change the `src="company-logo.png"` in `index.html` in all three places (navbar, hero, footer).

The site uses your logo in the navbar, hero, and footer. PNG or JPG is fine; 400×400 or similar works well.

Bootstrap is loaded from the CDN in `index.html`, so you don’t need to install anything to view it locally.

---

## Tweaks

- **Colors**: Edit the `:root` variables in `styles.css` (e.g. `--ironclad-primary`, `--ironclad-accent`).
- **Content**: Edit the text directly in `index.html` in the relevant sections.
- **Contact**: Update the phone and email in the Contact section and footer in `index.html`.

Once you’re happy, use Option A or B above to bring it into Wix.
