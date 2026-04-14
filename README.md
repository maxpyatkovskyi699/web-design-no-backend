Here is the English version of your README, with the improvements incorporated:

---

# 💅 Chic & Charm — Beauty Salon Information System

A beauty salon website developed as a coursework project for the discipline _"Web Technologies and Web Design"_ (DUITS, 2025).

---

## 📋 Table of Contents

- [About the Project](#about-the-project)
- [Features](#features)
- [Technologies](#technologies)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Pages](#pages)
- [Author](#author)

---

## About the Project

**Chic & Charm** is a responsive beauty salon website that allows clients to explore services, book appointments online, leave reviews, and contact the administration. All functionality is implemented in pure HTML/CSS/JavaScript with no backend — data is stored in the browser's `localStorage`.

Here's the updated **About the Project** section with all 8 features listed:

---

The project includes the following features:

1. **Live clock** — real-time digital clock with auto-update
2. **Login / Logout** — user registration and authentication via modal windows
3. **Masters slider** — cyclic image slider showcasing salon staff
4. **Reviews** — customer review system with star ratings (1–5)
5. **Currency converter** — live UAH exchange rates via PrivatBank API
6. **Task manager** — internal tool for staff to create, track, and filter tasks
7. **Marketplace** — service catalogue with cart, quantity control, and order history
8. **Support** — contact form with JS validation for submitting issues to the administration

---

## You can drop this in to replace the current "About the Project" section in your `README.md`. Want me to also regenerate the full file with this update included?

## Features

### Home Page (`index.html`)

- Digital clock with auto-update (Ukrainian locale)
- Registration and login via modal windows (`localStorage`)
- Masters slider with navigation and cyclic transitions
- Real-time weather widget (OpenWeatherMap API)
- Currency converter (PrivatBank API)
- Review system with star ratings (1–5)

### Shop (`shop.html`)

- Responsive service card grid (1–4 columns depending on screen size)
- Add/remove items from cart without page reload
- Quantity adjustment with automatic total calculation
- Sorting by name and price
- Order confirmation modal window
- Order history (`localStorage`)

### Support (`support.html`)

- Contact form with 5 fields (full name, phone, email, subject, description)
- Step-by-step JS validation with detailed error messages
- Submissions saved to `localStorage` under key `SupportMessages`

### Tasks (`tasks.html`)

- Add new tasks
- Change status: _"in progress"_ → _"done"_ / _"deleted"_
- Permanent deletion via trash icon
- Filter by status
- Display of creation and modification timestamps

---

## Technologies

| Technology         | Purpose                                                   |
| ------------------ | --------------------------------------------------------- |
| HTML5              | Page structure                                            |
| CSS3               | Styling, responsive design (Flexbox, Grid, Media Queries) |
| JavaScript (ES6+)  | Interactivity, DOM manipulation, Fetch API                |
| localStorage       | Client-side data persistence                              |
| OpenWeatherMap API | Real-time weather data                                    |
| PrivatBank API     | Live exchange rates                                       |
| Figma              | Interface prototyping                                     |

---

## Project Structure

```
project/
├── index.html          # Home page
├── shop.html           # Shop / service catalogue
├── support.html        # Contact / feedback form
├── tasks.html          # Task management system
│
├── css/
│   ├── header.css
│   ├── main.css
│   ├── footer.css
│   ├── auth.css
│   ├── flexheader.css
│   ├── masters.css
│   ├── weather.css
│   ├── currency.css
│   ├── reviews.css
│   ├── shop.css
│   ├── cart.css
│   ├── history.css
│   ├── modal.css
│   ├── sort.css
│   ├── support.css
│   └── tasks.css
│
├── js/
│   ├── dateTime.js     # Digital clock
│   ├── auth.js         # Registration / login
│   ├── masters.js      # Masters slider
│   ├── weather.js      # Weather widget
│   ├── currency.js     # Currency converter
│   ├── reviews.js      # Review system
│   ├── shop.js         # Catalogue and cart
│   ├── support.js      # Support form
│   └── tasks.js        # Task manager
│
└── images/
    └── shop/           # Service images
```

---

## Getting Started

The project requires no build step or backend. Simply open `index.html` in your browser.

```bash
# Option 1 — open the file directly
open index.html

# Option 2 — local server via VS Code (Live Server extension)
# or via Python:
python -m http.server 8000
# or
py -m http.server 8000
```

### ⚠️ API Notes

**Currency widget (PrivatBank API):** Requires the CORS proxy to be activated. Visit [cors-anywhere.herokuapp.com/corsdemo](https://cors-anywhere.herokuapp.com/corsdemo) and click _"Request temporary access to the demo server"_ before using the converter.

**Weather widget (OpenWeatherMap API):** Make sure your API key is inserted into `js/weather.js`. Look for the `API_KEY` constant near the top of the file and replace the placeholder with your own key from [openweathermap.org](https://openweathermap.org/api).

---

## Pages

| Page    | File           | Description                                     |
| ------- | -------------- | ----------------------------------------------- |
| Home    | `index.html`   | Salon info, masters, weather, currency, reviews |
| Shop    | `shop.html`    | Service catalogue, cart, orders                 |
| Support | `support.html` | Contact/feedback form                           |
| Tasks   | `tasks.html`   | Task manager for staff                          |

---

## Author

**Piatkovskyi Maksym Oleksandrovych**

2nd-year student, group CS-2.02 (by April-May 2025)
Speciality: _Computer Science_ (F3, 122)  
**SUITT** — STATE UNIVERSITY OF INTELLIGENT TECHNOLOGIES AND TELECOMMUNICATIONS
Supervisor: Senior Lecturer of CS — Severyn M.V.

_Coursework project, 2025_
