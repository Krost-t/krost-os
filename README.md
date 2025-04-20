# Krost-os  🖥️📱

Welcome to **krost-os**, my immersive **web application** that emulates the aesthetics and user experience of **macOS** (Aqua) and **iPadOS/iOS** (responsive with touch gestures). Each icon in the Dock or Launchpad opens a web "window" showcasing one of my development projects or skills.

---

## 🔍 Overview

![Screenshot of krost-os](path/to/screenshot.png)

🔗 **Live Demo:** [krost-os.app](https://your-domain.com)

---

## ✨ Features

- **🧭 Interactive Dock:** A bottom screen bar with hoverable and clickable icons, replicating the macOS effect.
- **🪟 Translucent Windows:** Utilises `backdrop-filter` to simulate Aqua-style blurs.
- **📱 Responsive Launchpad:** A grid of icons adaptable to touch screens (drag & drop, swipe).
- **🎞️ Smooth Animations:** Transitions crafted with Framer Motion.
- **♿ Accessibility:** Keyboard navigation, ARIA roles, and focus management.
- **🛠️ Technologies:** React, Tailwind CSS v4.1, Framer Motion, CSS Modules.&#8203;:contentReference[oaicite:0]{index=0}

---

## ⚙️ Installation & Start-up

1. **Clone the repository:**

   ```bash
   git clone https://github.com/your-username/krost-os.git
   ```

2. **Navigate to the directory :**

   ```bash
   cd krost-os
   ```

3. **Install dependencies :**

   ```bash
   npm install
   ```

4. **Start the development server :**

   ```bash
   npm run dev
   ```

## 🧭 Usage

1. Open your browser at `http://localhost:3000`.
2. Click or tap the Dock/Launchpad icons to open presentation windows.
3. On mobile/tablet, test touch gestures (_swipe_, _drag & drop_)  for navigation.

## 🗂️ Project Structure

```bash
krost-os/
├─ public/            # Static assets (images, favicon)
├─ src/
│  ├─ components/     # UI: Window, Dock, Launchpad, IconGrid
│  ├─ pages/          # Content: Projects, About, Contact
│  ├─ styles/         # Variables, themes, Tailwind utilities
│  └─ App.jsx         # React entry point + routes
├─ tailwind.config.js # Tailwind CSS configuration
└─ README.md          # Project documentation

```

## 🤝 Contributing

Contributions are welcome! Here's how to get involved :

1. Fork this repository.
2. Create a branch : `git checkout -b feature/ma-fonctionnalité`.
3. Commit your changes : `git commit -m "Ajout de ma fonctionnalité"`.
4. Push to your branch : `git push origin feature/ma-fonctionnalité`.
