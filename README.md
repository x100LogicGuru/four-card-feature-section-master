---
# Four Card Feature Section – Documentation

## Overview

This project is a responsive web component that displays a four-card feature section, inspired by a popular frontend challenge. It uses semantic HTML and modern CSS Grid for layout, with a focus on clean, scalable, and mobile-friendly design.
---

## Project Structure

```
<code_block_to_apply_changes_from>
```

---

## HTML Structure (`index.html`)

- **Header Section**: Contains the main heading and a short descriptive paragraph.
- **Card Container**: Uses a grid layout to display four feature cards.
  - Each card includes:
    - An icon (SVG)
    - A heading
    - A short description

---

## CSS Structure (`style.css`)

### 1. CSS Variables

Defined in the `:root` for easy theming:

- **Primary Colors**: `--red`, `--cyan`, `--orange`, `--blue`
- **Neutral Colors**: `--very-dark-blue`, `--grayish-blue`
- **Typography**: Font family, size, and weights

### 2. Base Styles

- **Box Sizing**: `border-box` for all elements
- **Body**: Sets font, background color, and base font size

### 3. Header

- **.header**: Centered, with responsive width
- **.header-one** and **.header-two**: Different font weights for visual hierarchy
- **.short-paragraph**: Responsive width and larger font for readability

### 4. Card Layout

- **.card-container**: Uses CSS Grid for layout
  - **Desktop**: 3 columns, fixed width (400px each), centered
  - **Tablet**: Columns become responsive using `minmax(250px, 1fr)`
  - **Mobile**: Single column, cards stack vertically
- **.card**: Styled with border-radius, box-shadow, and padding
- **Card Variants**: Each card has a unique top border color and grid position for visual distinction

### 5. Responsive Design

- **@media (max-width: 1500px)**: Header width increases for smaller screens
- **@media (max-width: 1350px)**: Adjusts card alignment and grid spans
- **@media (max-width: 1300px)**: Grid columns become responsive
- **@media (max-width: 1035px)**: Grid switches to a single column, cards stack vertically, and custom grid positions are reset
- **@media (max-width: 900px)**: Header width set to 90% for small screens

### 6. Accessibility & UX

- **Text Contrast**: Uses strong color contrast for readability
- **Responsive Images**: Icons scale with card size
- **Centered Content**: Ensures content is always visually centered and accessible

---

## Key Design Decisions

- **CSS Grid**: Chosen for its flexibility in creating both multi-column and single-column layouts with minimal code.
- **CSS Variables**: Make it easy to update colors and fonts across the project.
- **Mobile-First Enhancements**: Media queries ensure the layout adapts smoothly to all screen sizes.
- **Separation of Concerns**: All styles are in `style.css`, keeping HTML clean and semantic.

---

## Customization

- **Colors and Fonts**: Easily changeable via CSS variables in `:root`.
- **Card Content**: Add or remove cards by editing the HTML and updating grid settings if needed.
- **Breakpoints**: Adjust media query values in `style.css` to fit your specific needs.

---

## Assets

- **Design Images**: For reference only, not used in the live site.
- **SVG Icons**: Used in each card for visual appeal.

---

## How to Use

1. Open `index.html` in your browser to view the component.
2. Edit `style.css` to customize the look and feel.
3. Use the design images in `/design` as a reference for pixel-perfect implementation.

---

## Credits

- Challenge and design inspiration from [Frontend Mentor](https://www.frontendmentor.io/).
- Icons from the provided assets.

