SaXhamAI Blog - Operations Manual 🚀

**Project:** Professional Static Blog for SaXhamAI  
**Owner:** Nitin Pawar (Founder)  
**Location:** Navi Mumbai, India  
**Tech Stack:** HTML5, CSS3, Git (GitHub Pages)  

---

## 📂 1. Project Folder Structure (Naksha)

Understanding where files are located is critical for maintaining the site.

```text
Saxhamai-bolgs/
│
├── index.html                  🏠 HOMEPAGE (Hero section + Latest 3 articles)
├── about.html                  👤 ABOUT PAGE (Profile & Mission)
├── contact.html                📞 CONTACT PAGE (Email & Ecosystem links)
├── resources.html              🛠️ RESOURCES (Checklists & Tools)
│
├── sitemap.xml                 🤖 SEO MAP (List of all pages for Google)
├── robots.txt                  🤖 BOT PERMISSIONS (Allows Google to crawl)
│
├── assets/
│   └── css/
│       └── style.css           🎨 GLOBAL STYLES (Colors, Fonts, Mobile Layout)
│
└── blog/
    ├── index.html              📚 ARCHIVE PAGE (List of ALL blog posts)
    ├── why-trust-matters.html  📄 Article 1
    ├── google-maps-mistakes.html 📄 Article 2
    └── ... (New posts go here)

📝 2. SOP: How to Add a New Blog Post
Follow this checklist strictly to publish a new article without breaking the design.
✅ Step 1: Create the Article File
 * Go to the blog/ folder.
 * Copy an existing file (e.g., google-maps-mistakes.html).
 * Paste it and Rename it to your new topic.
   * Rule: Use lowercase and dashes only.
   * Example: linux-server-security.html
✅ Step 2: Edit the Code (HTML)
Open your new file in a code editor and update these 5 specific lines:
 * Title:
   <title>Your New Headline Here | SaXhamAI</title>
 * Description:
   <meta name="description" content="Write a 2-line summary for Google here.">
 * Canonical URL:
   <link rel="canonical" href="https://blog.saxhamai.com/blog/linux-server-security.html">
 * Publish Date:
   Update text: Published on Jan 15, 2026 • By Nitin Pawar
 * Schema (JSON-LD):
   Update "headline", "datePublished", and "description" inside the <script> tag.
✅ Step 3: Update the Blog Archive
 * Open blog/index.html.
 * Copy one <article class="blog-card">...</article> block.
 * Paste it at the TOP of the list (inside <div class="blog-grid">).
 * Update the Heading, Short Description, and Link (href).
✅ Step 4: Update the Homepage (Optional)
 * Open index.html (Root folder).
 * If this is a major post, replace the oldest card in the "Latest Articles" section with this new one.
✅ Step 5: Update SEO (Sitemap)
 * Open sitemap.xml (Root folder).
 * Add a new block at the bottom:
   <url>
   <loc>[https://blog.saxhamai.com/blog/linux-server-security.html](https://blog.saxhamai.com/blog/linux-server-security.html)</loc>
   <lastmod>2026-01-15</lastmod>
   <priority>0.8</priority>
</url>

🚀 3. Deployment Commands (Git)
Once you have saved all files, open your terminal/command prompt and run:
# 1. Check which files changed
git status

# 2. Add all changes to staging
git add .

# 3. Save changes with a message
git commit -m "Added new blog post: [Topic Name]"

# 4. Upload to live server
git push origin main

🎨 4. Design Guidelines (Style.css)
Do not change colors randomly. Use these CSS variables to maintain brand consistency.
 * Primary (Navy Blue): var(--primary) → #0f172a
 * Accent (Bright Blue): var(--accent) → #2563eb
 * Background (Light Grey): var(--bg-light) → #f8fafc
 * Mobile Layout: The site uses .cols-2 class to automatically stack content on mobile devices.
📞 Support & Maintenance
Maintained by: Nitin Pawar
Ecosystem: SaXhamOps | TechnoStar Infotech

