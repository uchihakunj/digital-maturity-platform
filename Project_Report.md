# Digital Maturity Assessment Platform (Team-9)

<div align="center">
  <img src="images/iiit_logo.jpg" alt="IIIT Naya Raipur Logo" width="200" style="margin-bottom: 20px;">
  
  <h1>Project Report</h1>
  <p><strong>Course:</strong> Digital Transformation</p>
  <p><strong>Team Members:</strong> Sunil Kerketta, Raghwendra Kunjam, Vineet, Tejendra Kanwar, Vikas Rajput</p>
  <p><strong>Guided By:</strong> Dr. Krishna Bandaru</p>
</div>

---

## I. Introduction

### Problem Statement
In the rapidly evolving digital landscape, enterprises struggle to objectively measure their digital readiness. Departments often operate in silos with disparate technologies, cultural resistance, and outdated processes. Without a unified framework to assess maturity across critical dimensions, organizations cannot identify gaps or prioritize strategic investments effectively.

### Project Goal
The **Digital Maturity Assessment Platform** aims to provide a centralized, automated tool for evaluating organizational readiness. By assessing five key dimensions—Technology, Culture, Process, Skills, and Risk—the platform offers granular insights and actionable recommendations to drive digital transformation initiatives (Week 1: Concepts, Trends).

### Context
This project serves as an enabler for broader transformation strategies, moving organizations from ad-hoc digitization to optimized, data-driven ecosystems.

---

## II. Solution Architecture

### Architectural Overview (System & Tech Viability)
The solution follows a streamlined **Micro-MVC (Model-View-Controller)** architecture designed for agility and rapid deployment (Week 4: Enterprise Architecture).

*   **Frontend (View):** Built with **Streamlit**, offering a responsive, interactive web interface. It ensures accessibility across devices and minimizes development overhead for internal tools.
*   **Backend (Controller):** **Python** serves as the core logic engine, handling data processing, scoring algorithms (`logic.py`), and visualization rendering via **Plotly**.
*   **Database (Model):** **SQLite** (`database.py`) provides a lightweight, serverless relational database solution, ideal for the PoC phase with easy scalability paths to PostgreSQL/Cloud SQL (Week 7: Cloud Computing).
*   **Deployment:** The application is container-ready and currently deployed via **Streamlit Cloud**, ensuring high availability and ease of access.

### Justification
*   **Streamlit & Python:** Chosen for their dominant position in Data Science/Analytics, allowing for rapid iteration of the scoring model without complex frontend code.
*   **Plotly:** Enables dynamic, interactive visualizations (Radar charts, Heatmaps) essential for executive decision-making.

---

## III. Proof of Concept (PoC) & Implementation

### Functionality
The PoC demonstrates the core value proposition through a fully functional web application:
1.  **Assessment Interface:** Interactive forms capture qualitative data across 5 dimensions.
2.  **Maturity Dashboard:** Real-time visualization of data using Heatmaps and Radar charts to identify organizational strengths and weaknesses (Week 5/6: AI & Data Analytics).
3.  **Automated Roadmap:** A rule-based engine (`logic.py`) generates tailored strategic recommendations (e.g., "Legacy systems detected -> Prioritize cloud migration") and exports them as PDF reports.
4.  **Bulk Upload:** Supports CSV ingestion for enterprise-wide data processing.

### Dataset
The system presently uses synthetic data representing various departmental profiles (Finance, HR, IT) to validate the scoring algorithms and visualization logic. The database structure (`assessments` table) allows for seamless integration of real-world survey data.

### Code Quality
The codebase is structured into modular components: `app.py` (UI), `logic.py` (Business Rules), and `database.py` (Data Persistence), adhering to clean coding standards and maintained in a Git repository.

---

## IV. Business Model & Value

### Value Proposition
The platform transforms consulting-heavy, manual assessment processes into a scalable, self-service digital product. It democratizes access to strategic insights, allowing mid-sized enterprises to benchmark themselves without expensive external audits (Week 3: Digital Business Models).

### ROI Quantification
*   **Cost Reduction:** Automates the data collection and analysis phase, reducing assessment time by approximately **70%** compared to manual interviews.
*   **Strategic Alignment:** Ensures IT spend is targeted at high-impact areas (e.g., upskilling vs. software purchase) based on empirical data rather than gut feeling.
*   **Revenue Impact:** Accelerates time-to-market for digital initiatives by identifying and removing bottlenecks early.

---

## V. Risk & Governance

### Cybersecurity & Privacy
*   **Data Minimization:** The system collects only essential departmental metrics, avoiding Personally Identifiable Information (PII) where possible (Week 9: Cybersecurity & Privacy).
*   **Access Control:** Deployment via secured cloud environments ensures restricted access to sensitive maturity data.

### Change Management
*   **User Adoption:** The simple, form-based interface reduces friction for non-technical users.
*   **Organizational Enablement:** The "Roadmap" feature acts as a change agent, providing clear, step-by-step instructions that empower department heads to take ownership of their transformation journey (Week 10).

---

<div align="center">
  <p><em>Submitted as part of the Digital Transformation Course Requirements.</em></p>
</div>
