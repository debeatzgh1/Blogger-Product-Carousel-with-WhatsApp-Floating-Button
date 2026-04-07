
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Premium Digital Hub</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@200;400;800&display=swap" rel="stylesheet">
    <style>
        body { font-family: 'Plus Jakarta Sans', sans-serif; scroll-behavior: smooth; }
        .hero-bg {
            background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.8)), 
                        url('https://images.unsplash.com/photo-1497215728101-856f4ea42174?q=80&w=2070&auto=format&fit=crop');
            background-size: cover;
            background-position: center;
        }
        .modal-overlay {
            display: none;
            position: fixed;
            top: 0; left: 0; width: 100%; height: 100%;
            background: rgba(0,0,0,0.9);
            z-index: 1000;
            backdrop-filter: blur(10px);
        }
    </style>
</head>
<body class="bg-white">

    <div id="urlModal" class="modal-overlay">
        <div class="flex flex-col h-full w-full max-w-5xl mx-auto p-4 md:p-10">
            <div class="flex justify-between items-center mb-4">
                <h3 id="modalTitle" class="text-white uppercase tracking-widest text-xs font-bold">Previewing Resource</h3>
                <button onclick="closeModal()" class="text-white hover:text-gray-400 flex items-center gap-2 transition-all">
                    <span class="text-xs uppercase font-bold">Close</span>
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><line x1="18" y1="6" x2="6" y2="18"></line><line x1="6" y1="6" x2="18" y2="18"></line></svg>
                </button>
            </div>
            <iframe id="modalFrame" src="" class="w-full h-full rounded-lg bg-white border-0"></iframe>
        </div>
    </div>

    <section class="h-[70vh] hero-bg relative flex items-center justify-center text-center px-6">
        <div class="max-w-4xl">
            <h1 class="text-6xl md:text-9xl font-extrabold text-white tracking-tighter mb-8 uppercase leading-none">
                CAPTURE <br><span class="text-transparent" style="-webkit-text-stroke: 1px white;">THE MOMENT</span>
            </h1>
            <p class="text-gray-300 text-sm md:text-lg font-light tracking-[0.2em] uppercase mb-12">
                High Performance Business Assets & AI Solutions
            </p>
            <a href="https://beatzde4.blogspot.com/p/blog-page_10.html" 
               target="_blank"
               class="inline-block bg-white text-black px-12 py-4 text-xs font-extrabold tracking-[0.3em] uppercase hover:bg-gray-200 transition-all">
                Access Catalog
            </a>
        </div>
    </section>

    <section class="py-32 bg-white">
        <div class="max-w-7xl mx-auto px-6">
            <div class="grid grid-cols-1 md:grid-cols-3 gap-16">
                
                <div class="group">
                    <div class="h-[400px] bg-gray-100 mb-8 overflow-hidden relative cursor-pointer" onclick="openModal('https://beatzde4.blogspot.com/p/catalog-styles.html', 'Catalog Styles')">
                        <img src="https://images.unsplash.com/photo-1486406146926-c627a92ad1ab?q=80&w=800&auto=format&fit=crop" class="w-full h-full object-cover grayscale group-hover:grayscale-0 transition-all duration-700">
                        <div class="absolute inset-0 bg-black/20 group-hover:bg-transparent transition-all"></div>
                    </div>
                    <h2 class="text-2xl font-bold tracking-tight mb-2">CATALOG STYLES</h2>
                    <p class="text-gray-500 font-light text-sm mb-6 uppercase tracking-wider">Interface Design</p>
                    <button onclick="openModal('https://beatzde4.blogspot.com/p/catalog-styles.html', 'Catalog Styles')" class="text-[10px] font-black uppercase tracking-[0.2em] border-b-2 border-black pb-1 hover:text-gray-500 hover:border-gray-500 transition-all">
                        Launch Preview
                    </button>
                </div>

                <div class="group">
                    <div class="h-[400px] bg-gray-100 mb-8 overflow-hidden relative cursor-pointer" onclick="openModal('https://beatzde4.blogspot.com/p/fab-floating-button-whatsappfab.html', 'Floating Buttons')">
                        <img src="https://images.unsplash.com/photo-1551288049-bbbda536339a?q=80&w=800&auto=format&fit=crop" class="w-full h-full object-cover grayscale group-hover:grayscale-0 transition-all duration-700">
                        <div class="absolute inset-0 bg-black/20 group-hover:bg-transparent transition-all"></div>
                    </div>
                    <h2 class="text-2xl font-bold tracking-tight mb-2">FLOATING UI</h2>
                    <p class="text-gray-500 font-light text-sm mb-6 uppercase tracking-wider">Dynamic Interaction</p>
                    <button onclick="openModal('https://beatzde4.blogspot.com/p/fab-floating-button-whatsappfab.html', 'Floating Buttons')" class="text-[10px] font-black uppercase tracking-[0.2em] border-b-2 border-black pb-1 hover:text-gray-500 hover:border-gray-500 transition-all">
                        Launch Preview
                    </button>
                </div>

                <div class="group">
                    <div class="h-[400px] bg-gray-100 mb-8 overflow-hidden relative cursor-pointer" onclick="openModal('https://beatzde4.blogspot.com/p/product-1.html', 'Product Architecture')">
                        <img src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f?q=80&w=800&auto=format&fit=crop" class="w-full h-full object-cover grayscale group-hover:grayscale-0 transition-all duration-700">
                        <div class="absolute inset-0 bg-black/20 group-hover:bg-transparent transition-all"></div>
                    </div>
                    <h2 class="text-2xl font-bold tracking-tight mb-2">PRODUCT HUBS</h2>
                    <p class="text-gray-500 font-light text-sm mb-6 uppercase tracking-wider">Scalable Frameworks</p>
                    <button onclick="openModal('https://beatzde4.blogspot.com/p/product-1.html', 'Product Architecture')" class="text-[10px] font-black uppercase tracking-[0.2em] border-b-2 border-black pb-1 hover:text-gray-500 hover:border-gray-500 transition-all">
                        Launch Preview
                    </button>
                </div>

            </div>
        </div>
    </section>

    <script>
        function openModal(url, title) {
            document.getElementById('modalFrame').src = url;
            document.getElementById('modalTitle').innerText = title;
            document.getElementById('urlModal').style.display = 'block';
            document.body.style.overflow = 'hidden'; // Stop background scroll
        }

        function closeModal() {
            document.getElementById('urlModal').style.display = 'none';
            document.getElementById('modalFrame').src = '';
            document.body.style.overflow = 'auto'; // Restore scroll
        }

        // Close on ESC key
        window.addEventListener('keydown', function (e) {
            if (e.key === 'Escape') closeModal();
        });
    </script>
</body>
</html>





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
