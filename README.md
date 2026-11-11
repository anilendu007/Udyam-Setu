# Udyam Setu — Demo Prototype

A responsive, front-end-only demo for a platform that helps India's informal workers manage independent businesses, collaborate on larger orders, coordinate group procurement, and maintain portable professional records.

## Demo features

- Overview dashboard with business activity
- My Business: sample customer orders and searchable records
- Collective Orders: illustrative 590-school-uniform group project
- Group Procurement: sample supplier quote comparison
- Professional Identity Passport: sample worker profile and downloadable text report
- Interactive demo actions and modal forms

## Run locally

No build step or package installation is required.

1. Download and extract this repository.
2. Open `index.html` in a browser.

For local hosting, run:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`.

## Deploy on Render

1. Push this folder to a GitHub repository.
2. In Render, choose **New → Static Site**.
3. Connect the repository.
4. Set **Build Command** to blank.
5. Set **Publish Directory** to `.`.
6. Deploy.

A `render.yaml` is included for Blueprint-based deployment.

## Important prototype limitations

This is a UI demonstration using fictional sample data. It has no backend, authentication, database, real supplier connections, real orders, payment processing, or actual verification. The 590-uniform order and all business figures are illustrative. Do not present the demo records as real users, customers, partnerships, or completed transactions.

## Suggested next development steps

- Add authentication and role-based access.
- Add a database for worker profiles, orders, allocations and procurement requests.
- Implement consent-based evidence and customer confirmation for work-history records.
- Add transparent allocation rules and dispute workflows.
- Add multilingual support and low-bandwidth/mobile-first refinements.
