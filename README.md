For More details --> **Property Name - mdn css ** 
---

# 📘 CSS Cheat Sheet – Most Used Properties

| **Category**                | **Property**                  | **Example**                       | **Purpose**                       |
| --------------------------- | ----------------------------- | --------------------------------- | --------------------------------- |
| 🎨 **Text & Fonts**         | `color`                       | `color: red;`                     | Text color                        |
|                             | `font-size`                   | `font-size: 18px;`                | Size of text                      |
|                             | `font-family`                 | `font-family: Arial, sans-serif;` | Font style                        |
|                             | `font-weight`                 | `font-weight: bold;`              | Boldness                          |
|                             | `text-align`                  | `text-align: center;`             | Align text                        |
|                             | `text-decoration`             | `text-decoration: none;`          | Remove underline                  |
|                             | `line-height`                 | `line-height: 1.5;`               | Space between lines               |
| 📦 **Box Model**            | `width / height`              | `width: 200px; height: 100px;`    | Element size                      |
|                             | `margin`                      | `margin: 20px;`                   | Space outside element             |
|                             | `padding`                     | `padding: 10px;`                  | Space inside element              |
|                             | `border`                      | `border: 1px solid black;`        | Border around element             |
|                             | `box-sizing`                  | `box-sizing: border-box;`         | Includes border & padding in size |
| 🎯 **Layout & Positioning** | `display`                     | `display: flex;`                  | Defines layout type               |
|                             | `position`                    | `position: absolute;`             | Position control                  |
|                             | `top / left / right / bottom` | `top: 10px;`                      | Position offsets                  |
|                             | `float`                       | `float: left;`                    | Push elements left/right          |
|                             | `clear`                       | `clear: both;`                    | Stops float overlap               |
|                             | `z-index`                     | `z-index: 10;`                    | Layer order                       |
| 🖼️ **Background**          | `background-color`            | `background-color: lightblue;`    | Background color                  |
|                             | `background-image`            | `background-image: url(bg.jpg);`  | Background image                  |
|                             | `background-size`             | `background-size: cover;`         | Image scaling                     |
|                             | `background-repeat`           | `background-repeat: no-repeat;`   | Prevent repeating                 |
|                             | `background-position`         | `background-position: center;`    | Image position                    |
| 📐 **Flexbox**              | `display`                     | `display: flex;`                  | Enables flexbox                   |
|                             | `flex-direction`              | `flex-direction: column;`         | Row / Column layout               |
|                             | `justify-content`             | `justify-content: space-between;` | Horizontal alignment              |
|                             | `align-items`                 | `align-items: center;`            | Vertical alignment                |
|                             | `flex-wrap`                   | `flex-wrap: wrap;`                | Wraps items                       |
| 🟦 **Grid**                 | `display`                     | `display: grid;`                  | Enables grid                      |
|                             | `grid-template-columns`       | `grid-template-columns: 1fr 1fr;` | Defines columns                   |
|                             | `grid-template-rows`          | `grid-template-rows: auto auto;`  | Defines rows                      |
|                             | `gap`                         | `gap: 10px;`                      | Space between items               |
| ✨ **Effects & Animation**   | `opacity`                     | `opacity: 0.7;`                   | Transparency                      |
|                             | `cursor`                      | `cursor: pointer;`                | Mouse pointer style               |
|                             | `transition`                  | `transition: all 0.3s;`           | Smooth animations                 |
|                             | `transform`                   | `transform: scale(1.2);`          | Rotate/Scale/Move                 |
|                             | `box-shadow`                  | `box-shadow: 0 4px 8px gray;`     | Shadow effect                     |
|                             | `border-radius`               | `border-radius: 10px;`            | Rounded corners                   |
| 📜 **Overflow**             | `overflow`                    | `overflow: hidden;`               | Handle extra content              |

---

⚡ With this cheat sheet, you can **cover 90% of daily CSS work**.

---

# 📏 CSS Measuring Units Cheat Sheet

## 1️⃣ **Absolute Units** (fixed, not relative to anything)

| **Unit** | **Full Form** | **Range (Min → Max)** | **Example**        | **What it does**                                      |
| -------- | ------------- | --------------------- | ------------------ | ----------------------------------------------------- |
| `px`     | Pixels        | `0px → very large`    | `font-size: 16px;` | 1 px = 1 screen pixel (depends on device resolution). |
| `pt`     | Points        | `0pt → very large`    | `font-size: 12pt;` | 1 pt = 1/72 inch (used in print media).               |
| `pc`     | Picas         | `0pc → very large`    | `font-size: 1pc;`  | 1 pc = 12 pt (used in print).                         |
| `in`     | Inches        | `0in → very large`    | `width: 2in;`      | 1 in = 2.54 cm (real-world measurement).              |
| `cm`     | Centimeters   | `0cm → very large`    | `margin: 5cm;`     | Defines size in centimeters.                          |
| `mm`     | Millimeters   | `0mm → very large`    | `margin: 10mm;`    | Defines size in millimeters.                          |

✅ Use case → `px` is the most common for screen design, while `cm`, `mm`, `in`, `pt`, `pc` are mostly for **print**.

---

## 2️⃣ **Relative Units** (size depends on parent or viewport)

| **Unit** | **Full Form**                | **Range (Min → Max)** | **Example**          | **What it does**                                |
| -------- | ---------------------------- | --------------------- | -------------------- | ----------------------------------------------- |
| `%`      | Percentage                   | `0% → 100%+`          | `width: 50%;`        | Size relative to parent container.              |
| `em`     | Relative to parent font-size | `0em → large`         | `font-size: 2em;`    | 1em = current font-size of parent (e.g., 16px). |
| `rem`    | Root em                      | `0rem → large`        | `font-size: 1.5rem;` | 1rem = font-size of root (`html` element).      |
| `ex`     | x-height                     | `0ex → large`         | `font-size: 2ex;`    | Relative to height of lowercase "x".            |
| `ch`     | Character width              | `0ch → large`         | `width: 30ch;`       | Width of the character "0" in current font.     |

✅ Use case → `rem` (for consistent scaling), `%` (for responsive width/height), `em` (for nested scaling).

---

## 3️⃣ **Viewport Units** (responsive to screen size)

| **Unit** | **Full Form**    | **Range (Min → Max)** | **Example**         | **What it does**                      |
| -------- | ---------------- | --------------------- | ------------------- | ------------------------------------- |
| `vw`     | Viewport Width   | `0vw → 100vw`         | `width: 50vw;`      | % of browser width.                   |
| `vh`     | Viewport Height  | `0vh → 100vh`         | `height: 100vh;`    | % of browser height.                  |
| `vmin`   | Viewport Minimum | `0vmin → 100vmin`     | `font-size: 5vmin;` | % of the smaller side (width/height). |
| `vmax`   | Viewport Maximum | `0vmax → 100vmax`     | `font-size: 5vmax;` | % of the larger side (width/height).  |

✅ Use case → Great for **responsive layouts** (fullscreen sections, text that scales with screen).

---

## 4️⃣ **Time Units** (for animations & transitions)

| **Unit** | **Full Form** | **Range (Min → Max)** | **Example**               | **What it does**                  |
| -------- | ------------- | --------------------- | ------------------------- | --------------------------------- |
| `s`      | Seconds       | `0s → unlimited`      | `transition: all 2s;`     | Defines duration in seconds.      |
| `ms`     | Milliseconds  | `0ms → unlimited`     | `animation-delay: 500ms;` | Defines duration in milliseconds. |

✅ Use case → Animations & transitions.

---

## 5️⃣ **Angle Units** (for rotation, gradients, transforms)

| **Unit** | **Full Form** | **Range (Min → Max)** | **Example**                   | **What it does**                         |
| -------- | ------------- | --------------------- | ----------------------------- | ---------------------------------------- |
| `deg`    | Degrees       | `0deg → 360deg`       | `transform: rotate(45deg);`   | Rotation in degrees.                     |
| `grad`   | Gradians      | `0grad → 400grad`     | `transform: rotate(200grad);` | 1 circle = 400 grad.                     |
| `rad`    | Radians       | `0rad → 6.283rad`     | `transform: rotate(3.14rad);` | Rotation in radians (π rad = 180°).      |
| `turn`   | Turns         | `0turn → 1turn`       | `transform: rotate(0.5turn);` | Fraction of full circle (1 turn = 360°). |

✅ Use case → Mostly `deg` for easy understanding.

---

## 6️⃣ **Frequency Units** (rare, used in media)

| **Unit** | **Full Form** | **Range (Min → Max)** | **Example**         | **What it does**             |
| -------- | ------------- | --------------------- | ------------------- | ---------------------------- |
| `Hz`     | Hertz         | `0Hz → unlimited`     | `frequency: 300Hz;` | Number of cycles per second. |
| `kHz`    | Kilohertz     | `0kHz → unlimited`    | `frequency: 1kHz;`  | 1000 Hertz.                  |

✅ Rarely used in CSS except for **speech styles**.

---

## 7️⃣ **Resolution Units** (for media queries & printing)

| **Unit** | **Full Form**       | **Range (Min → Max)** | **Example**                        | **What it does**      |
| -------- | ------------------- | --------------------- | ---------------------------------- | --------------------- |
| `dpi`    | Dots per Inch       | `72dpi → 600dpi+`     | `@media (min-resolution: 300dpi)`  | Print resolution.     |
| `dpcm`   | Dots per Centimeter | `0dpcm → large`       | `@media (min-resolution: 118dpcm)` | Resolution in cm.     |
| `dppx`   | Dots per Pixel      | `1dppx → 3dppx+`      | `@media (min-resolution: 2dppx)`   | Device pixel density. |

✅ Use case → Responsive design for **retina displays** & print.

---

✨ **Summary**

* **Screen design → `px`, `rem`, `%`, `vw/vh`**
* **Responsive design → `rem`, `%`, `vh/vw`, `vmin/vmax`**
* **Animations → `s`, `ms`**
* **Rotation → `deg`**
* **Print → `cm`, `mm`, `pt`, `pc`, `in`**
* **Hi-res displays → `dpi`, `dppx`**

---
