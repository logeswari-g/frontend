## CSS Box Model
The CSS Box Model treats every HTML element as a rectangular box with the following components:

1. **Content**: The actual content inside the element (text, image, etc.).
2. **Padding**: Space between the content and the border.
3. **Border**: Edge around the padding and content.
4. **Margin**: Space outside the border (separates elements).

![css_box-model](https://github.com/user-attachments/assets/a6e3b1f3-dfb4-4282-90f6-aa9fc74ca95f)

```
.box {
      width: 200px;
      height: 100px;
      padding: 20px;
      border: 5px;
      /* border: 5px solid #3498db; */
      margin: 20px;
      /* background-color: #ecf0f1; */
      color: #333;
    }
```

## Sample Structure for CSS box Model

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>CSS Box Model Demo</title>
  <style>
    .box {
      width: 200px;
      height: 100px;
      padding: 20px;
      border: 5px;
      /* border: 5px solid #3498db; */
      margin: 20px;
      /* background-color: #ecf0f1; */
      color: #333;
    }
  </style>
</head>
<body>

  <h2>CSS Box Model</h2>
  <br>
  <div>
    Content Box<br>
    Width = 200px<br>
    Padding + Border added outside
  </div>
  <div>
    Content Box<br>
    Width = 200px<br>
    Padding + Border inside width
  </div>
</body>
</html>
```