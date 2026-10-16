# Clearinfra Official Website (`clearinfra.in`)

High-performance marketing and product intelligence website for **Clearinfra** — the CI-driven operating system for sustainable building design, EnergyPlus parity simulation, and NBC/ECBC automated compliance.

Built with **Astro**, **Tailwind CSS v4**, and optimized for zero-latency deployment on **Cloudflare Pages**.

---

## ⚡ Quick Start

### 1. Development Server
```bash
npm run dev
# Starts local development server at http://localhost:4321
```

### 2. Production Build
```bash
npm run build
# Compiles static HTML/CSS/JS into ./dist in < 500ms
```

### 3. Local Preview
```bash
npm run preview
# Serves the compiled production build locally
```

---

## ☁️ Deploying to Cloudflare Pages

1. **Push this repository to GitHub/GitLab:**
   ```bash
   git add .
   git commit -m "feat: initial clearinfra.in website"
   git remote add origin <your-github-repo-url>
   git push -u origin main
   ```

2. **In the Cloudflare Dashboard:**
   - Navigate to **Workers & Pages** → **Create Application** → **Pages** → **Connect to Git**.
   - Select your `Clearinfra-website` repository.
   - Use the following build configuration:
     - **Framework preset:** `Astro`
     - **Build command:** `npm run build`
     - **Build output directory:** `dist`
     - **Environment variables:** (none required for static mode)

3. **Custom Domain:**
   - Go to your Pages project → **Custom Domains** → **Set up a custom domain**.
   - Enter `clearinfra.in` and `www.clearinfra.in`.
   - Cloudflare will automatically provision SSL certificates and configure DNS records.

---

## 🏛️ Architecture & Routing

| Domain | Role | Repository |
| :--- | :--- | :--- |
| **`clearinfra.in`** | Marketing, product capabilities, research, contact | This repository (`Clearinfra-website`) |
| **`app.clearinfra.in`** | Interactive 3D editor, digital twin & simulation platform | Core app repository (`Clearinfra-Editor`) |
