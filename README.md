# BRACU Routine & CGPA Tools

A web app for BRAC University students to view, manage, and share class routines and calculate CGPA.  
Includes a main routine planner, a CGPA calculator, and a simplified RS routine viewer.

## Features

- **Routine Planner:**

  - Search and select courses/sections.
  - Visual weekly schedule with conflict detection.
  - Copy/share compressed routine IDs.
  - Download routine as an image.
  - Persistent storage via localStorage.
  - PWA support (offline access).

- **CGPA Calculator:**

  - Calculate new CGPA based on current CGPA, credits, and semester grades.
  - Real-time validation and error handling.
  - Responsive and mobile-friendly.

- **RS Routine Viewer:**
  - View routines for RS sections.
  - Download/print friendly.

## Project Structure

```
/
├── index.html              # Main routine planner
├── compressor.js           # Section ID compressor/encoder
├── service-worker.js       # PWA support for main app
├── cg/                     # CGPA calculator app
│   ├── index.html
│   ├── script.js
│   ├── style.css
│   ├── service-worker.js
│   └── ...
├── rs/                     # RS routine viewer
│   ├── index.html
│   ├── activities.json
│   ├── mon-wed.json
│   ├── sun-tues.json
│   └── ...
└── ...
```

## Getting Started

1. **Clone the repository:**

   ```sh
   git clone https://github.com/Sabbirba10/bracutine.git
   cd your-repo
   ```

2. **Install dependencies (if any):**

   - This project is mostly static HTML/JS/CSS.
   - For local development, you can use [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) or any static server.

3. **Run locally:**

   ```sh
   npx serve .
   # or use VSCode Live Server extension
   ```

4. **Deploy:**
   - The project is ready to deploy on Firebase Hosting or any static hosting provider.

## Usage

- Open `index.html` for the main routine planner.
- Open `cg/index.html` for the CGPA calculator.
- Open `rs/index.html` for the RS routine viewer.

## Technologies

- HTML, CSS (Tailwind, custom), JavaScript
- [html2canvas](https://html2canvas.hertzen.com/) for screenshotting
- PWA (Service Worker)
- Firebase Hosting (recommended)

## License

MIT

---

**Contributions welcome!**  
For issues or suggestions, please open an issue or pull request.
