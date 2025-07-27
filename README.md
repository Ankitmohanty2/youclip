# 🎬 YouClip: Snip Clips. Make Bangers.

A fun, open-source SaaS tool to snip your favorite moments from YouTube videos! Just paste a URL, set start/end times, and download your custom clip. Perfect for sharing bangers, memes, or highlights. Free for everyone who loves code!

---

## 🚀 Features

- **Frontend:** Next.js + Tailwind CSS (with Shadcn/UI)
- **Backend:** Node.js (Express) with Bun runtime
- **Video Processing:** Uses `yt-dlp` and `ffmpeg` for fast, high-quality clips
- **No cloud storage:** Clips download straight to your device

---

## 🛠️ Prerequisites



Make sure you have these installed:

- [Bun](https://bun.sh/) (`bun` v1.2.7+)
- [Node.js](https://nodejs.org/) (`node` v18+)
- [npm](https://www.npmjs.com/) (v10+)
- [yt-dlp](https://github.com/yt-dlp/yt-dlp)
- [ffmpeg](https://ffmpeg.org/)

**Check versions:**
```sh
bun --version
node --version
npm --version
yt-dlp --version
ffmpeg -version
```
If you're missing any, install them via your package manager (e.g., `brew install bun yt-dlp ffmpeg` on macOS).

---

## 🏁 Getting Started

### 1. Clone the repo
```sh
git clone https://github.com/Ankitmohanty2/youclip.git
cd youclip
```

### 2. Install dependencies
#### Backend
```sh
cd backend
bun install
```
#### Frontend
```sh
cd ../frontend
bun install
```

### 3. Run the app
#### Start backend
```sh
cd backend
bun run src/index.ts
```
- Backend runs at [http://localhost:3001](http://localhost:3001)

#### Start frontend
```sh
cd ../frontend
bun run dev
```
- Frontend runs at [http://localhost:3000](http://localhost:3000)

---

## ✂️ Usage
1. Open [http://localhost:3000](http://localhost:3000)
2. Paste a YouTube URL and set start/end times (`HH:MM:SS`)
3. Click **Clip Video**
4. Download your custom `clip.mp4`!

---

## 📁 Project Structure
```
youclip/
  backend/
    src/
    uploads/
    package.json
    tsconfig.json
  frontend/
    app/
    public/
    components/
    package.json
    tsconfig.json
    next.config.ts
```

---

## 🧰 Troubleshooting
- **yt-dlp or ffmpeg not found:** Make sure both are installed and in your PATH.
- **Video upload issues:** Update ffmpeg if you have trouble with Twitter compatibility.
- **Port conflicts:** Change the port in backend/frontend configs if needed.

---

## 👩‍💻 Development Notes
- TypeScript is used throughout.
- Hot reload is NOT enabled.
- Linting: `bun run lint` in frontend.

---

**Enjoy snipping!**

If you have questions or ideas, open an issue or PR. Star the repo if you like it! ⭐
