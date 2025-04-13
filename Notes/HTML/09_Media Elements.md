# HTML Media Elements

HTML allows embedding of multimedia content like **audio**, **video**, and **images**. These media elements help create engaging and interactive web pages.

---

## 1. `<img>` – Images

- Used to embed images into the webpage.
- Requires the `src` (image path) and `alt` (alternative text) attributes.

### Example:

```html
<img src="nature.jpg" alt="A beautiful landscape" width="300" height="200">
```

### Common Attributes:

| Attribute | Description                      |
|-----------|----------------------------------|
| `src`     | Path to the image file           |
| `alt`     | Alternative text for accessibility |
| `width`   | Width of the image               |
| `height`  | Height of the image              |

---

## 2. `<audio>` – Audio Files

- Used to embed sound files like music or narration.
- Requires the `controls` attribute to display play/pause UI.

### Example:

```html
<audio controls>
  <source src="song.mp3" type="audio/mpeg">
  Your browser does not support the audio element.
</audio>
```

### Common Attributes:

| Attribute     | Description                               |
|---------------|-------------------------------------------|
| `controls`    | Adds audio controls (play, pause, etc.)   |
| `autoplay`    | Starts playing automatically              |
| `loop`        | Loops the audio indefinitely              |
| `muted`       | Mutes the audio by default                |

---

## 3. `<video>` – Video Files

- Used to embed videos in the page.
- Requires the `controls` attribute to allow user interaction.

### Example:

```html
<video width="320" height="240" controls>
  <source src="video.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>
```

### Common Attributes:

| Attribute     | Description                               |
|---------------|-------------------------------------------|
| `controls`    | Adds video controls (play, pause, etc.)   |
| `autoplay`    | Plays video automatically                 |
| `loop`        | Repeats the video                         |
| `muted`       | Starts video with no sound                |
| `poster`      | Image displayed before video plays        |

---

## 4. `<iframe>` – Embedding External Media (like YouTube)

- Used to embed another webpage or external media (maps, videos, etc.) in a frame.

### Example:

```html
<iframe width="560" height="315" src="https://www.youtube.com/embed/examplevideo" 
        title="YouTube video" frameborder="0" 
        allowfullscreen>
</iframe>
```

### Common Attributes:

| Attribute     | Description                             |
|---------------|-----------------------------------------|
| `src`         | URL of the page or media to embed       |
| `width`/`height` | Dimensions of the frame              |
| `allowfullscreen` | Allows full-screen display          |

---
