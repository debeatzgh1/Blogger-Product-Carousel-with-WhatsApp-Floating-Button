<style>
  /* Catalog Styles */
  .wa-catalog {
    display: flex;
    flex-wrap: wrap;
    gap: 15px;
    padding: 15px;
    max-width: 700px;
    margin: auto;
  }
  .wa-product {
    border: 1px solid #ddd;
    border-radius: 10px;
    overflow: hidden;
    width: 160px;
    background: #fff;
    text-align: center;
    font-family: Arial, sans-serif;
    box-shadow: 0 2px 8px rgba(0,0,0,0.1);
  }
  .wa-product img {
    width: 100%;
    height: 160px;
    object-fit: cover;
  }
  .wa-product h4 {
    margin: 8px 0 4px;
    font-size: 14px;
  }
  .wa-product p {
    font-size: 12px;
    color: #555;
    padding: 0 5px;
    min-height: 32px;
  }
  .wa-product .price {
    font-weight: bold;
    color: #25D366;
    margin: 4px 0;
  }
  .wa-product button {
    background: #25D366;
    border: none;
    color: white;
    padding: 8px;
    cursor: pointer;
    width: 100%;
    font-size: 12px;
  }
  /* Floating Chat Styles */
  .wa-fab {
    position: fixed;
    right: 20px;
    top: 50%;
    transform: translateY(-50%);
    background: #25D366;
    color: white;
    border-radius: 50%;
    width: 56px;
    height: 56px;
    display: flex;
    align-items: center;
    justify-content: center;
    cursor: pointer;
    box-shadow: 0 4px 10px rgba(0,0,0,0.3);
    z-index: 9999;
    font-size: 28px;
  }
  .wa-chat-box {
    position: fixed;
    right: 90px;
    top: 50%;
    transform: translateY(-50%);
    width: 280px;
    background: white;
    border: 1px solid #ddd;
    border-radius: 8px;
    display: none;
    flex-direction: column;
    font-family: Arial, sans-serif;
    box-shadow: 0 4px 15px rgba(0,0,0,0.2);
    z-index: 9999;
  }
  .wa-chat-header {
    background: #25D366;
    color: white;
    padding: 10px;
    font-size: 14px;
    border-radius: 8px 8px 0 0;
  }
  .wa-chat-body {
    padding: 10px;
    font-size: 13px;
    color: #333;
  }
  .wa-chat-footer {
    padding: 10px;
    border-top: 1px solid #ddd;
    text-align: right;
  }
  .wa-chat-footer button {
    background: #25D366;
    border: none;
    color: white;
    padding: 6px 12px;
    font-size: 12px;
    cursor: pointer;
  }
</style>

<div class="wa-catalog" id="waCatalog"></div>

<!-- Floating Chat -->
<div class="wa-fab" id="waFab">💬</div>
<div class="wa-chat-box" id="waChatBox">
  <div class="wa-chat-header">WhatsApp Live Chat</div>
  <div class="wa-chat-body">
    Hi 👋, how can we help you today?  
    Click below to start a chat on WhatsApp.
  </div>
  <div class="wa-chat-footer">
    <button onclick="window.open('https://wa.me/233549757544','_blank')">Start Chat</button>
  </div>
</div>

<script>
(function(){
  const PRODUCTS = [
    {
      title: "Classic Leather Handbag",
      price: "₵250",
      img: "https://via.placeholder.com/160x160/E1A87B/000?text=Handbag",
      desc: "Premium leather tote for work, travel & everyday style.",
      link: "https://wa.me/p/8796681600402535/233549757544"
    },
    {
      title: "Wireless Bluetooth Headphones",
      price: "₵320",
      img: "https://via.placeholder.com/160x160/1A1A1A/FFF?text=Headphones",
      desc: "Deep bass, noise-cancelling & all-day comfort.",
      link: "https://wa.me/p/4801727346588745/233549757544"
    },
    {
      title: "Casual Sneakers",
      price: "₵180",
      img: "https://via.placeholder.com/160x160/C8E6C9/222?text=Sneakers",
      desc: "Lightweight sneakers perfect for daily wear.",
      link: "https://wa.me/p/5908362889193112/233549757544"
    },
    {
      title: "Luxury Wristwatch",
      price: "₵500",
      img: "https://via.placeholder.com/160x160/2E3B55/FFF?text=Watch",
      desc: "Elegant design with precision quartz movement.",
      link: "https://wa.me/p/5176804599022575/233549757544"
    }
  ];

  const catalogEl = document.getElementById("waCatalog");
  PRODUCTS.forEach(p => {
    const card = document.createElement("div");
    card.className = "wa-product";
    card.innerHTML = `
      <img src="${p.img}" alt="${p.title}">
      <h4>${p.title}</h4>
      <p>${p.desc}</p>
      <div class="price">${p.price}</div>
      <button onclick="window.open('${p.link}', '_blank')">Send Message</button>
    `;
    catalogEl.appendChild(card);
  });

  // Floating Chat Toggle
  const fab = document.getElementById("waFab");
  const chatBox = document.getElementById("waChatBox");
  fab.addEventListener("click", () => {
    chatBox.style.display = chatBox.style.display === "flex" ? "none" : "flex";
  });
})();
</script>


# Blogger Product Carousel with WhatsApp Floating Button

## 📌 Overview
This project displays Blogger pages in a product carousel with:
- Embedded live previews via `<iframe>`
- "Open Live Preview" buttons
- Floating WhatsApp button for instant chat

## 🚀 Live Demo
[Click here to view on GitHub Pages](https://yourusername.github.io/whatsapp-products-carousel/)

## 📂 How to Use
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/whatsapp-products-carousel.git

# 🚀 DeBeatzGH – AI Tools & Side Hustle Hub  

![DeBeatzGH Thumbnail](https://debeatzgh.wordpress.com/wp-content/uploads/2025/08/designamodernminimalisticdesignfeaturinganai-themedicon28likeabraincircuitorrobot29overlaidwithdebeatzghoraitoolshustles6089986211026037047.jpg)  

## 🌟 About  
Welcome to **[DeBeatzGH](https://debeatzgh.wordpress.com/)** — your go-to hub for **AI tools, side hustle strategies, blogging resources, and digital growth guides**.  

Our platform is built to help **students, creators, startups, and professionals** unlock the power of AI, monetize their skills, and thrive in today’s digital economy.  

### ✨ What You’ll Find  
- 💡 Explore **AI prompts, tools, and hacks**  
- 📈 Discover **side hustle strategies & online income ideas**  
- ✍️ Access **blogging & digital business guides**  
- 🚀 Stay ahead with **regular updates and fresh insights**  

---

## 👉 Get Started  
🔥 **Start your journey today → [Visit DeBeatzGH](https://debeatzgh.wordpress.com/)**  

---

<!-- README: DebeatzGH Digital Store (HTML-friendly for GitHub) -->
<div align="center">
  <a href="https://www.socialcreator.com/debeatzgh" target="_blank" rel="noopener">
    <img
      src="https://debeatzgh.wordpress.com/wp-content/uploads/2025/08/designadigitalproductse-commerceonlinedeals3545265155247625100.jpg"
      alt="DebeatzGH Digital Store"
      style="max-width:100%; border-radius:16px;"
    />
  </a>

  <h1 style="margin-top: 14px;">DebeatzGH Digital Store</h1>
  <p style="max-width:780px;">
    Your hub for AI insights, tech tutorials, side-hustle playbooks, and productivity tools.
    Learn, build, and launch digital projects faster.
  </p>

  <!-- CTAs -->
  <p>
    <a href="https://www.socialcreator.com/debeatzgh" target="_blank" rel="noopener"
       style="display:inline-block; padding:10px 16px; margin:4px; border-radius:999px; text-decoration:none; font-weight:600; border:1px solid #2563eb;">
      🚀 View Live App
    </a>
    <a href="https://github.com/debeatzgh1/Personal-Portfolio-site-" target="_blank" rel="noopener"
       style="display:inline-block; padding:10px 16px; margin:4px; border-radius:999px; text-decoration:none; font-weight:600; border:1px solid #111827;">
      ⭐ Star this Repo
    </a>
  </p>
</div>

<hr/>

<h2>Overview</h2>
<p>
  <strong>DebeatzGH</strong> helps beginners and creators build profitable digital assets:
  blogs, affiliate funnels, AI-assisted content, and more. Explore tutorials, tools, and
  ready-to-use components to speed up your workflow.
</p>

<h2>Features</h2>
<ul>
  <li><strong>AI & Tech Learning:</strong> Bite-sized guides for modern tools and workflows.</li>
  <li><strong>Side-Hustle Playbooks:</strong> Practical steps to validate and launch ideas.</li>
  <li><strong>Productivity Toolkit:</strong> Reusable widgets, templates, and scripts.</li>
  <li><strong>Beginner-Friendly:</strong> Clear explanations, curated resources, and examples.</li>
</ul>

<h2>Quick Start</h2>
<ol>
  <li>Clone:
    <pre><code>git clone https://github.com/debeatzgh1/Personal-Portfolio-site-</code></pre>
  </li>
  <li>Enter folder:
    <pre><code>cd debeatzgh</code></pre>
  </li>
  <li>Install deps (adjust to your stack):
    <pre><code># Node
npm install
npm run dev

# or Python
pip install -r requirements.txt
python app.py</code></pre>
  </li>
  <li>Open in browser:
    <pre><code>http://localhost:3000</code></pre>
  </li>
</ol>

<h2>Project Links</h2>
<ul>
  <li>🌐 Live App: <a href="https://www.socialcreator.com/debeatzgh" target="_blank" rel="noopener">socialcreator.com/debeatzgh</a></li>
  <li>🖼️ Thumbnail: <a href="https://debeatzgh.wordpress.com/wp-content/uploads/2025/08/designadigitalproductse-commerceonlinedeals3545265155247625100.jpg" target="_blank" rel="noopener">View image</a></li>
</ul>

<h2>Contributing</h2>
<p>
  Contributions are welcome! Open an issue for bugs or ideas. For changes, fork the repo,
  create a feature branch, and submit a pull request.
</p>

<h2>License</h2>
<p>
  Released under the <a href="./LICENSE">MIT License</a>.
</p>

<hr/>

<div align="center">
  <p><em>If this project helps you, consider giving it a star. It really helps! ⭐</em></p>
  <p>
    <a href="https://www.socialcreator.com/debeatzgh" target="_blank" rel="noopener"
       style="display:inline-block; padding:10px 16px; margin-top:6px; border-radius:10px; text-decoration:none; font-weight:600; border:1px solid #2563eb;">
      Open DebeatzGH Now →
    </a>
  </p>
</div>
