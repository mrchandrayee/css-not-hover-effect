# CSS Not Hover Effect — runnable recreation

[![Live Demo](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-blue?style=for-the-badge&logo=github)](https://mrchandrayee.github.io/css-not-hover-effect/)
[![HTML](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org) [![CSS](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org) [![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](./LICENSE)

This project is recreated from the supplied 72.7-second screen-recording.

## Run
Open `index.html` in a modern browser, or start a local server:

```bash
python3 -m http.server 8000
```

Visit http://localhost:8000.

## Source visible in the video

HTML structure (the recording shows the `1.jpg` through `4.jpg` image names):

```html
<div class="container">
  <div class="card"><img src="1.jpg" alt=""></div>
  <div class="card"><img src="2.jpg" alt=""></div>
  <div class="card"><img src="3.jpg" alt=""></div>
  <div class="card"><img src="4.jpg" alt=""></div>
</div>
```

CSS transcribed from the editor frames:

```css
body {
  background-color: #1e272e;
}
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 50vh;
}
img {
  width: 200px;
  border-radius: 10px;
  -webkit-box-reflect: below 2.5px
    linear-gradient(transparent, transparent, rgba(3, 3, 3, 0.2));
  border: 3px ridge #a5b1c2;
  margin: 5px;
}
.card {
  transition: 0.5s ease;
  cursor: pointer;
}
.container:hover > :not(:hover) {
  opacity: 0.3;
}
.card:hover {
  transform: scale(1.1);
  filter: grayscale(0%);
}
```

The screen recording visibly types these rules. The `body` background is `#1e272e` in the editor, while the tutorial's outer presentation uses a yellow background. This runnable recreation uses the yellow tutorial presentation around a dark gallery panel so the final result matches the video composition. The four thumbnails are crops from the finished gallery shown in the uploaded video; they are not the creator's original full-resolution image files.

## 👨‍💻 Author

**mrchandrayee** · [GitHub](https://github.com/mrchandrayee)

## 📄 License

[MIT License](./LICENSE)
