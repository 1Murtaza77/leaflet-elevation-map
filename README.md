# Leaflet Elevation Map

## 📌 Project Overview
This project provides an interactive map built with **Leaflet** that allows users to click anywhere on the map and retrieve elevation data using the **OpenTopoData API**. The backend runs on **Google Colab** and is exposed publicly using **Cloudflared**.

## ✨ Features
- Interactive map using Leaflet
- Fetch elevation data from OpenTopoData
- Backend hosted on Google Colab
- Public access via Cloudflared tunnel
- Hosted front-end on GitHub Pages

## 🚀 Live Demo
[View the map here](https://YOUR_USERNAME.github.io/leaflet-elevation-map/)  
*(Replace YOUR_USERNAME with your GitHub username)*

## 🛠 Setup Instructions
1. Clone this repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/leaflet-elevation-map.git
   ```
2. Open `index.html` and replace `YOUR_PUBLIC_URL` with the Cloudflared URL from your Colab session (e.g., `https://abc123.trycloudflare.com`).
3. Commit and push changes:
   ```bash
   git add index.html
   git commit -m "Update Cloudflared URL"
   git push origin main
   ```
4. Enable GitHub Pages:
   - Go to **Settings → Pages**
   - Set **Source** to `main` and folder to `/ (root)`
   - Save and wait for the site to build

## 🔄 Updating Cloudflared URL
Every time you restart Colab, the Cloudflared URL changes. Update the `proxyBase` variable in `index.html` and push the changes to GitHub.

## ✅ How It Works
- **Leaflet Front-End**: Displays the map and handles user clicks.
- **Flask API (Colab)**: Proxies requests to OpenTopoData.
- **Cloudflared Tunnel**: Exposes the Flask app publicly.
- **GitHub Pages**: Hosts the static HTML front-end.

## 📄 License
This project is licensed under the MIT License.
