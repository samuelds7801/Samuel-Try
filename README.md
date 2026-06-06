# My Portfolio Website

## Project Overview

This project is a personal creative portfolio website built with **HTML, CSS, and JavaScript** in one main file: `index.html`.

The website showcases two types of creative work:

- **Design Works**
- **Video Works**

It uses a red-and-black visual style, responsive layout, automatic design/video loading, a homepage slideshow, and a lightbox preview for opening images and videos in a larger view.

---

## Main File

| File | Purpose |
|---|---|
| `index.html` | Main website file. It contains the HTML structure, CSS styling, and JavaScript functionality. |

---

## Main Features

### Home Page

The home page introduces the portfolio with the heading **Creative Work Gallery**. It includes two buttons:

- **View Designs**
- **View Videos**

These buttons switch the visible page without opening a new HTML file.

### Design Gallery

The design page automatically displays images from the `images` folder.

Supported image formats:

```text
jpg, jpeg, png, webp, gif
```

Expected file naming pattern:

```text
images/work1.jpg
images/work2.jpg
images/work3.png
images/work4.jpeg
images/work5.webp
```

### Video Gallery

The video page automatically displays videos from the `videos` folder.

Supported video formats:

```text
mp4, webm, mov, ogg
```

Expected file naming pattern:

```text
videos/video1.mp4
videos/video2.webm
videos/video3.mov
videos/video4.ogg
```

### Lightbox Preview

When a user clicks an image or video card, it opens in a larger preview window called a lightbox.

- Images open as enlarged previews.
- Videos open with controls and autoplay.
- Clicking the close button or the dark background closes the lightbox.

### Slideshow

The homepage preview area automatically shows uploaded design images. The slideshow changes every 3 seconds.

### Responsive Design

The website adjusts depending on screen size:

- Large screens: 4-column gallery
- Medium screens: 3-column or 2-column gallery
- Mobile screens: 1-column gallery

---

## Folder Structure

Use this structure for your project:

```text
portfolio-project/
│
├── index.html
│
├── images/
│   ├── work1.jpg
│   ├── work2.jpg
│   ├── work3.png
│   └── work4.webp
│
└── videos/
    ├── video1.mp4
    ├── video2.webm
    └── video3.mov
```

---

## How to Run the Website

1. Put `index.html` inside your project folder.
2. Create an `images` folder for design works.
3. Create a `videos` folder for video works.
4. Open `index.html` in your browser.

No installation is needed because this is a static website.

---

## How to Add Design Works

1. Open the `images` folder.
2. Add your design image.
3. Rename it using the required format:

```text
work1.jpg
work2.jpg
work3.png
```

Example:

```text
images/work6.jpg
```

The website checks up to 500 possible design files.

---

## How to Add Video Works

1. Open the `videos` folder.
2. Add your video file.
3. Rename it using the required format:

```text
video1.mp4
video2.webm
video3.mov
```

Example:

```text
videos/video5.mp4
```

The website checks up to 500 possible video files.

---

## JavaScript Functions Explained

| Function | Purpose |
|---|---|
| `showPage(pageId)` | Shows the selected page and hides the other pages. |
| `imageExists(path)` | Checks if an image file exists in the `images` folder. |
| `videoExists(path)` | Checks if a video file exists in the `videos` folder. |
| `loadDesigns()` | Searches for design image files and adds them to the design list. |
| `loadVideos()` | Searches for video files and adds them to the video list. |
| `displayDesigns()` | Creates design cards and places them inside the design gallery. |
| `displayVideos()` | Creates video cards and places them inside the video gallery. |
| `startSlideshow()` | Starts the automatic homepage design slideshow. |
| `openImageLightbox(src)` | Opens a clicked design image in the lightbox. |
| `openVideoLightbox(src)` | Opens a clicked video in the lightbox. |
| `closeLightbox()` | Closes the lightbox and stops the video. |

---

## Design and Styling

The website uses a dark creative style with red highlights.

Main colors used:

```text
Black background: #050505
Dark red gradient: #130000
Bright red accent: #ff2525
Button red: #ff2020
White text: #ffffff
Gray paragraph text: #d0d0d0
```

The font stack uses:

```text
Gotham, Montserrat, Arial, sans-serif
```

Montserrat is loaded from Google Fonts as a fallback font.

---

## Customization Guide

### Change the Website Title

Edit this line:

```html
<title>My Portfolio</title>
```

### Change the Logo Text

Edit this line:

```html
<div class="logo">MY<span>PORTFOLIO</span></div>
```

### Change the Main Heading

Edit this line:

```html
<h1>Creative <span>Work Gallery</span></h1>
```

### Change the Intro Text

Edit the paragraph inside the home page hero section:

```html
Welcome to my personal portfolio. This website showcases my designs and video works
in a clean red and black visual style.
```

---

## Important Notes

- Keep the file name as `index.html`.
- Keep design files inside the `images` folder.
- Keep video files inside the `videos` folder.
- Follow the naming pattern: `work1`, `work2`, `video1`, `video2`, and so on.
- If no image or video files are found, the website will show an empty message telling you what files to add.

---

## Built With

- HTML
- CSS
- JavaScript
- Google Fonts

---

## Author

Created as a personal creative portfolio website.
