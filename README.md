# Custom Theme Lava 2.0

This document provides a detailed overview of the custom CSS used in the "Lava 2.0" theme. The CSS code included here is designed to enhance the visual appearance and functionality of your website. Feel free to make any adjustments to improve the theme further.

## Table of Contents
- [Social Links Buttons](#social-links-buttons)
- [Album Grid](#album-grid)
- [Project Navigation](#project-navigation)
- [Navigation Arrows](#navigation-arrows)
- [Site Header Button](#site-header-button)
- [Logo Styles](#logo-styles)
- [General Styles](#general-styles)
- [Mobile Adjustments](#mobile-adjustments)
- [Image and Video Styles](#image-and-video-styles)
- [Credits](#credits)

## Social Links Buttons
```css
.site-footer-socials .fo-social-link {
  font-size: 20px; /* Adjust size as needed */
  width: 40px; /* Adjust width as needed */
  height: 40px; /* Adjust height as needed */
  line-height: 40px; /* Vertically center the icon */
}
```

## Album Grid
```css
.album-grid.square .album-item {
  border-radius: 10px; /* Adjust value as needed */
  overflow: hidden; /* Ensures content within the item also has rounded borders */
  background-color: #0a0a0a; /* Default background color */
  transition: background-color 0.3s ease; /* Smooth transition for background color */
}

.album-grid.square .album-image {
  border-radius: 10px; /* Applies rounded borders to images within album items */
}
```

## Project Navigation
```css
.project-nav-link.project-nav-next.square {
  display: none !important; /* Uses !important to ensure the rule is applied */
}

.project-title.title-font.container-sm.text-center + .project-images .project-assets-item {
  margin-bottom: 10px; /* Adjust value as needed */
}

.project-title.title-font.container-sm.text-center + .project-images .project-assets-item-inner {
  margin-bottom: 10px; /* Adjust value as needed */
}
```

## Navigation Arrows
```css
.project-page-prev, .project-page-next {
  position: fixed;
  top: 50vh;
  text-align: center;
  z-index: 2;
  color: inherit;
  width: 5rem;
  font-size: 2.5rem;
  transform: translate(0, -50%);
}

.project-page-prev {
  left: 1rem; /* Adjust position as needed */
}

.project-page-next {
  right: 1rem; /* Adjust position as needed */
}
```

## Site Header Button
```css
.site-header-btn {
  position: absolute;
  top: 1.2857142857rem;
  right: 0.3571428571rem;
  padding: 0.7142857143rem;
  line-height: 0.9285714286rem;
  font-size: 0.0714285714rem;
  cursor: pointer;
  outline: 0;
  display: none;
  background: transparent;
}
```

## Site Header Button
```css
.site-header-btn {
  position: absolute;
  top: 1.2857142857rem;
  right: 0.3571428571rem;
  padding: 0.7142857143rem;
  line-height: 0.9285714286rem;
  font-size: 0.0714285714rem;
  cursor: pointer;
  outline: 0;
  display: none;
  background: transparent;
}
```

## Logo Style
```css
.site-logo img {
  max-width: 100%;
}

img {
  vertical-align: top;
  border-style: none;
}

*, *:before, *:after {
  box-sizing: border-box;
}
```

## General Styles
```css
body {
  font-weight: 300;
  letter-spacing: 0px;
  line-height: 1.75;
  color: var(--body-color);
  background-color: var(--body-bg);
  min-height: 100vh;
  display: flex;
  flex: 1 1 100vw;
  flex-flow: column nowrap;
  max-width: 100%;
  font-family: var(--font-family-primary);
}

.album-grid {
  display: grid;
  grid-template-columns: 1fr;
  grid-column-gap: 1rem; /* Reduces column spacing */
  grid-row-gap: 1rem; /* Reduces row spacing */
}
```

## Mobile Adjustments
```css
@media (max-width: 768px) {
  .site-header-btn {
      display: block; /* Makes the button visible on mobile devices */
      position: relative;
      top: 0;
      right: 0;
      padding: 0.5rem;
      font-size: 1rem;
  }

  .site-header {
      display: flex;
      justify-content: space-between;
      align-items: center;
  }

  .site-logo {
      flex-grow: 1;
  }

  .site-header-btn {
      position: relative;
      top: 0;
      right: 0;
      padding: 0.5rem;
      font-size: 1rem;
  }

  .site-header-btn .line {
      width: 1.6428571429rem;
      height: 0.2142857143rem;
      background: var(--accent-color);
      position: relative;
      transition: opacity .2s linear, transform .2s linear, left .2s linear;
  }

  .site-header-btn .icon-close {
      width: 1.6428571429rem; /* Same width as .line */
      height: 1.6428571429rem; /* Same height as .line */
      background: var(--accent-color);
      position: absolute;
      top: 0;
      right: 0;
      padding: 0.5rem;
      font-size: 1rem;
      cursor: pointer;
      outline: 0;
      display: none;
      background: transparent;
  }

  .menu-open .site-header-btn .icon-close {
      display: block;
  }

  .menu-open .site-header-btn .icon-menu {
      display: none;
  }

  .header-nav-active .site-header-btn {
      position: fixed;
      z-index: 11;
      top: 0;
      right: 0;
      padding: 0.5rem;
      font-size: 1rem;
  }
}
```

## Credits

This custom CSS was created by [Thiago Lage](https://thiagollage.art). Feel free to connect with me on my social media platforms:

- **Twitter:** [@thiagollage](https://twitter.com/thiagollage)
- **Instagram:** [@thiagollage](https://www.instagram.com/thiagollage)
- **Artstation:** [thiagollage](https://www.artstation.com/thiagollage)

This document is open for new adjustments and improvements by other users.