# Project Documentation: Báo Tường Tết Nguyên Đán

This document provides an overview and guide to the "Báo Tường Tết Nguyên Đán" (Tet New Year Wall Newspaper) project. It is designed to help anyone understand its structure, content, and how to interact with it.

## 1. Project Overview

This project is a simple, static website designed as an e-magazine or "wall newspaper" focusing on Vietnamese Lunar New Year (Tết Nguyên Đán) traditions and culture. It serves as an informative and engaging presentation for a school project by "Nhóm 5 STEM 12".

**Key Features:**
*   **Main Page:** An index page with navigation to various articles and multimedia content.
*   **Informative Articles:** Dedicated pages for specific Tet traditions (e.g., Bánh Chưng, Spring Atmosphere).
*   **Interactive Elements:** Embedded video, audio, and a comment/wish submission form.
*   **Team Introduction:** A page listing the project members.
*   **Styling:** Consistent visual design across all pages.

## 2. File Structure

The project is organized into the following directories and files:

```
/home/jmy/someshit/
├── .gitattributes
├── banh-chung.html         // Article: Bánh Chưng (Chung Cake)
├── gui-loi-chuc.html       // Page: Send New Year Wishes/Comments
├── khong-khi-ngay-xuan.html // Article: Spring Atmosphere
├── main.html               // Main entry point/Homepage
├── members.html            // Page: Team Members Introduction
├── README.md               // (This file - if project uses README for general info)
├── style.css               // External stylesheet for main.html
├── audio/
│   └── nhac.m4a            // Tet-themed background music
├── pic/
│   ├── bangtrung.jpg       // Image: Bánh Chưng (used in main.html thumbnail)
│   ├── chotet.jpg          // Image: Spring Market (used in main.html thumbnail)
│   └── nam_and_lion.png    // Image: (Present in folder, but currently unused in HTML)
└── video/
    └── am_thuc.mp4         // Video: Tet Cuisine (embedded in main.html)
```

## 3. Page Breakdown

### `main.html` (Homepage/Index)
*   **Purpose:** The central hub of the project. It introduces the theme of Tet and provides navigation to other detailed content pages.
*   **Content:**
    *   **Header:** Project title and slogan.
    *   **Navigation:** Links to sections within `main.html` (Introduction, Articles, Photos, Music & Video) and to `gui-loi-chuc.html`.
    *   **Introduction (`#gioi-thieu`):** Text about the significance of Tet.
    *   **Music & Video (`#am-nhac`):** Features an embedded video (`video/am_thuc.mp4`) and an audio player (`audio/nhac.m4a`).
    *   **Main Topics (`#bai-viet`):** Links to `banh-chung.html` and `khong-khi-ngay-xuan.html` using visually appealing card layouts.
    *   **New Year Wishes (`#binh-luan`):** A button leading to the `gui-loi-chuc.html` form.
    *   **Footer:** Project credits, contact, and references.
*   **Styling:** Uses the external `style.css` file.

### `banh-chung.html`
*   **Purpose:** Provides detailed information about the "Bánh Chưng - Bánh Giầy" tradition during Tet.
*   **Content:** Text describing the symbolism of Bánh Chưng, accompanied by relevant images. A "Back to main page" button is included.
*   **Styling:** Contains internal CSS, embedding all styles from `style.css` directly within its `<head>` section.

### `gui-loi-chuc.html`
*   **Purpose:** Allows users to submit New Year wishes or comments through a simple form.
*   **Content:** A form with fields for name, email, and a message. Includes a "Back to main page" button.
*   **Styling:** Contains internal CSS, embedding all styles from `style.css` directly within its `<head>` section.

### `khong-khi-ngay-xuan.html`
*   **Purpose:** Describes the festive atmosphere of Tet, with a focus on specific elements like cherry blossoms.
*   **Content:** Text explaining the Tet atmosphere and a section about cherry blossoms with an image. Includes a "Back to main page" button.
*   **Styling:** Contains internal CSS, embedding all styles from `style.css` directly within its `<head>` section.

### `members.html`
*   **Purpose:** Introduces the team members of the project.
*   **Content:** A table listing the names and sequential numbers of the team members. Includes a "Back to homepage" button.
*   **Styling:** Contains internal CSS, embedding all styles from `style.css` directly within its `<head>` section.

## 4. Styling (`style.css`)

The `style.css` file defines the visual presentation of the entire project.
*   **Global Styles:** Sets font family (`Arial, sans-serif`), removes default margins, and applies a fixed, full-cover background image.
*   **Structural Styling:** Styles `header`, `menu`, `content`, `footer`, and general container elements for consistent layout.
*   **Navigation (`#menu`):** Center-aligned list items for navigation links.
*   **Content Cards (`.card-container`, `.section-link-card`):** Uses flexbox for responsive card layouts, with defined widths, padding, borders, shadows, and hover effects.
*   **Forms (`#comment-form`):** Provides basic styling for input fields, text areas, and buttons.
*   **Tables (`.members-table`):** Styles for a clear and readable table, including responsive adjustments for smaller screens (table cells stack vertically).
*   **Multimedia:** Styles for video and audio players, ensuring they are responsive and well-placed.
*   **Color Palette:** Utilizes a scheme with red, yellow, and various shades of blue and grey, contributing to a festive yet clean aesthetic.
*   **Responsiveness:** Includes a media query (`@media (max-width: 768px)`) to optimize the layout for smaller devices, particularly affecting tables.

## 5. Multimedia Assets

The project incorporates various multimedia files to enhance the user experience:
*   **Audio:** `audio/nhac.m4a` (Tet-themed music for background or specific sections).
*   **Video:** `video/am_thuc.mp4` (Video related to Tet cuisine).
*   **Images:**
    *   `pic/bangtrung.jpg`: Thumbnail for Bánh Chưng article.
    *   `pic/chotet.jpg`: Thumbnail for Spring Atmosphere article.
    *   `pic/nam_and_lion.png`: An additional image in the `pic` folder, but not currently used in any of the HTML files.
    *   External images are also used (e.g., in `banh-chung.html`, `khong-khi-ngay-xuan.html`).
    *   The background image `Hinh-nen-tet-2025-cho-may-tinh-10` referenced in `style.css` is assumed to be an external or missing asset.

## 6. How to View the Project

To view this project, simply open the `main.html` file in any web browser.
All other HTML files are linked from `main.html` and can be navigated to by clicking the respective links.

## 7. Potential Enhancements

*   **Semantic HTML:** Further refactor `div` elements into more semantic HTML5 tags where appropriate for better accessibility and structure.
*   **JavaScript Interactivity:** Add JavaScript for features like form validation, dynamic content loading, or interactive galleries.
*   **External Assets:** Ensure all referenced external images are properly sourced or locally stored.
*   **Accessibility:** Improve accessibility features for users with disabilities.
*   **Consistent Styling:** While `main.html` uses external CSS and other pages embed it, a fully external CSS approach for all pages might be cleaner for larger projects.
