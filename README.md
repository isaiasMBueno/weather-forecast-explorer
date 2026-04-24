# Weather Forecast Explorer

A lightweight front-end project that demonstrates how to consume a public weather API and render a **7-day forecast** with a clean, card-based interface.

Although simple by design, this project is a great practical showcase of core web development concepts such as asynchronous requests, XML parsing, DOM manipulation, input normalization, and user-driven data flows.

---

## Project Overview

**Weather Forecast Explorer** allows users to:

1. Type a city name.
2. Fetch matching cities from the CPTEC/INPE service.
3. Select the exact city from a dynamic dropdown.
4. Request and display a 7-day weather forecast.

The interface highlights the current day and presents the remaining days in compact forecast cards with icon-based visual cues.

---

## Key Features

- **City lookup with dynamic options** based on user input.
- **Accent-insensitive search preparation** (diacritic normalization).
- **Duplicate prevention** when adding cities to the selection list.
- **7-day weather forecast rendering** from real API data.
- **Weather-code translation layer** (code → human-readable weather condition).
- **Condition-based icon mapping** (rainy, cloudy, sunny).
- **Instant UI refresh** on each new query.

---

## Concepts Demonstrated

This repository is especially useful as a didactic/demo project because it touches multiple foundational topics:

- **HTML structure and semantic organization** for user input and data display.
- **CSS styling and responsive behavior** for forecast cards.
- **JavaScript + jQuery** for event-triggered interactions.
- **AJAX requests** to external endpoints.
- **XML traversal/parsing** to extract weather values.
- **Dynamic DOM creation** through template strings.
- **Client-side validation and guard clauses** for better UX.

---

## Tech Stack

- **HTML5**
- **CSS3**
- **JavaScript (ES6)**
- **jQuery (AJAX + DOM utilities)**
- **CPTEC/INPE Weather API (XML responses)**

---

## External Data Source

The application consumes data from CPTEC/INPE endpoints:

- City search: `http://servicos.cptec.inpe.br/XML/listaCidades?city=<CITY_NAME>`
- Forecast by city ID: `http://servicos.cptec.inpe.br/XML/cidade/7dias/<CITY_ID>/previsao.xml`

> Note: This is a front-end educational example that depends on internet access and API availability.

---

## How to Run

Because this is a static front-end project, setup is minimal:

1. Clone or download the repository.
2. Ensure internet access.
3. Open `index.html` in your browser.

---

## Educational Value

This project is ideal for:

- Students learning how to integrate APIs into front-end apps.
- Practice with asynchronous data flows and rendering pipelines.
- Demonstrating clean separation between data retrieval, mapping logic, and presentation.

In short: a compact but valuable portfolio piece that demonstrates practical web fundamentals.
