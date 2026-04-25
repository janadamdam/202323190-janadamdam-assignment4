# Technical Documentation

## Overview

This project is a complete personal portfolio web application built using HTML, CSS, and JavaScript.

The goal is to present personal information and projects while providing an interactive and user-friendly experience. The application combines multiple features such as filtering, API integration, animations, and persistent data storage.

---

## Technologies Used

* HTML for structure
* CSS for styling and responsive layout
* JavaScript for interactivity and logic
* localStorage for saving user preferences
* Pexels API for dynamic image content

---

## Project Structure

assignment4/
├── index.html
├── css/
│   └── styles.css
├── js/
│   └── script.js
├── assets/
│   └── images/
├── docs/
│   ├── ai-usage-report.md
│   └── technical-documentation.md

---

## Core Features Implementation

### 1. Welcome Overlay & Personalization

* A welcome popup asks for the user’s name
* The name is saved using localStorage
* On reload, the overlay is skipped if a name exists
* The greeting updates dynamically based on time of day

This improves user experience by personalizing the interface.

---

### 2. Mode Switching System

* Users can switch between:

  * All
  * Professional
  * Creative

* Each project is tagged with a class

* JavaScript filters projects based on selected mode

* The page theme updates using body classes

This feature demonstrates conditional rendering and dynamic UI updates.

---

### 3. Favorites System

* Users can mark projects as favorites
* Favorite state is stored in localStorage
* Favorites persist after page reload
* Users can filter to show only favorite projects

This feature combines:

* state management
* filtering logic
* user interaction

---

### 4. Scroll Animations

* Sections and elements appear when scrolling
* Implemented using JavaScript and CSS transitions

This improves visual engagement and user experience.

---

### 5. Contact Form Validation

* Validates:

  * name
  * email format
  * message length

* Displays error messages for invalid input

* Displays success message when valid

This ensures proper user input handling.

---

### 6. API Integration (Pexels)

* Users enter a keyword
* A fetch request is sent to the Pexels API
* Images are dynamically displayed on the page

Example:

```javascript
fetch(`https://api.pexels.com/v1/search?query=${query}`)
```

* Handles:

  * empty input
  * failed requests
  * no results found

This feature demonstrates working with external APIs and asynchronous JavaScript.

---

### 7. Tooltip User Guidance

* A tooltip appears when hovering over the mode button
* It explains how to switch between views
* Improves usability and user understanding

---

## Error Handling

* Empty input fields show clear messages
* Invalid email format is detected
* No matching projects shows a message
* API errors display user-friendly feedback

---

## Performance Considerations

* Efficient DOM updates (only necessary elements updated)
* LocalStorage used instead of repeated input
* Images optimized and loaded dynamically
* Minimal unnecessary re-renders

---

## Conclusion

This project demonstrates how multiple web development concepts can be combined into a complete application. It integrates user interaction, conditional logic, external APIs, and persistent data storage to create a functional and polished portfolio website.
