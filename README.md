# Udyam Setu
### Empowering India's informal workforce to manage independently, collaborate collectively, and grow sustainably.

<p align="center">
  <strong>Own Your Work. Grow Together.</strong>
</p>

<p align="center">
  <em>A worker-first business and collaboration platform for India's informal workforce.</em>
</p>

---

> **At a glance:** Udyam Setu is a prototype of a digital business operating system for independent workers and micro-entrepreneurs. It brings together day-to-day business management, collective fulfilment of larger orders, group procurement, and a portable professional activity record—so small businesses can access larger opportunities without giving up their independence.

**Project status:** Hackathon demo / frontend prototype  
**Current implementation:** Responsive browser-based application using HTML, CSS and vanilla JavaScript  
**Data in this demo:** Fictional sample data only  
**Backend:** Not implemented in this prototype

---

## Table of contents

- [1. The problem](#1-the-problem)
- [2. The idea behind Udyam Setu](#2-the-idea-behind-udyam-setu)
- [3. Who it is for](#3-who-it-is-for)
- [4. How the platform works](#4-how-the-platform-works)
- [5. Product modules](#5-product-modules)
- [6. The 590-school-uniform use case](#6-the-590-school-uniform-use-case)
- [7. Key user journeys](#7-key-user-journeys)
- [8. What makes the approach different](#8-what-makes-the-approach-different)
- [9. Prototype features and interactions](#9-prototype-features-and-interactions)
- [10. Technology used](#10-technology-used)
- [11. Architecture of the current prototype](#11-architecture-of-the-current-prototype)
- [12. Repository structure](#12-repository-structure)
- [13. Run locally](#13-run-locally)
- [14. Deploy on Render](#14-deploy-on-render)
- [15. Proposed production architecture](#15-proposed-production-architecture)
- [16. Proposed data model](#16-proposed-data-model)
- [17. Trust, fairness, privacy and security](#17-trust-fairness-privacy-and-security)
- [18. Accessibility and inclusion principles](#18-accessibility-and-inclusion-principles)
- [19. Business model hypotheses](#19-business-model-hypotheses)
- [20. Validation plan](#20-validation-plan)
- [21. Roadmap](#21-roadmap)
- [22. Demo walkthrough for evaluators](#22-demo-walkthrough-for-evaluators)
- [23. Current limitations](#23-current-limitations)
- [24. Contributing](#24-contributing)
- [25. License](#25-license)
- [26. Team and acknowledgements](#26-team-and-acknowledgements)

---

## 1. The problem

India's informal workforce includes tailors, artisans, street vendors, home-food entrepreneurs, electricians, plumbers, repair professionals, domestic workers, and many other skilled people who provide essential goods and services.

Many of these workers are capable of running independent businesses. However, the systems available to support them are often fragmented.

### The challenges

**1. Business administration is scattered**

Customer details, orders, quotations, payments, expenses and repeat-customer information may be spread across notebooks, messaging applications, calls and memory. This makes it harder to maintain a consistent view of a business.

**2. Large opportunities can exceed individual capacity**

A school, housing society, retailer or institution may need a large quantity of products or a coordinated service. A single small business may not have enough people, equipment, working capital or production capacity to accept the entire requirement.

**3. Collaboration is difficult to organise**

Even when several capable workers could fulfil an order together, they need a practical way to agree on responsibilities, quantities, quality expectations, deadlines, procurement, progress and payment terms.

**4. Purchasing power is fragmented**

Independent businesses often buy materials separately. Coordinating demand may help them compare supplier quotations and explore bulk purchasing opportunities, but doing so requires transparent requirements and reliable coordination.

**5. Professional history is not always portable**

A worker's skills, completed projects, references and business activity may be recorded in different places—or not recorded at all. When approaching a new customer, institution or partner, it can be difficult to present a clear professional history.

### The core insight

The challenge is not simply that workers need another place to find jobs. They also need practical infrastructure to manage their businesses, collaborate with one another, and carry evidence of their professional activity across opportunities.

---

## 2. The idea behind Udyam Setu

**Udyam Setu is designed as a worker-first business and collaboration platform.**

It connects three capabilities:

1. **Run an independent business:** manage customers, orders, quotations, invoices and business records.
2. **Grow through collective work:** combine capacity with other independent businesses to fulfil larger orders.
3. **Build a portable professional identity:** maintain a worker-controlled record of skills, experience, references and professional activity.

The platform is intended to support independent businesses—not turn workers into employees of the platform.

### Our vision

> Small businesses should not have to become large companies individually to access larger opportunities collectively.

### Our mission

Give informal workers accessible digital tools to manage their work, collaborate transparently and build a stronger professional track record.

---

## 3. Who it is for

Udyam Setu is designed for independent workers and small businesses whose work can be managed through customer records, orders, capacity, milestones or repeatable service activities.

| Worker segment | Example use on Udyam Setu |
|---|---|
| Tailors and garment makers | Combine production capacity for uniform or garment orders |
| Artisans and craft producers | Coordinate a larger craft order across independent makers |
| Home-food entrepreneurs | Coordinate bulk food orders, subject to food-safety and delivery requirements |
| Electricians | Coordinate teams for larger maintenance projects |
| Plumbers | Organise work allocation for building or housing-society maintenance |
| Repair professionals | Maintain customer and service histories |
| Small vendors and producers | Manage customers, inventory and bulk orders |

### Initial demonstration segment

The current demo uses **tailors and garment makers** as its primary example.

This is a useful first workflow because it makes production capacity, quantities, materials, allocation and deadlines easy to understand. The underlying product model can later be adapted to other compatible worker groups.

---

## 4. How the platform works

The intended product journey is:

1. A worker creates a profile and records their profession, skills, experience and available capacity.
2. The worker manages customers and individual orders in their business workspace.
3. A suitable large order is posted by an institution or buyer.
4. Interested workers review the requirement and decide whether to participate.
5. The group agrees on capacity, responsibilities, deadlines, quality requirements and payment terms.
6. Participants coordinate materials and compare supplier quotations where useful.
7. Progress and individual contributions are recorded.
8. Completed work can become part of each worker's professional activity record, with the appropriate confirmation and evidence status.

The worker remains an independent business owner and chooses which opportunities to accept and which information to share.

---

## 5. Product modules

### 5.1 My Business — independent business management

A simple workspace for the day-to-day operations of a microbusiness.

**Planned capabilities**
- Maintain a customer list.
- Record customer orders and order details.
- Prepare quotations.
- Record invoices and payment status.
- Track business income and expenses.
- Maintain product or material information where relevant.
- Identify repeat customers.
- Review business activity over time.
- Export business records.

**Why it matters**

Workers should be able to use digital tools to manage their own customers and records. Their relationship with a customer should not exist only inside a third-party marketplace.

**In the current demo**
- A business overview with sample statistics.
- A recent-orders table.
- Search/filter interaction for sample orders.
- A modal form that demonstrates adding an order.

These interactions are illustrative. They do not yet persist to a database.

### 5.2 Collective Orders — collective fulfilment

This is the central collaboration concept.

Collective Orders is designed to help independent workers participate in a larger project when the work can be divided into manageable contributions.

**Planned capabilities**
- View or post a larger order.
- Review the required skills, quantity, location and deadline.
- Express interest in participating.
- Declare available capacity.
- Form a compatible group.
- Agree on each participant's work allocation.
- Track milestones and progress.
- Record individual contributions.
- Maintain a project-level completion record.
- Record agreed payment terms and payment status.

**Fairness principles**

Work allocation should be visible and agreed upon by participants. Workers should be able to understand:
- What quantity or task has been assigned to them.
- Why the proposed allocation is suitable.
- What deadline they are accepting.
- What payment terms have been agreed.
- How their progress and contribution are recorded.

The platform should not silently assign work or hide important terms from participants.

### 5.3 Group Procurement — coordinated purchasing

Independent businesses may need similar raw materials, tools or packaging. Group Procurement is designed to help them combine requirements and compare supplier quotations.

**Planned capabilities**
- Record each participant's material requirement.
- Calculate the group's combined estimated requirement.
- Request quotations from suppliers.
- Compare price, quality, minimum quantity, delivery time and other terms.
- Let participants review the options.
- Record each participant's final commitment.
- Track procurement and delivery status.

**Important principle**

Combining demand does not automatically guarantee a discount. The product should display actual quotations and terms, and workers should make informed choices. Any savings claim must be based on a real comparison with a valid reference price.

### 5.4 Professional Identity Passport — portable work history

A worker-controlled professional record that can help them present their experience to potential customers, institutions and participating platforms.

**Planned record categories**
- Skills and experience.
- Completed work history.
- Customer references.
- Business transaction summaries.
- Participation in collective projects.
- Individual contribution records.
- Downloadable business performance reports.

**Record status must be clear**

A live implementation should distinguish between:
- **Self-reported:** entered by the worker.
- **Customer-confirmed:** confirmed by the relevant customer.
- **Evidence-supported:** supported by a defined document or record.
- **Platform-recorded:** generated from activity within Udyam Setu.

A record should never be described as verified merely because it was entered into a profile.

**Worker control**

Workers should be able to choose what information to share, with whom and for what purpose. The product should support export and sharing without claiming that every external platform already accepts the record.

---

## 6. The 590-school-uniform use case

This is the main illustrative scenario used in the demo.

### The situation

A school needs **590 uniforms**.

Five independent tailoring businesses are interested in the opportunity. Each has skills and some available production capacity, but accepting and managing the complete order individually may be difficult.

The group explores a collective approach.

### Illustrative allocation

| Participant | Illustrative allocation |
|---|---:|
| Tailor 1 | 118 uniforms |
| Tailor 2 | 118 uniforms |
| Tailor 3 | 118 uniforms |
| Tailor 4 | 118 uniforms |
| Tailor 5 | 118 uniforms |
| **Total** | **590 uniforms** |

This equal allocation is used only to make the demonstration easy to follow. In a real project, allocation should depend on each worker's declared capacity, skill, availability, quality requirements and mutually agreed terms—not automatically divide every order equally.

### How Udyam Setu supports the workflow

1. **Opportunity:** the buyer's requirement is represented as one collective order.
2. **Participation:** suitable independent businesses express interest.
3. **Capacity:** each worker declares how much work they can undertake.
4. **Agreement:** participants review and accept their individual allocation.
5. **Procurement:** the group can combine material requirements and compare supplier quotations.
6. **Coordination:** deadlines and milestones are visible.
7. **Contribution:** each worker's completed quantity is recorded separately.
8. **Completion:** the buyer reviews the delivered order and confirms the relevant work.
9. **Professional history:** eligible records can be added to each worker's passport with a clear confirmation status.

### Why this scenario matters

It demonstrates the central idea of Udyam Setu: **independent businesses can coordinate their capabilities to pursue opportunities that may be difficult to fulfil alone.**

> **Demo disclaimer:** The 590-uniform scenario, participants, order value, supplier details, dates, ratings and progress shown in this repository are fictional sample data. They do not represent a real buyer, confirmed order, actual workers, supplier quotation, completed project or measured impact.

---

## 7. Key user journeys

### Journey A — an independent tailor

1. Ravi creates a worker profile.
2. He records tailoring skills and experience.
3. He adds customers and records orders.
4. He prepares a quotation for a customer.
5. He reviews business activity and exports a sample report.

**Expected value:** more organised business records and easier customer follow-up.

### Journey B — a group of tailors

1. A buyer posts a large uniform requirement.
2. Tailors review the quantity, location, deadline and requirements.
3. Interested workers declare capacity.
4. The group agrees on work allocation and terms.
5. The group coordinates fabric procurement.
6. Each participant updates progress.
7. Contributions are recorded separately.
8. The buyer confirms the completed work.

**Expected value:** a practical coordination layer for collective fulfilment.

### Journey C — a worker sharing professional history

1. A worker reviews their skills and work records.
2. They select which records they want to share.
3. They generate a shareable or downloadable report.
4. A prospective customer or institution reviews the information.
5. The worker can continue maintaining their own record.

**Expected value:** a more portable way to present professional activity.

---

## 8. What makes the approach different

Udyam Setu is not positioned only as a worker directory or job-listing platform.

Its core proposition is the combination of:

| Capability | Purpose |
|---|---|
| Independent business tools | Help workers manage their own customer relationships and records |
| Collective fulfilment | Help compatible businesses coordinate larger orders |
| Group procurement | Help participants compare purchasing options together |
| Portable professional records | Help workers carry a structured history of skills and work |

The intended differentiation is the **connected workflow** between running an independent business, collaborating on larger opportunities and building a worker-controlled professional record.

This is a product hypothesis, not a claim that no other platform offers any of these individual features. Competitor research and field validation are required before making strong market-exclusivity claims.

---

## 9. Prototype features and interactions

The current repository contains a responsive frontend demonstration.

| Screen | What the evaluator can explore |
|---|---|
| Overview | Business summary, sample activity and featured 590-uniform opportunity |
| My Business | Sample customer orders, order statuses and search |
| Collective Orders | 590-uniform scenario, sample worker allocations and milestones |
| Group Procurement | Sample combined material requirement and supplier comparisons |
| Identity Passport | Sample professional profile, activity records, sharing choices and report download |

### Interactive elements
- Sidebar navigation between modules.
- Search through sample business orders.
- Open forms to simulate adding an order, posting an opportunity or requesting a quote.
- Demo action feedback for joining a group and viewing quotations.
- Selectable information categories for a sample shareable summary.
- Download a sample Professional Identity Passport as a text file.

### What happens when a user submits a form?

The current prototype displays a confirmation message to demonstrate the interface flow. It does **not** save the submitted information to a server or persistent database.

---

## 10. Technology used

### Current prototype

| Technology | Purpose |
|---|---|
| HTML5 | Page structure and semantic content |
| CSS3 | Layout, responsive styling and visual design |
| Vanilla JavaScript | Navigation, modal forms, filtering and demo interactions |
| Google Fonts | DM Sans and Manrope typography |
| Render Static Site | Suggested static hosting option |

The prototype intentionally avoids a complex build system so it can be opened locally and deployed quickly.

### Why this stack for the demo?

- No package installation is required.
- The project is easy for evaluators to run.
- The frontend can be hosted as a static site.
- The core user journeys can be demonstrated without pretending that backend services already exist.

---

## 11. Architecture of the current prototype

The current application is a static frontend.

```text
Browser
  |
  v
index.html
  |
  +---- styles.css
  |       Layout, colours, responsive design
  |
  +---- app.js
          |
          +---- Page navigation
          +---- Demo modal forms
          +---- Order search/filter
          +---- Toast notifications
          +---- Sample passport export
```

### Current data flow

- Sample records are embedded in the HTML.
- JavaScript controls frontend interactions.
- No API requests are made.
- No database is connected.
- No user authentication is implemented.
- Downloading the passport creates a local text file in the browser.

This is a prototype architecture, not the final production architecture.

---

## 12. Repository structure

```text
udyam-setu/
├── index.html          # Main application and demo screens
├── styles.css          # Responsive design and visual styles
├── app.js              # Frontend interactions and navigation
├── render.yaml         # Render static-site configuration
├── README.md           # Project documentation
└── docs/
    └── architecture.md # Product and future architecture notes
```

---

## 13. Run locally

### Requirements

- A modern web browser.
- Git, if cloning the repository.
- Python is optional and only needed for the simple local HTTP server shown below.

### Option 1 — open directly

1. Download or clone this repository.
2. Open the project folder.
3. Open `index.html` in a modern browser.

### Option 2 — run a local server

From the project directory:

```bash
python -m http.server 8000
```

Open:

```text
http://localhost:8000
```

Stop the server with `Ctrl + C`.

### Clone from GitHub

Replace the placeholder with the actual repository URL:

```bash
git clone https://github.com/YOUR-USERNAME/udyam-setu.git
cd udyam-setu
python -m http.server 8000
```

---

## 14. Deploy on Render

The included `render.yaml` describes a static site.

### Deploy using the Render dashboard

1. Push the project to a GitHub repository.
2. Sign in to Render.
3. Select **New → Static Site**.
4. Connect the GitHub repository.
5. Set the build command to blank.
6. Set the publish directory to `.`.
7. Create the static site and wait for deployment.
8. Open the generated URL and test the navigation and demo interactions.

### Deploy using the Blueprint

If using Render Blueprints, select the repository containing `render.yaml` and review the detected service configuration before deploying.

### Before submission

- Confirm the deployed URL loads.
- Test all five navigation items.
- Test the order search.
- Open and close each demo form.
- Test the passport download.
- Check the site on a mobile-sized screen.
- Ensure the repository and deployed URL are publicly accessible if the hackathon requires public access.

---

## 15. Proposed production architecture

The following is a **future implementation proposal**, not functionality currently present in this repository.

A production version would need secure authentication, persistent data, role-based permissions, audit trails and reliable workflows.

### Suggested stack

| Layer | Suggested technology | Responsibility |
|---|---|---|
| Frontend | Next.js or React | Responsive worker and institution interfaces |
| Styling | Tailwind CSS or CSS modules | Accessible, consistent UI |
| Backend | Node.js with a structured API | Business logic and validation |
| Database | PostgreSQL | Users, businesses, orders, allocations and records |
| Authentication | Supabase Auth or a comparable provider | Secure account access |
| File storage | Supabase Storage or equivalent | Consent-based supporting documents |
| Hosting | Render or another managed platform | Application deployment |
| Monitoring | Structured application logs and error monitoring | Reliability and issue diagnosis |

### Proposed service boundaries

```text
Worker / Buyer / Organisation
            |
            v
     Web or Mobile UI
            |
            v
      Secure API Layer
            |
   +--------+---------+----------------+
   |                  |                |
   v                  v                v
Business Service  Collective Service  Identity Service
   |                  |                |
   +------------------+----------------+
                      |
                      v
                 PostgreSQL
                      |
             Consent-controlled files
```

### Production modules

**Identity and access**
- Account registration and sign-in.
- Worker, buyer, supplier and organisation roles.
- Permission checks on every protected operation.
- Account recovery and session management.

**Business management**
- Customer and order CRUD operations.
- Quotations and invoice records.
- Transaction and expense entries.
- Exportable business data.

**Collective coordination**
- Opportunity creation and discovery.
- Worker applications and capacity declarations.
- Participant acceptance.
- Allocation and milestone tracking.
- Dispute and change-management workflows.

**Procurement**
- Group requirements.
- Supplier quotation requests.
- Quote comparison.
- Participant approvals.
- Procurement status and delivery records.

**Professional identity**
- Skill and experience records.
- Work-history entries.
- Customer confirmations.
- Evidence metadata.
- Consent and sharing controls.
- Downloadable reports and revocation of share access where supported.

---

## 16. Proposed data model

The following entities are a starting point for backend design.

| Entity | Example fields | Purpose |
|---|---|---|
| `users` | id, name, phone/email, created_at | Login identity |
| `businesses` | id, owner_id, name, category, location | Worker-owned business |
| `skills` | id, name, category | Standardised skill catalogue |
| `business_skills` | business_id, skill_id, experience_level | Skills associated with a business |
| `customers` | id, business_id, name, contact_consent | Customer records |
| `orders` | id, business_id, customer_id, description, amount, status | Individual business orders |
| `quotations` | id, order_id, version, amount, terms, status | Quotation history |
| `collective_orders` | id, buyer_id, title, quantity, deadline, status | Larger shared opportunity |
| `collective_members` | id, collective_order_id, business_id, status | Participating businesses |
| `worker_allocations` | id, member_id, quantity_or_scope, agreed_terms, status | Agreed individual work |
| `milestones` | id, collective_order_id, title, due_at, status | Project milestones |
| `contribution_records` | id, allocation_id, completed_quantity, evidence_status | Individual contribution |
| `supplier_requests` | id, collective_order_id, material, quantity, status | Group procurement request |
| `supplier_quotes` | id, supplier_id, request_id, price, terms, valid_until | Supplier quotation |
| `transactions` | id, business_id, order_id, amount, type, recorded_at | Business transaction records |
| `work_records` | id, business_id, source, confirmation_status, created_at | Professional activity history |
| `references` | id, work_record_id, reference_type, consent_status | Customer or institutional reference |
| `sharing_grants` | id, owner_id, recipient, scope, expires_at, revoked_at | Controlled sharing permissions |
| `audit_events` | id, actor_id, action, entity_type, entity_id, created_at | Security and accountability log |

### Important implementation notes

- Use unique IDs and foreign keys.
- Store money as integer minor units (for example, paise) with a currency code.
- Store timestamps consistently and display them in the user's local timezone.
- Keep original and updated quotation terms so changes are traceable.
- Do not overwrite contribution history when an allocation changes.
- Keep self-reported, customer-confirmed and evidence-supported records distinguishable.
- Restrict access to customer contact information.
- Use database transactions for operations that update multiple related records.

---

## 17. Trust, fairness, privacy and security

Trust is not an optional feature in a platform that coordinates independent workers. It is part of the product itself.

### Fair work allocation

A production implementation should:
- Show allocation proposals before acceptance.
- Make quantities, responsibilities, quality criteria and deadlines visible.
- Record participant acceptance.
- Allow participants to raise allocation or quality concerns.
- Record changes with timestamps and the reason for the change.
- Avoid opaque or discriminatory ranking.

### Professional record integrity

- A worker can create a self-reported entry.
- A customer can confirm only the work they are authorised to confirm.
- A platform-generated record should identify its source.
- Evidence should be handled with appropriate access controls.
- Disputed or withdrawn records should have a defined review process.
- No profile should imply government certification or formal accreditation unless such a credential has actually been issued by the relevant authority.

### Privacy and consent

- Collect only information needed for a defined purpose.
- Explain why personal information is requested.
- Let workers choose what professional records to share.
- Do not expose customer phone numbers or addresses to unrelated participants.
- Do not sell personal worker data.
- Provide a clear process for correcting inaccurate records and requesting account/data deletion, subject to applicable legal requirements.

### Application security

Before production, implement:
- Server-side validation for all input.
- Authentication and role-based authorisation.
- Secure password/session handling through a trusted provider.
- Rate limiting and abuse prevention.
- Protection against common web vulnerabilities.
- Secure file upload validation and access control.
- Secrets stored in environment variables, never committed to Git.
- Audit logs for sensitive actions.
- Backups and a tested recovery process.
- Dependency updates and security review.

The current static demo does not implement these production safeguards because it does not process real accounts or private records.

---

## 18. Accessibility and inclusion principles

The intended users may have different levels of digital familiarity, device capability and internet connectivity.

A production product should be designed around:

- Mobile-first layouts.
- Clear language and short instructions.
- Large, readable text and touch targets.
- High-contrast controls.
- Keyboard accessibility and visible focus states.
- Screen-reader-friendly labels.
- Local-language support.
- Low-bandwidth performance.
- Clear error messages and recovery paths.
- Minimal data entry and reusable records.
- Assisted onboarding through trusted community organisations where appropriate.

The interface should respect workers' skills and agency. It should never portray them as helpless or incapable.

---

## 19. Business model hypotheses

The following are potential revenue models to validate—not current revenue, signed contracts or proven willingness to pay.

| Potential customer | Possible paid offering |
|---|---|
| Individual workers | Optional premium business tools |
| Small business groups | Team coordination and advanced order tools |
| Institutional buyers | Order coordination and project dashboards |
| Suppliers | Supplier-side tools for responding to procurement requests |
| Cooperatives and NGOs | Onboarding and programme-management dashboards |

### Worker-first pricing principles

- Keep basic access to a worker's own professional records free.
- Do not require payment merely to view an opportunity.
- Disclose coordination fees before participants accept work.
- Never sell personal worker data.
- Test institutional willingness to pay before charging workers for essential features.
- Publish clear terms for cancellations, refunds and disputes before handling real transactions.

---

## 20. Validation plan

The product should be tested with real workers and potential buyers before claims about impact or market demand are made.

### Worker interviews

Speak with tailors or other target users and ask:

1. How do you currently record customer details and orders?
2. What happens when you receive an order that is larger than your available capacity?
3. Have you ever collaborated with another independent worker to complete an order?
4. How do you divide responsibilities, deadlines and payments?
5. How do you purchase materials, and how do you compare supplier prices?
6. What proof of skills or completed work do new customers ask for?
7. Which records would you want to take with you if you stopped using a particular platform?
8. Which part of this product would save you the most time or help you take on work?

### Buyer interviews

Speak with schools, housing societies, local businesses, cooperatives or other potential institutional buyers.

Ask:
- How do you currently find small suppliers or service providers?
- What makes you comfortable placing a large order with a group?
- What quality checks and delivery commitments are necessary?
- Would a single coordination dashboard be useful?
- What evidence would you need before accepting a group of independent businesses?

### What to measure in a pilot

- Time required to create a business profile.
- Percentage of invited workers who complete onboarding.
- Time required to form a group.
- Percentage of allocations accepted.
- On-time milestone completion.
- Order completion and buyer confirmation.
- Number of procurement quotes compared.
- Repeat participation.
- Worker understanding of payment and allocation terms.
- Accuracy and correction rate of professional records.

Do not report projected outcomes as measured impact.

---

## 21. Roadmap

### Phase 1 — hackathon prototype
- [x] Responsive frontend demo.
- [x] Business overview.
- [x] Sample business order table.
- [x] Illustrative collective 590-uniform workflow.
- [x] Sample procurement comparison.
- [x] Sample professional identity passport.
- [x] Basic interactions and sample report download.

### Phase 2 — functional MVP
- [ ] Worker and buyer registration.
- [ ] Secure authentication.
- [ ] Persistent database.
- [ ] Worker and business profiles.
- [ ] Customer and order management.
- [ ] Collective opportunity creation.
- [ ] Worker capacity declarations.
- [ ] Participant acceptance and allocation records.
- [ ] Milestone and contribution tracking.
- [ ] Consent-based work-history confirmations.

### Phase 3 — pilot-ready product
- [ ] Supplier onboarding and real quotations.
- [ ] Procurement commitments and delivery tracking.
- [ ] Notifications and reminders.
- [ ] Dispute and change-management workflows.
- [ ] Downloadable PDF reports.
- [ ] Local-language interface.
- [ ] Accessibility and low-bandwidth testing.
- [ ] Privacy and security review.
- [ ] Pilot with a small group of workers and one or more buyers.

### Phase 4 — expansion
- [ ] Adapt workflows for artisans and home-food businesses.
- [ ] Add service-team workflows for electricians and plumbers.
- [ ] Integrate with participating organisations where agreements exist.
- [ ] Develop interoperable record-sharing options.
- [ ] Evaluate sustainable institutional revenue models.

---

## 22. Demo walkthrough for evaluators

A suggested 3–4 minute walkthrough:

### 0:00–0:30 — Explain the problem

Introduce the 590-uniform scenario. Explain why a large order can be difficult for a single small tailoring business to fulfil.

### 0:30–1:00 — Show the overview

Open the dashboard and explain that Udyam Setu supports independent business management as well as collective opportunities.

### 1:00–1:45 — Show My Business

Open the order list. Explain how a worker can organise customer orders and business records.

### 1:45–2:40 — Show Collective Orders

Open the 590-uniform scenario. Walk through the illustrative group allocation and explain why transparent participant agreement matters.

### 2:40–3:10 — Show Group Procurement

Explain how participants can combine requirements and compare supplier quotations. Clarify that the displayed quotations are sample data.

### 3:10–3:40 — Show Identity Passport

Show the professional activity record and its sharing controls. Explain the distinction between self-reported and confirmed records.

### Closing statement

> Udyam Setu is built around a simple belief: workers should not have to give up their independence to access bigger opportunities. By helping them manage their own businesses, coordinate collective work and carry their professional history with them, we want to make it easier for small businesses to grow together.

---

## 23. Current limitations

Transparency matters. This repository is a frontend demo and should be evaluated as such.

| Area | Current state |
|---|---|
| User accounts | Not implemented |
| Authentication | Not implemented |
| Database | Not connected |
| Persistent records | Not implemented |
| Business orders | Sample data and demo-only form interactions |
| Collective order | Illustrative scenario |
| Allocation engine | Static example; no automated allocation |
| Procurement | Fictional supplier and quote examples |
| Payments | Not implemented |
| Verification | No real identity, customer or work verification |
| Passport | Sample text export only |
| Notifications | Not connected |
| External integrations | Not implemented |
| Analytics | Static sample figures |

The prototype is intended to communicate the product workflow and gather feedback. It must not be used to coordinate real paid work or store sensitive personal information.

---

## 24. Contributing

Ideas, feedback and improvements are welcome.

For a contribution:
1. Fork the repository.
2. Create a feature branch.
3. Make a focused change.
4. Test the interface at desktop and mobile widths.
5. Submit a pull request describing the change and how it was tested.

For substantial product changes, open an issue first to discuss the proposed workflow.

### Suggested contribution areas
- Local-language interface and translations.
- Accessibility improvements.
- Mobile usability.
- Worker onboarding flows.
- Better collective allocation UX.
- Documentation and user testing.
- Backend architecture and security review.

---

## 25. License

No open-source license has been selected for this prototype yet. Unless a license is added to the repository, all rights remain with the project authors by default. Contact the project maintainers before reusing or redistributing the code.

---

## 26. Team and acknowledgements

**Project:** Udyam Setu  
**Category:** Informal workforce empowerment / micro-enterprise enablement  
**Prototype type:** Hackathon frontend demo

Built to explore how accessible digital infrastructure can help independent workers manage their businesses, collaborate on larger opportunities and maintain portable professional records.

If you are evaluating this project, please start with the **590-school-uniform scenario** in the Collective Orders section. It demonstrates the central product idea in one workflow.

---

<p align="center">
  <strong>UDYAM SETU</strong><br>
  <em>Own Your Work. Grow Together.</em>
</p>
