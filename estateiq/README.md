# EstateIQ — AI-Informed Real Estate Discovery

> **Live demo:** https://kushagra69yr.github.io/estateiq/  
> **Source:** https://github.com/kushagra69yr/kushagra69yr.github.io/tree/main/estateiq

EstateIQ is a responsive real-estate discovery demo that lets users browse sample listings, filter homes, save favorites during the current session, compare up to three properties, and explore an illustrative price estimate.

## Demo disclaimer

The listings and prices are illustrative demo data, not verified active properties or real market data. The current hosted Price Lab uses a transparent rule-based calculation in the browser; it is **not connected to a trained machine-learning model, backend API, or database**. Do not use its output for a real purchase, loan, or investment decision.

## Features in the current demo

- Responsive premium green-and-cream UI.
- Search listings by city/neighborhood or property name.
- Filter by property type, budget, and minimum bedrooms.
- Listing cards with property facts and illustrative asking prices.
- Save/remove favorites during the current browser session.
- Select and compare up to three homes in a comparison view.
- Price Lab form with input validation and an explicitly labelled illustrative estimate.
- Mobile-friendly layouts and empty states.

## Technology used in the current demo

- HTML5
- CSS3 (responsive layout and design system)
- Vanilla JavaScript (filtering, favorites, comparison, and demo estimate)
- Unsplash-hosted property photography

## Run locally

This current frontend is a static page and does not need Python or Node:

1. Clone or download this repository.
2. Open `estateiq/index.html` in a browser, or run a static server from the repository root:

   ```bash
   python -m http.server 5500
   ```

3. Open `http://127.0.0.1:5500/estateiq/`.

## How the planned full-stack version can work

The next iteration can add a real backend and model:

1. **Frontend:** React + TypeScript + Tailwind CSS.
2. **API:** Python FastAPI endpoints for property listings and price prediction.
3. **Database:** PostgreSQL tables for users, properties, favorites, and inquiries.
4. **ML pipeline:** Scikit-learn regression model trained on a documented, relevant property dataset.
5. **Evaluation:** Report measured MAE and R² on a held-out test set; never invent metrics.
6. **Deployment:** Static frontend hosting plus separately deployed API and managed PostgreSQL.

These are proposed next steps, not capabilities of the currently hosted demo. A meaningful price prediction feature requires suitable real-world training data and honest evaluation.

## Core subjects demonstrated

- **Web development:** HTML, CSS, JavaScript, responsive design.
- **Data structures and algorithms:** array filtering, sorting/selection logic, sets for saved and selected listing IDs.
- **Software engineering:** UI state handling, input validation, separation of concerns within the demo.
- **Machine Learning (planned extension):** supervised regression, feature engineering, train/test split, evaluation metrics.
- **DBMS (planned extension):** relational schema, SQL, CRUD, constraints, and persistence.
- **Computer Networks (planned extension):** HTTP and REST APIs between frontend and backend.

## Suggested future improvements

- Move the page into reusable React components.
- Build FastAPI listing and prediction endpoints.
- Add PostgreSQL persistence and secure authentication.
- Train and evaluate a model on a documented dataset.
- Add tests, CI, API documentation, and deployment health checks.
- Replace illustrative listings with licensed, verified data.

## Author

Kushagra Burman — B.E. Artificial Intelligence and Machine Learning student.

This project is a portfolio demonstration and should be described according to what is implemented and tested.