# New Year Countdown Project

## Overview
This project is a web-based New Year countdown timer that also features a falling snowflake animation. It consists of three main components:

1. **HTML**: Defines the structure and content of the webpage.
2. **CSS**: Provides the visual styling, including animations and responsive design.
3. **JavaScript**: Implements dynamic functionalities like the countdown timer and snowflake animation.

---

## Files and Their Functions

### `index.html`
The HTML file provides the foundational structure of the webpage. Key elements include:

- **Title and Metadata**: Sets the document title and includes links to external resources like the CSS and JavaScript files.
- **Countdown Section**:
  - Displays the days, hours, minutes, and seconds left until the next New Year.
  - Includes a button to preview the "Happy New Year" message or refresh the page.
- **About Section**:
  - Features a title, an image, a description, and a list of skills.

### `style.css`
This file styles the webpage and adds animations. Major features include:

- **Font Styling**: Uses the "Aleo" font for all text.
- **Background**: Implements a radial gradient background with a dark theme.
- **Responsive Design**: Adjusts the layout and font sizes for smaller screens.
- **Key Animations**:
  - `moveBg`: Animates the background of text labels to create a shimmering effect.

### `script.js`
This file manages dynamic behaviors and animations. Major functionalities include:

#### Snowflake Animation
- **`Snowflake` Class**: Represents individual snowflakes.
  - Properties like position (`x`, `y`), velocity (`vx`, `vy`), size (`radius`), and transparency (`alpha`).
  - `reset()`: Reinitializes a snowflake's properties when it moves off the screen.
  - `update()`: Updates the snowflake's position based on its velocity.
- **`Snow` Class**: Manages the canvas and the collection of snowflakes.
  - `onResize()`: Adjusts the canvas size when the window is resized.
  - `createSnowflakes()`: Generates snowflakes based on the screen width.
  - `update()`: Clears the canvas and redraws all snowflakes.

#### Countdown Timer
- **`calculateRemainingTime()`**: Computes the remaining days, hours, minutes, and seconds until January 1 of the next year.
  - Updates the corresponding elements in real-time.
  - Stops when the countdown reaches zero and displays "Happy New Year."
- **`initCountdown()`**: Initializes the countdown and updates it every second.

#### Button Interaction
- **`handleClick()`**: Toggles the button functionality between previewing "Happy New Year" and refreshing the page.

---

## How It Works
1. The webpage initializes with a New Year countdown timer and falling snowflake animation.
2. The JavaScript code dynamically updates the countdown every second.
3. The button allows users to preview the "Happy New Year" message or refresh the page.
4. Snowflakes continuously fall and are regenerated when they exit the viewport.

---

## Features
- Fully responsive design for different screen sizes.
- Smooth animations for snowflakes and shimmering text.
- Real-time countdown to the New Year.

---

## Setup
To run the project:
1. Clone or download the repository.
2. Open `index.html` in any modern browser.

---

## Future Enhancements
- Add customization options for themes or snowflake properties.
- Provide an option to set custom countdown dates.
- Include celebratory animations or sound effects when the countdown ends.

