# Technologies Used in "Báo Tường Tết Nguyên Đán" Project

This document outlines the core web technologies utilized in the "Báo Tường Tết Nguyên Đán" project, explaining their role and specific application within the website.

## 1. HTML5

**Role:** HTML5 (HyperText Markup Language 5) is the latest standard for HTML. It provides the fundamental structure and content of all web pages. It defines elements for text, images, multimedia, forms, and semantic sections of a document.

**Usage in Project:**
*   **Document Structure:** All `.html` files in the project (`main.html`, `banh-chung.html`, `gui-loi-chuc.html`, `khong-khi-ngay-xuan.html`, `members.html`) are written using HTML5.
*   **Semantic Elements:** Modern HTML5 semantic tags like `<header>`, `<nav>`, `<main>`, `<section>`, `<footer>`, and `<article>` are used to clearly define the purpose and structure of different parts of the web pages, improving readability for both developers and search engines.
*   **Content Embedding:**
    *   `<img>` tags are used extensively to embed images, both local (from the `pic/` folder) and external (from URLs).
    *   `<video>` tags (`<video class="tet_video" controls>`) are used in `main.html` to embed a video (`video/am_thuc.mp4`).
    *   `<audio>` tags (`<audio controls class="tet_audio">`) are used in `main.html` to embed an audio file (`audio/nhac.m4a`).
*   **Forms:** The `gui-loi-chuc.html` page utilizes HTML5 form elements such as `<form>`, `<label>`, `<input type="text">`, `<input type="email">`, `<textarea>`, and `<button type="submit">` for user input.
*   **Tables:** The `members.html` page uses `<table>`, `<thead>`, `<tbody>`, `<tr>`, `<th>`, and `<td>` elements to display structured team member data.
*   **Metadata:** `<meta charset="UTF-8">` and `<meta name="viewport" ...>` are included for proper character encoding and responsive viewing across devices.

## 2. CSS3

**Role:** CSS3 (Cascading Style Sheets, Level 3) is a stylesheet language used for describing the presentation of a document written in HTML. It controls layout, colors, fonts, and overall visual appearance.

**Usage in Project:**
*   **Styling Strategy:**
    *   `main.html` uses an **external stylesheet** by linking to `style.css` via `<link rel="stylesheet" href="style.css">`. This allows for a single source of truth for its styles.
    *   Other HTML files (`banh-chung.html`, `gui-loi-chuc.html`, `khong-khi-ngay-xuan.html`, `members.html`) embed the CSS rules directly within a `<style>` block in their `<head>` section. This makes each page's styling self-contained.
*   **Selectors:** A combination of element selectors (`body`, `h1`, `p`), class selectors (`.tet_video`, `.section-link-card`, `.button-link`), and ID selectors (`#header`, `#menu`, `#footer`) are used to target specific HTML components.
*   **Layout and Positioning:**
    *   Extensive use of `margin`, `padding`, `display` properties (e.g., `block`, `inline-block`, `flex`, `grid`).
    *   `flexbox` is employed for responsive layouts in areas like `.card-container` and `.section-link-card`.
    *   `grid` is used for `.animal-grid` to create a flexible column layout.
    *   `background-image`, `background-size: cover`, `background-attachment: fixed`, and `background-position: center` are used to create a full-page background effect.
*   **Typography:** `font-family: Arial, sans-serif` is consistently applied across the site.
*   **Visual Effects:** `border`, `border-radius`, `box-shadow`, and `transition` properties are used to enhance the visual appeal of elements and provide subtle interactive feedback (e.g., on hover).
*   **Color Scheme:** Uses a specific palette involving red, yellow, blues, and grays for headers, menus, and text.
*   **Responsiveness:** Media queries (`@media (max-width: 768px)`) are utilized to adjust layout for smaller screens, most notably in the `.members-table` to ensure readability on mobile devices.

## 3. Multimedia Assets

**Role:** Provides rich media content to make the website more dynamic and engaging.

**Usage in Project:**
*   **Images (`.jpg`, `.png`):**
    *   `pic/bangtrung.jpg`: Used as a thumbnail for the "Bánh Chưng" article on `main.html`.
    *   `pic/chotet.jpg`: Used as a thumbnail for the "Không Khí Ngày Xuân" article on `main.html`.
    *   External images: Several external image URLs are directly embedded in `banh-chung.html` and `khong-khi-ngay-xuan.html`.
    *   Background image: A background image (referenced as `Hinh-nen-tet-2025-cho-may-tinh-10` in `style.css`) is used for the `body`.
*   **Audio (`.m4a`):** `audio/nhac.m4a` is integrated into `main.html` to provide an optional audio experience.
*   **Video (`.mp4`):** `video/am_thuc.mp4` is embedded in `main.html` to showcase video content related to Tet.

These technologies collectively form the foundation of the "Báo Tường Tết Nguyên Đán" project, allowing for a structured, visually appealing, and media-rich presentation.
