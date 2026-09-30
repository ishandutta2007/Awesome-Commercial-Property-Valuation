# Awesome-Commercial-Property-Valuation

# Top Commercial Property Valuation Platforms Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**
*Focused on Commercial Real Estate DCF Modeling, Mass Appraisal, Lease Abstraction & Deal Underwriting*
**Last updated: September 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Commercial Property Valuation**. These tools help appraisers, investors, and asset managers value office, retail, industrial, and multifamily assets using income, sales comparison, and cost approaches.

**Examples** include Argus Enterprise, Valcre, LightBox Valuation, Reonomy, CompStak, HouseCanary, Cherre, Crexi Intelligence, Dealpath Analytics, and PropMix (the category leaders).

**Open-source emphasis**: Commercial property valuation is a **commercially dominated category**—Argus Enterprise is virtually the industry standard for institutional DCF modeling. However, the **open-source foundation is maturing rapidly**. **Rangekeeper** decomposes DCF proforma modeling into recomposable code functions, supporting full-resolution modeling from early estimates to detailed commercial appraisals . **OpenAVMKit** provides a complete Python library for mass appraisal . **cre.dcf** delivers R-based commercial real estate DCF tools including debt scheduling, DSCR, and LTV calculations . **CRE Agent Skills** offers 90 AI agent skills covering underwriting, lease abstraction, and due diligence . **SignalTruth** reconstructs real estate market intelligence from public records with confidence scoring . **RICS Data Standards** provide an MIT-licensed data exchange standard .

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Argus Enterprise](https://www.altusgroup.com/argus/)**
  **The de facto standard for commercial real estate valuation.** Altus Group's flagship product, used for virtually all institutional CRE underwriting and DCF modeling. Provides cash flow projections, lease modeling, and valuation reports for office, retail, industrial, and multifamily assets. **Argus Cloud MCP** (Vinkius) provides 6 tools enabling AI agents to connect directly to Argus Cloud data for asset inventory, valuation tracking, portfolio details, and notification review .

- **[Valcre](https://www.valcre.com/)**
  Valuation platform designed specifically for appraisers. Provides data collection, comparable sales analysis, income approach modeling, and report generation with workflow management for appraisal firms.

- **[LightBox Valuation](https://www.lightboxre.com/)**
  Commercial real estate data and analytics platform. Provides valuation tools, market data, and due diligence support across the U.S. commercial property market.

- **[Reonomy](https://www.reonomy.com/)**
  Commercial real estate data platform. Provides property ownership, loan, sales history, and tenant information supporting underwriting and valuation analysis.

- **[CompStak](https://www.compstak.com/)**
  Commercial lease comparable data platform. Crowdsources lease comps to provide market rent and terms data for appraisals and underwriting.

- **[HouseCanary](https://www.housecanary.com/)**
  Residential and commercial property valuation analytics platform. Provides AVM, market trends, and portfolio analysis.

- **[Cherre](https://cherre.com/)**
  Real estate data connection and insight platform. Unifies multi-source data for valuation, underwriting, and asset management decisions.

- **[Crexi Intelligence](https://www.crexi.com/)**
  Data and analytics module within the Crexi platform. Provides valuation tools, market trends, and transaction data.

- **[Dealpath Analytics](https://www.dealpath.com/)**
  Investment management platform providing deal pipeline, underwriting analysis, and portfolio management with valuation tracking.

- **[PropMix](https://propmix.io/)**
  Real estate data and analytics platform. Provides property valuation, market analysis, and data API services.

## Open-Source GitHub Projects

### DCF Modeling & Valuation Engines

- **[Rangekeeper](https://github.com/daniel-fink/rangekeeper)**
  **The most mature open-source library for commercial real estate financial modeling.** Decomposes **DCF proforma modeling methods** into recomposable code functions that can be flexibly combined into complete models . **Full-resolution valuation**: from early "back-of-envelope" estimates to detailed commercial appraisals, fully synchronized with 3D design, engineering, and logistics modeling. Development follows the rigorous methodology established by Professors **Geltner and de Neufville** in *Flexibility and Real Estate Valuation under Uncertainty*. **Python library** + Jupyter Book documentation + Rhino Grasshopper component (C#). **Open source**.

- **[cre.dcf](https://cran.r-project.org/package=cre.dcf)**
  **Commercial real estate DCF toolkit for R.** Builds **unlevered and levered DCF tables**, generates bullet and amortizing debt schedules, and calculates **DSCR, debt yield, and forward LTV** . Provides an explicit property-level operating chain from **GEI (Gross Effective Income) to NOI (Net Operating Income) to PBTCF (Pre-Tax Cash Flow)**. Supports end-to-end scenario execution from **YAML configuration files**. **MIT licensed**, **published on CRAN**, version 0.0.5 (April 2026).

### Mass Appraisal (AVM)

- **[OpenAVMKit](https://pypi.org/project/openavmkit/)**
  **Python library for mass appraisal of real estate.** Contains modules for data cleaning, data enrichment, modeling, and statistical evaluation of prediction models, plus Jupyter Notebook workflow examples . **Published on PyPI**. Suited for appraisal districts, tax assessment, and portfolio valuation use cases.

- **[CCAO Residential AVM (Cook County)](https://github.com/ccao-data/model-res-avm)**
  **Open-source residential AVM from the Cook County Assessor's Office.** **57 stars, 17 forks**, **AGPL-3.0 licensed**, **R language** . Uses **LightGBM** as the primary model, chosen for its documentation, accuracy, speed, native categorical feature support, and widespread use in housing ML models. Provides **SHAP values** for individual property explanation, and aggregate feature importance based on LightGBM's built-in methods . **Production deployment**: used to value all class 200 residential properties (excluding vacant land and condos) in Cook County.

- **[dmai287/real-estate-avm](https://github.com/dmai287/real-estate-avm)**
  Open-source AVM using **linear regression, random forest, and XGBoost** trained on MLS data for Chicago, Dallas, and Denver . Provides data ingestion, preprocessing, feature engineering, model evaluation (RMSE, MAE, R²), and a RESTful API. **Jupyter Notebook format**.

### AI Agent Skills & Workflows

- **[CRE Agent Skills](https://github.com/ahacker-1/cre-agent-skills)**
  **90 open-source AI agent skills covering the full commercial real estate underwriting, lease abstraction, and due diligence lifecycle.** **Apache 2.0 licensed, completely free** . **Nine skill packs**: Multifamily Acquisition Core, Industrial, Brokerage Investment Sales, Asset Management, Office, Capital Markets, Retail, Lender & Credit, and Development & Construction. **Representative skills**: rent roll analysis, lease abstract review, lease-by-lease underwriting, market and comps research, debt sizing and refinance gap analysis, guarantor review, construction draw review, covenant monitoring, and investment committee memo drafting. **35 knowledge bases**, 93 research notes, 14 Claude Code plugins. **No API keys, no installation, no dependencies**—runs directly in Claude, ChatGPT, and Cursor .

- **[cre-skills-plugin](https://github.com/mariourquia/cre-skills-plugin)**
  **100+ institutional-grade CRE skills for Claude Code, Desktop, and Cowork.** Covers deal screening, underwriting, structuring, capital markets, asset management, leasing, investor relations, development, and disposition . **50+ expert agents, 12+ Python calculators, 10+ orchestration pipelines**. **Decision-grade outputs** are labeled with explicit **human gates** (analyst review, AM/CFO sign-off, IC approval). **Apache 2.0 open-source core**, with a Pro version offering an institutional governance layer (lifecycle hooks, four-eyes approval matrix, audit logs).

### Data Standards & Infrastructure

- **[RICS Data Standards](https://www.rics.org/)**
  **RICS official data standards, MIT licensed.** Merge **IPMS and ICMS** into a single schema covering data capture, sharing, and exchange for land, property, real estate, and infrastructure assets . Supports XML and JSON formats with HTML documentation. References RICS and international standards covering property measurement, valuation, due diligence, lifecycle costing, carbon emissions, building operations, brokerage, leasing, and construction measurement.

- **[OSCRE Industry Data Model](https://www.oscre.org/)**
  Commercial real estate data standard with **over 1,200 end-user license agreements** completed since becoming freely available in 2020 . The **OSCRE Enterprise Toolkit** ($1,195) provides 180+ use cases, XML/JSON schemas, and UML data model visualizations. The **Development Handover** use case standardizes data transfer from new development to asset management .

- **[IBPDI Common Data Model](https://github.com/ibpdi/cdm)**
  **Open-source real estate common data model from the International Building Performance & Data Initiative (IBPDI).** Defines standard entities (area measurement, building, price, cost, climate, etc.) to promote data interoperability . **Modular clusters**: Energy & Resources, Portfolio Management, Asset Management, Property Management, Facility Management, Transaction Management, Market Data, User Experience, Finance, Project Management, Organization Management, Documents, Order Management. **MIT licensed (code) / CC-BY-4.0 (documentation)**.

- **[SignalTruth](https://roxanneardary.com/signaltruth/)**
  **Modular open-source commercial real estate intelligence system that reconstructs markets from public records.** **AGPL 3.0+ licensed** . Builds a **living property graph**: ownership changes, lease events, permits, liens, and valuation updates as continuous records. **Confidence scoring**: every output carries quantified confidence, source attribution, and method traceability. **Completeness detection** identifies missing or inconsistent public record data. **Market modules** analyze comps, pricing trends, and vacancy dynamics. **Legal intelligence module** maps jurisdictional rules into structured, queryable logic.

### Additional Strong Open-Source Options

- **DCF Modeling**: **Rangekeeper** (Python, recomposable functions, Geltner methodology), **cre.dcf** (R, CRAN, YAML configuration, DSCR/LTV).
- **Mass Appraisal**: **OpenAVMKit** (Python, complete AVM pipeline), **CCAO AVM** (R/LightGBM, production deployment, SHAP).
- **AI Skills**: **CRE Agent Skills** (90 skills, Apache 2.0), **cre-skills-plugin** (100+ skills, human gates).
- **Data Standards**: **RICS** (MIT, IPMS+ICMS), **OSCRE IDM** (180+ use cases), **IBPDI CDM** (13 clusters).
- **Market Intelligence**: **SignalTruth** (public records graph, confidence scoring).

**Frameworks for building custom systems**: Combine **Rangekeeper** or **cre.dcf** as the DCF modeling engine, **OpenAVMKit** or **CCAO AVM** for mass appraisal, **CRE Agent Skills** for AI-assisted underwriting and lease abstraction, **SignalTruth** for public records market intelligence, and **RICS/OSCRE/IBPDI** standards for data interoperability. Add **PostgreSQL** for persistence and **Python/R** ecosystems for analysis and modeling.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Commercial property valuation platforms handle sensitive financial and property data; ensure compliance with appraisal standards (USPAP, IVS) and relevant regulations.
- **Open-source reality**: The open-source ecosystem for commercial property valuation is **maturing rapidly** at the **DCF modeling** (Rangekeeper, cre.dcf), **mass appraisal** (OpenAVMKit, CCAO AVM), and **AI-assisted workflow** (CRE Agent Skills) layers. **RICS, OSCRE, and IBPDI** provide open data standard foundations . However, **Argus Enterprise** remains the **de facto standard** for institutional DCF modeling, lease abstraction, and portfolio management, and open-source alternatives still have significant gaps in **lease-level cash flow modeling precision, institutional-grade report output, and industry adoption**. The open-source path is best suited for **appraisal research, mass AVM, AI-assisted underwriting**, or **data standardization projects** rather than directly replacing Argus production valuation workflows.

---

**Made for commercial real estate appraisers, investment analysts, asset managers, underwriting teams, and PropTech developers.**
Let's make commercial property valuation more open, transparent, and data-driven.
