 <div align="center">

<img src="https://upload.wikimedia.org/wikipedia/commons/e/ef/Youtube_logo.png" alt="YouTube Logo" width="55" align="center" />

# YouTube Thumbnail Downloader

A lightweight, browser-based application for extracting, previewing, and downloading YouTube video thumbnails in multiple resolutions.

</div>

---

## Preview

<div align="center">
  <img
    src="https://i.postimg.cc/QdCvtk0G/Screenshot-2026-11-12-012643.png"
    alt="YouTube Thumbnail Downloader Preview"
    width="100%"
  />
</div>

## Overview

YouTube Thumbnail Downloader allows users to retrieve thumbnails from YouTube videos by simply entering a video URL. It automatically extracts the video ID and displays available thumbnail resolutions, making it easy to preview and download images directly from the browser.

The application is built using HTML, Tailwind CSS, and Vanilla JavaScript, with no backend infrastructure or API keys required.

## Features

- **Multiple URL Formats:** Supports YouTube watch URLs, shortened links, embedded player URLs, mobile links, and Shorts URLs.
- **Multiple Resolutions:** Retrieves thumbnails in maximum, standard, high, and medium quality where available.
- **Instant Preview:** Displays available thumbnail images before downloading.
- **Resolution Detection:** Handles unavailable thumbnail resolutions and provides alternative options.
- **Direct Downloads:** Allows users to download thumbnails directly to their devices.
- **Client-Side Processing:** All URL parsing and application logic run directly in the browser.
- **No API Keys Required:** Uses publicly accessible YouTube thumbnail image endpoints.
- **Lightweight Architecture:** No backend, database, or build process required.

## Supported Resolutions

| Quality | Thumbnail Identifier | Dimensions |
|---|---|---|
| Maximum Resolution | `maxresdefault` | 1280 × 720 |
| Standard Definition | `sddefault` | 640 × 480 |
| High Quality | `hqdefault` | 480 × 360 |
| Medium Quality | `mqdefault` | 320 × 180 |

Actual availability and dimensions may vary depending on the video.

## Technology Stack

- HTML5
- Tailwind CSS
- Vanilla JavaScript
- YouTube Public Thumbnail Image Endpoints

## Repository Structure

```text
youtube-thumbnail-downloader/
├── index.html
└── README.md
```

## Getting Started

### Prerequisites

A modern web browser such as Google Chrome, Mozilla Firefox, Microsoft Edge, or Safari.

No additional runtime or development dependencies are required.

### Installation

Clone the repository:

```bash
git clone https://github.com/Akshay-gurav-31/youtube-thumbnail-downloader.git
```

Navigate to the project directory:

```bash
cd youtube-thumbnail-downloader
```

### Running the Application

Open `index.html` directly in your preferred browser.

Alternatively, start a local development server:

```bash
python3 -m http.server 8000
```

Navigate to:

```text
http://localhost:8000
```

## How It Works

### 1. URL Parsing

The application identifies and extracts the unique 11-character video ID from supported YouTube URL formats.

### 2. Thumbnail Retrieval

Once the video ID is extracted, the application constructs thumbnail image URLs using YouTube's public image endpoint.

```text
https://img.youtube.com/vi/VIDEO_ID/RESOLUTION.jpg
```

Replace `VIDEO_ID` with the extracted video ID and `RESOLUTION` with the required thumbnail identifier.

### 3. Preview and Download

The application loads the available thumbnail images, displays their previews, and provides download options for supported resolutions.

Unavailable resolutions are handled through image-loading fallback logic.

## Privacy

The application processes video URLs directly in the browser.

- No user accounts or registration required.
- No application backend required.
- No API keys required.
- No video URL submission to a custom backend.

Thumbnail requests are made directly to YouTube's image servers.

## Contributing

Contributions, bug reports, and feature suggestions are welcome.

To contribute:

1. Fork the repository.
2. Create a feature branch:

   ```bash
   git checkout -b feature/your-feature-name
   ```

3. Commit your changes:

   ```bash
   git commit -m "Add your feature"
   ```

4. Push your branch:

   ```bash
   git push origin feature/your-feature-name
   ```

5. Open a Pull Request.

## License

This project is distributed under the MIT License. See the `LICENSE` file for details.

---

<div align="center">

Developed by [Akshay Gurav](https://github.com/Akshay-gurav-31)

</div>
