[README.md](https://github.com/user-attachments/files/34746988/README.md)
# ALJO ANDRADE — Editable Portfolio Website


This is an **original implementation**, using its own HTML, CSS, JavaScript, text, geometric artwork and interface mockups. No images, project code, or personal details were copied from the reference site.

## How to open

1. Unzip the portfolio folder.
2. Double-click **index.html** to preview it in your browser.
3. To edit it, open the folder in Visual Studio Code or another text editor.

No installation, account, or web framework is needed. The font loads from Google Fonts online, with local system-font fallback offline.

## What to personalize

**1. Your email, social links, and photo**: At the TOP of `script.js`, edit `SITE_CONFIG`:

```js
const SITE_CONFIG = {
  email: 'your-real-email@example.com',
  github: 'https://github.com/your-username',
  linkedin: 'https://www.linkedin.com/in/your-profile',
  instagram: '',
  profileImage: 'assets/aljo-andrade-portrait.jpg'
};
```

Your original photograph is included unchanged at `assets/aljo-andrade-portrait.jpg` and is displayed prominently in the hero section. Replace that file to update your photograph. Your email and social links are still blank.

**2. Main introduction and About section**: Edit the visible text in `index.html`, especially `#home` and `#about`.

**3. Project entries**: Edit each card in `index.html`. Change project names, card previews, captions, and `data-category` values. Edit the matching project descriptions inside the `projects` object in `script.js`. The six supplied entries are **academic ideas/concepts**, not verified completed projects; update their completion statuses truthfully.

**4. Colors**: At the top of `styles.css`, change `--paper`, `--accent`, `--ink`, and other CSS variables.

**5. Work process and contact text**: Edit the `#process` and `#contact` sections of `index.html`.

## Features

- Responsive homepage, about, projects, process, contact, and footer
- Sticky navigation and mobile menu
- Filterable project cards
- Clickable project detail dialog with Escape and keyboard focus support
- Contact form that opens a visitor's email app (`mailto:`)
- Editable contact links and photograph
- Modern design with no build dependencies

**Important:** The form does NOT send email from a backend. It prepares an email in the visitor's preferred email app. Set `SITE_CONFIG.email` first. The site does not capture, store, or transmit form information to a server.

## How to put it online with GitHub Pages (free)

1. Sign in to GitHub and create a new public repository, for example `aljo-portfolio`.
2. Upload **index.html**, **styles.css**, **script.js**, **README.md**, and the **assets** folder to the root of your repository.
3. Commit your files to the default branch.
4. Under **Settings → Pages**, choose **Deploy from a branch**, choose your default branch and **/(root)**, then save.
5. Once GitHub Pages finishes deploying, your address should follow the pattern `https://YOUR-GITHUB-USERNAME.github.io/aljo-portfolio/` (replace the placeholder with your actual username and repository name).

Your site is not live on the internet until you publish it using a host. Opening the HTML file locally does not create a public URL.

## What can be updated next

- Real photo and contact details
- Genuine screenshots and demo links for completed projects
- Resume download link
- Education timeline, awards, certifications, internship experiences
- A working backend contact form if needed
