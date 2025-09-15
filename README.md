SnowPlow Services – Static Website

SnowPlow is a simple, single‑page marketing website for a student‑run snow plowing service based in Camrose, Canada. It is built using only plain HTML and CSS, making it easy to customise and deploy on any static host. The site advertises the business, outlines various service plans, showcases recent work, tells visitors about the company and includes a contact form that forwards enquiries via Formspree.

🧰 Features

The site consists of an index.html file and a main.css stylesheet. Together they provide the following sections:

Header and hero

A fixed header with a logo title “Snow Plow Services Camrose” and navigation links (Home, Plans, Gallery, About, Contact)
raw.githubusercontent.com
.

A hero section with a headline (“Fast, Reliable Snow Plowing”) and a short tagline introducing the business
raw.githubusercontent.com
. The hero uses a snowy landscape image as a background with a dark overlay for contrast
raw.githubusercontent.com
.

Pricing table

A responsive pricing table showing four plans: Pay‑As‑You‑Go, Silver, Gold and Platinum
raw.githubusercontent.com
. Each row lists features like on‑demand snow removal, deicing, scheduled visits, two‑car coverage and emergency support, with tick marks or prices to indicate what’s included
raw.githubusercontent.com
.

Below the table is an “Exclusive Offers” box with referral and seasonal promotions
raw.githubusercontent.com
.

A footnotes section explains key service details such as two‑car coverage, emergency response times, appointment policies and pricing assumptions
raw.githubusercontent.com
.

Gallery

Three images (snowplow1.jpg, snowplow2.webp, snowplow3.jpg) showcase recent snow removal work
raw.githubusercontent.com
. The gallery uses flexbox to align the thumbnails and adds subtle shadows via CSS
raw.githubusercontent.com
.

About

An About section explains that SnowPlow is a student‑run service created to provide reliable, affordable snow removal for the local community
raw.githubusercontent.com
. It emphasises dedication, promptness and a friendly attitude.

Contact

A simple contact form collects the visitor’s name, email, phone number, referral code and a message
raw.githubusercontent.com
.

Form submissions are sent to a Formspree endpoint (https://formspree.io/f/mkggajvo) via a POST request
raw.githubusercontent.com
. You can replace this URL with your own Formspree form ID or backend endpoint.

Footer

The footer displays a copyright notice with the current year and business name
raw.githubusercontent.com
.

🗂 Directory structure
SnowPlow/
├── index.html    # main HTML file containing all sections:contentReference[oaicite:13]{index=13}
├── main.css      # stylesheet defining layout, colours, fonts and responsive styles:contentReference[oaicite:14]{index=14}
├── background*.jpg/jpeg # various background images used across the site
├── snowplow*.jpg/.webp  # gallery images
└── LICENSE       # GNU GPL v3 licence

🚀 Getting started

No special tooling is required: the site is completely static. To view it locally, clone the repository and open index.html in your browser:

git clone https://github.com/rcc00n/SnowPlow.git
cd SnowPlow
# open index.html in your browser of choice


If you prefer to serve it over HTTP (useful for testing forms), run a simple static server:

# using Python’s built‑in server
python3 -m http.server 8000
# then visit http://localhost:8000 in your browser

🎨 Customisation

Change branding: Edit the title and headings in index.html to reflect your business name and tagline
raw.githubusercontent.com
. Replace background6.jpg or the hero background URL in the CSS with your own imagery
raw.githubusercontent.com
.

Modify plans: Update the table rows to alter pricing, visit counts or add additional features
raw.githubusercontent.com
. Adjust colours in the .check and .xmark classes (green and red by default) to match your brand
raw.githubusercontent.com
.

Update offers and footnotes: Edit the <div class="offers-box"> content and the <ul> inside the footnotes to change promotions and service details
raw.githubusercontent.com
.

Swap gallery images: Replace snowplow1.jpg, snowplow2.webp and snowplow3.jpg with your own photos; ensure the filenames match the references in index.html
raw.githubusercontent.com
.

Update contact form: Substitute the action attribute’s Formspree URL with your own endpoint or remove it to handle submissions differently
raw.githubusercontent.com
. You can also add fields as needed.

Tweak styles: Modify colours, fonts and layout in main.css. The Poppins font is loaded via Google Fonts
raw.githubusercontent.com
. The CSS contains comments and section headings to help you find specific rules.

📦 Deployment

The project is ready for deployment on any static hosting service (GitHub Pages, Netlify, Vercel, etc.). For GitHub Pages, push the repository to GitHub and enable Pages under the repository settings. Netlify and Vercel can auto‑detect static sites—simply connect your repository and set the build command to null since there is no build step.

🪪 Licence

This project is licensed under the GNU General Public License v3.0. Please review the LICENSE file for the full terms of redistribution and modification.

SnowPlow was created as part of a student project; feel free to adapt it for your own local business or volunteer service.
