# S.M Touker Ahmed

**Senior Full-Stack & Backend Systems Engineer**  
📍 Dhaka, Bangladesh &nbsp;|&nbsp; ✉️ [ahamed.touker@gmail.com](mailto:ahamed.touker@gmail.com) &nbsp;|&nbsp; 📞 [+880 1794-621250](tel:+8801794621250)  
🔗 [LinkedIn](https://www.linkedin.com/in/toukerahmed/) &nbsp;|&nbsp; 💻 [GitHub](https://github.com/toukerahmed) &nbsp;|&nbsp; 🦊 [GitLab](https://gitlab.com/toukerahmed) &nbsp;|&nbsp; 🥞 [Stack Overflow](https://stackoverflow.com/users/16973138/touker-ahmed) &nbsp;|&nbsp; 📄 [Download PDF Resume](./Touker-Ahmed-Resume.pdf)

---

## Executive Profile

Senior Full-Stack & Backend Systems Engineer with **5+ years of production experience** architecting high-reliability web applications, enterprise ERPs, multi-tenant systems, and mission-critical back-offices. Specialized in **PHP (7.x - 8.4), Laravel (8 through 13), JavaScript (ES6+), TypeScript, React.js, Angular (15), Python (Django REST Framework), Node.js (Socket.io), and MySQL**.

Extensive domain experience across **enterprise healthcare (HMS & EMR), conglomerate logistics (Akij Group), retail multi-tenant inventory with immutable ledgers, FinTech payment checkout (PortPOS), cross-border e-commerce (Alibaba 1688 API), and national GovTech portals (Prottoyon)**. Direct experience designing database-per-tenant isolation, append-only stock ledgers, complex role-based access control (RBAC), background queue workers (Redis & Laravel Horizon), and headless document generation engines (Spatie Browsershot & Puppeteer).

---

## Core Technical Competencies

| Domain | Verified Technologies & Architectural Patterns |
| :--- | :--- |
| **Backend & Architecture** | PHP (7.x – 8.4), Laravel (8 to 13), Livewire 4, Python (Django REST Framework, ASGI/WSGI), Node.js (Express, Socket.io), Microservices, Modular Monoliths, MVC, Database-per-Tenant Multi-Tenancy |
| **Frontend & UI Systems** | JavaScript (ES6+), TypeScript, React.js, Angular 15, Angular Material, RxJS, Alpine.js, Tailwind CSS, Bootstrap, jQuery, Ajax, Responsive Web Design |
| **Databases & Data Modeling** | MySQL, MariaDB, SQLite, Oracle, Append-Only Ledgers, Relational Indexing Strategies, Query Optimization, Transactional Isolation, Schema Migrations |
| **Security & Authorization** | Granular Role-Based Access Control (RBAC), Spatie Laravel-Permission, Two-Factor Authentication (2FA / Laraguard), Laravel Sanctum, JWT Token Rotation, Audit Logging |
| **DevOps, Queues & Tooling** | Git, GitHub, GitLab, Redis, Laravel Horizon, Background Queue Workers, Headless Puppeteer / Spatie Browsershot, Linux CLI, CI/CD Pipelines |
| **Hardware, IoT & Real-Time** | Arduino, Raspberry Pi, Hardware Telemetry, Camera Node Authentication, WebSockets (Socket.io), Real-Time Push (Firebase) |

---

## Professional Experience

### **Senior Full-Stack & Backend Systems Engineer**  
**Lorapok Labs** &nbsp;|&nbsp; *Dhaka, Bangladesh*  
**Jun 2026 – Present**

- **Enterprise Hospital Management System (Lorapok-HMS):** Architecting full-lifecycle medical automation platform covering Outpatient (OPD) scheduling, Inpatient (IPD) admissions, Electronic Medical Records (EMR), and unified billing. Implemented normalized doctor/nurse availability schedules as validated JSON arrays, integrated Firebase real-time alerts, and managed background job processing using Redis Horizon.
- **Lorapok Retail & Inventory ERP:** Engineered multi-tenant inventory and POS engine featuring database-per-tenant isolation, append-only stock movement ledgers (`stock_movements`), server-authoritative pricing, zero-float integer currency columns, and weighted-average profit margin freezing.
- Lead system performance tuning, profiling high-volume database queries, and standardizing automated CI/CD workflows for multi-tenant deployments.

---

### **Software Engineer**  
**DebugVision** &nbsp;|&nbsp; *Dhaka, Bangladesh*  
**Jan 2024 – Aug 2026**

- **Akij Group Logistics Platform:** Built and maintained enterprise freight management systems for Akij Group managing end-to-end import/export shipment milestones, automated House Bill of Lading (HBL) generation, and headless PDF rendering using Spatie Browsershot and Puppeteer.
- **Government Citizen Certificate Portal (Prottoyon):** Maintained national civic certificate portal for local government divisions, implementing two-factor authentication (`Laraguard`), cryptographic QR verification tokens, and administrative approval chains.
- Designed and enforced granular Role-Based Access Control (RBAC) layers ensuring multi-tenant data privacy across enterprise accounts.
- Optimized MySQL database schemas and indexing structures, eliminating query bottlenecks and accelerating execution times by up to 40%.

---

### **Software Engineer**  
**TechWeb BD IT** &nbsp;|&nbsp; *Dhaka, Bangladesh*  
**Feb 2022 – Dec 2023**

- **PortPOS Angular 15 Frontend:** Developed high-speed single page application frontend with Angular 15, Angular Material, and reactive RxJS for Portonics PortPOS checkout and payment terminals.
- **SkyBuyBD & 1688 Cross-Border E-Commerce:** Built B2B/B2C cross-border sourcing platform integrating Alibaba 1688 Open APIs, real-time multi-currency exchange rate calculators, and volumetric freight tariff algorithms.
- **SOI CCTV Surveillance Backend:** Engineered Python Django REST Framework backend with custom authentication (`custom_auth.py`) and ASGI streaming endpoints for distributed camera hardware.
- Designed standardized multi-environment deployment pipelines and staging checklists to ensure reliable zero-surprise releases.

---

### **Software Engineer**  
**Avanteca Limited** &nbsp;|&nbsp; *Dhaka, Bangladesh*  
**May 2020 – Jan 2022**

- **Home Dyn & Canteen POS System:** Developed restaurant floor operations platform featuring digital Kitchen Order Ticketing (KOT), barcode scanning integration (`milon/barcode`), cashier POS checkout, and recipe-based ingredient depletion.
- **Portlink Logistics Document Automation (PDF-to-Excel):** Automated ingestion of non-standardized PDF freight documents into structured customs-ready Excel spreadsheets.
- Refactored legacy SQL queries and database routines, accelerating administrative report generation and reducing server memory usage.

---

## Detailed Production Projects

### 🏥 **1. Lorapok Medical Automation System (HMS & EMR)**
*Enterprise Healthcare Operating System & Electronic Medical Records* &nbsp;`[Lorapok Labs Flagship]`
- **Tech Stack:** Laravel 11, PHP 8.4, MySQL, Redis / Laravel Horizon, Firebase, Laravel Sanctum, CKEditor 5, RBAC
- **The Challenge:** Specialized multi-disciplinary medical facilities struggle with fragmented Electronic Medical Records (EMR), communication bottlenecks between OPD and IPD wards, doctor availability scheduling, pharmacy stock leakage, and slow invoice consolidation across beds, diagnostic tests, and dispensations.
- **Architectural Solution:** Architected an enterprise-grade hospital digital operating system integrating patient registration, doctor/nurse scheduling with JSON array availability attributes, clinical progress notes (CKEditor 5), IPD admission workflows, pharmacy inventory auditing, and unified ledger billing with OTP-gated authentication and Redis Horizon queue management.
- **Key Contributions & Features:**
  - Granular Role-Based Access Control (RBAC) across Doctors, Nurses, Pharmacists, Lab Technicians, Billing Clerks, and Super Admins.
  - Normalized doctor & nursing staff availability engine storing dynamic multi-slot schedules as validated JSON arrays.
  - Queue-driven background processing using Laravel Horizon & Redis for asynchronous report generation and automated billing alerts.
  - Firebase integration for real-time mobile push notifications and clinical state synchronization.
  - Complete clinical workflow: OPD appointments, IPD bed allocations, doctor rounds, diagnostic test tracking, and pharmacy dispensation.
  - Consolidated financial ledger automatically compiling doctor consultation fees, diagnostic lab tests, bed charges, and medication costs into audited invoices.

---

### 📦 **2. Lorapok Retail & Multi-Tenant Inventory ERP**
*Multi-Tenant POS & Serialized Goods Inventory for Retail Chains* &nbsp;`[Lorapok Labs]`
- **Tech Stack:** Laravel 13, Livewire 4, PHP 8.4, MySQL (Multi-Database per Tenant), Tailwind CSS, Alpine.js, CI/CD
- **The Challenge:** Retailers selling serialized goods (such as electronics and mobile devices with IMEI numbers) face inventory drift, float-rounding currency errors, untracked price tampering at the cash register, and retrospective profit margin distortion when restocking at fluctuating supplier costs.
- **Architectural Solution:** Engineered a database-per-tenant multi-tenant retail inventory and POS architecture with an append-only stock movement ledger, server-authoritative pricing, and strict currency calculations.
- **Key Contributions & Features:**
  - **Database-per-tenant isolation:** Each business gets an automated subdomain and dedicated MySQL database for complete security isolation.
  - **Append-only stock ledger:** `stock_movements` is strictly append-only (never updated, never deleted). `stock_levels` is a derived transactional cache validated by `stock:reconcile` CLI command.
  - **Immutable margin freezing:** Every sale freezes weighted-average cost at transaction time, preserving historic profit accuracy regardless of future supplier restocking costs.
  - **Strict currency integrity:** Zero float rounding. All prices stored as integer minor units (`*_minor`) with explicit currency codes, enforced by automated architecture tests.
  - **Server-authoritative pricing:** Cashiers cannot manipulate line totals or final balances; unauthorized price overrides are neutralized on the backend.
  - **Audit-trailed voiding:** Transactions are corrected exclusively via compensating entries rather than destructive deletions.

---

### 🚢 **3. Akij Group Logistics & Freight Management System**
*Enterprise Freight Operations, HBL Automation & Milestone Tracking* &nbsp;`[Akij Group]`
- **Tech Stack:** Laravel, PHP, MySQL, Spatie Laravel-Permission (RBAC), Spatie Browsershot, Headless Puppeteer, RESTful APIs
- **The Challenge:** Managing international freight forwarding across air and sea imports/exports requires strict House Bill of Lading (HBL) compliance, dynamic freight rates with fluctuating foreign exchange rates, and real-time transit visibility where manual documentation leads to port clearance penalties.
- **Architectural Solution:** Architected a comprehensive logistics management platform for Akij Group managing end-to-end import and export shipment lifecycles, automated HBL generation and issuance, headless browser PDF printing via Spatie Browsershot & Puppeteer, and multi-currency exchange rate engines.
- **Key Contributions & Features:**
  - End-to-end import and export shipment tracking with quick-store dispatching, inline status updating, and soft-delete restorations.
  - Complete House Bill of Lading (HBL) registry: automated generation, JSON export, verification, and formal issuance workflows.
  - Server-side pixel-perfect PDF rendering and printing of compliant HBL documents utilizing Spatie Browsershot and headless Puppeteer.
  - Dynamic rate calculation engine managing master freight rates, local port charges, and multi-currency exchange conversion rates.
  - Operational intelligence: Comprehensive import/export dashboards, carrier performance metrics, and ETD/ETA milestone tracking.
  - Enterprise access security: Gated by Spatie Laravel-Permission with user auditing and system activity logs.

---

### 💳 **4. PortPOS Payment Gateway & Checkout Frontend**
*FinTech Point-of-Sale Terminal & Payment Gateway UI* &nbsp;`[Portonics]`
- **Tech Stack:** Angular 15, TypeScript, Angular Material, RxJS, Angular CDK, Node.js, REST APIs
- **The Challenge:** Cashiers and merchants require a rapid, responsive, and fault-tolerant checkout frontend interface capable of executing complex payment routing, order splitting, and instant refund verifications without UI latency.
- **Architectural Solution:** Built a modular, high-speed single page application frontend with Angular 15, Angular Material, and reactive RxJS state management connecting to PortPOS gateway APIs.
- **Key Contributions & Features:**
  - Rapid order creation workflow supporting multi-item selection, quantity adjustments, and dynamic tax calculation.
  - Order management and refund administration engine with role-gated approval thresholds.
  - Modern Angular Material design system with fluid animations, keyboard navigation, and responsive touch layout.
  - Asynchronous HTTP interceptors for JWT token rotation, error telemetry, and retry resilience.

---

### 🏛️ **5. Prottoyon — Government Citizen Certificate System**
*GovTech Digital Public Infrastructure for Local Government Divisions* &nbsp;`[Public Sector]`
- **Tech Stack:** Laravel 8, PHP, MySQL, Laraguard (2FA), JavaScript, Bootstrap, Security RBAC
- **The Challenge:** Civic certificate issuance across municipal and upazilla offices traditionally involved manual paper handling, long citizen queues, risk of counterfeit certificates, and lack of central auditability.
- **Architectural Solution:** Engineered 'Prottoyon', an online civic portal empowering citizens to apply digitally for character, nationality, and birth certificates with multi-tier administrative approval, 2FA security, and unique verification tokens.
- **Key Contributions & Features:**
  - Digital citizen application submission with document verification, automated tracking, and status alerts.
  - Multi-stage administrative review and digital signature authorization hierarchy for municipal officials.
  - Two-factor authentication (2FA) for administrative accounts powered by `darkghosthunter/laraguard`.
  - Cryptographic QR code and verification token embedded in issued certificates for instant real-time authenticity validation.
  - Comprehensive immutable audit logging recording administrative views, approvals, and issuance timestamps.

---

### 📹 **6. SOI CCTV Surveillance System Backend**
*Real-Time Surveillance Telemetry & Camera Device Management* &nbsp;`[Security Infrastructure]`
- **Tech Stack:** Python, Django REST Framework, ASGI / WSGI, MySQL, Custom Auth, IoT Protocols
- **The Challenge:** Managing distributed CCTV surveillance hardware requires low-latency event ingestion, device telemetry, custom token-based camera authorization, and reliable video stream routing across concurrent monitoring stations.
- **Architectural Solution:** Engineered a high-performance Python Django REST Framework backend with custom authentication, ASGI/WSGI asynchronous streaming interfaces, and relational schema modeling for camera nodes and event feeds.
- **Key Contributions & Features:**
  - Custom token authentication layer (`custom_auth.py`) validating distributed CCTV field hardware and security stations.
  - High-throughput RESTful API endpoints for camera telemetry, device heartbeat monitoring, and incident recording.
  - Asynchronous ASGI request processing for real-time surveillance status updates and alert broadcasting.
  - Relational data schema optimized for rapid querying of historical camera logs, incident timestamps, and device operational statuses.

---

### 📑 **7. Portlink Logistics Document Automation (PDF-to-Excel)**
*Freight Manifest Ingestion & Customs Spreadsheet Pipeline* &nbsp;`[Portlink Logistics]`
- **Tech Stack:** Laravel / PHP, Python Data Parsers, MySQL, Spreadsheet Automation, JavaScript, Bootstrap
- **The Challenge:** Freight forwarders receive hundreds of non-standardized PDF air waybills (HAWB) and cargo manifests daily. Clerks spent hours manually transcribing numbers into spreadsheets, leading to costly data entry errors.
- **Architectural Solution:** Created an automated document processing pipeline ingesting PDF freight documents, extracting structured cargo milestones and consignee records, and generating compliant Excel reports for customs brokers.
- **Key Contributions & Features:**
  - Automated PDF document parser transforming unstructured air waybills into validated tabular data.
  - Validation engine flagging missing weight declarations, invalid tariff codes, and duplicate HAWB numbers.
  - High-speed export engine generating structured multi-sheet Excel workbooks formatted for customs submission.
  - Role-based administrative portal with audit logs and historical document archiving.

---

### 🛒 **8. SkyBuyBD & 1688 Cross-Border E-Commerce**
*High-Throughput B2B & B2C Sourcing Platform* &nbsp;`[Production Architecture]`
- **Tech Stack:** Laravel, PHP, 1688 Open APIs, MySQL, RESTful APIs, JavaScript, Redis
- **The Challenge:** Importing products directly from Alibaba 1688 to local markets requires translating product catalogs, converting currencies in real-time, calculating volumetric freight tariffs, and preventing duplicate order fulfillment during checkout spikes.
- **Architectural Solution:** Built an enterprise cross-border e-commerce and order management back-office connecting directly to 1688 APIs with real-time currency conversion, automated order duplication guards, and live transit tracking.
- **Key Contributions & Features:**
  - 1688 API integration synchronizing product listings, variants, inventory levels, and wholesale price tiers.
  - Dynamic currency and landed cost calculator factoring international shipping, customs tariffs, and local delivery.
  - Order duplication prevention engine resolving concurrent checkout requests and multi-vendor order routing.
  - End-to-end customer order tracking pipeline from China consolidation warehouses to local door-to-door delivery.

---

### 🍽️ **9. Home Dyn & Canteen Operations Management**
*Restaurant Floor POS, Kitchen Ticketing & Ingredient Depletion* &nbsp;`[Live Production]`
- **Tech Stack:** Laravel, PHP, MySQL, Barcode Engine (`milon/barcode`), JavaScript, jQuery, CSS3
- **The Challenge:** Busy food service operations struggle with lost handwritten order tickets, slow kitchen dispatching, manual bill splitting during peak lunch hours, and unmonitored raw ingredient depletion.
- **Architectural Solution:** Developed a comprehensive dining management system featuring digital Kitchen Order Ticketing (KOT), barcode-assisted order identification, cashier POS billing, and recipe-based ingredient depletion.
- **Key Contributions & Features:**
  - Real-time Kitchen Order Ticketing (KOT) routing floor orders directly to kitchen preparation stations.
  - High-speed cashier POS interface with barcode scanner support, bill splitting, and instant thermal receipt printing.
  - Automated ingredient inventory depletion tracking stock deductions according to standardized recipe specifications.
  - Cashier shift closing and daily sales audit reporting.

---

### 💬 **10. High-Concurrency WebSocket Communication Engine**
*Real-Time Bi-Directional Messaging Infrastructure* &nbsp;`[Node.js Engine]`
- **Tech Stack:** Node.js, Express, Socket.io, UUID, JavaScript ES6+, HTML5/CSS3
- **The Challenge:** Modern business web applications require real-time collaboration, instant user-to-user communication, and synchronized operational status alerts without polling server overhead.
- **Architectural Solution:** Built a scalable real-time messaging engine with Node.js, Express, and Socket.io with persistent user state mapping, UUID tracking, and message history caching.
- **Key Contributions & Features:**
  - Bi-directional WebSocket messaging with sub-10ms delivery latency.
  - Persistent connection state management tracking active user sessions and automated disconnect handling.
  - Synchronized message deletion across connected clients with UUID validation.
  - In-memory chat history buffering with automatic sliding-window memory reclamation.

---

## Engineering Philosophy & Principles

1. **Understand the Workflow First**  
   Software architecture must reflect real-world business realities. I collaborate closely with operators and stakeholders to map domain processes thoroughly before writing schema migrations or code.

2. **Access Control by Design (RBAC)**  
   Data security and authorization cannot be an afterthought. Granular permissions, role validation middleware, and tenant isolation are engineered into the database and application core from day zero.

3. **Fast Data & Resilient Deploys**  
   A platform is only as fast as its slowest query. I prioritize clean relational modeling, strategic indexing, and standardized deployment checklists to ensure zero-downtime, predictable production releases.

4. **Engineered for the Next Developer**  
   Code is read far more often than it is written. I adhere to clean coding conventions, modular component boundaries, meaningful commit histories, and self-documenting technical specifications.

---

## Education

**Bachelor of Science in Computer Science and Engineering (B.Sc CSE)**  
*American International University-Bangladesh (AIUB)*  
**Jan 2015 – Apr 2019** &nbsp;|&nbsp; *Dhaka, Bangladesh*

- Core coursework: Object-Oriented Programming, Data Structures & Algorithms, Database Management Systems (DBMS), Operating Systems, Software Engineering & Project Management, Computer Networks, Microprocessors & Embedded Systems.

---

## Verified Professional Profiles & Contact

- **Email:** [ahamed.touker@gmail.com](mailto:ahamed.touker@gmail.com)
- **Phone:** [+880 1794-621250](tel:+8801794621250)
- **Location:** House/Flat #2564, Plot #127/KA, Dakshinkhan, Uttara, Dhaka-1230, Bangladesh
- **LinkedIn:** [linkedin.com/in/toukerahmed](https://www.linkedin.com/in/toukerahmed/)
- **GitHub:** [github.com/toukerahmed](https://github.com/toukerahmed)
- **GitLab:** [gitlab.com/toukerahmed](https://gitlab.com/toukerahmed)
- **Stack Overflow:** [stackoverflow.com/users/16973138/touker-ahmed](https://stackoverflow.com/users/16973138/touker-ahmed)
- **Facebook:** [facebook.com/smtoukerahmed](https://www.facebook.com/smtoukerahmed/)
- **Live Interactive Portfolio:** [https://toukerahmed.github.io/Profile/](https://toukerahmed.github.io/Profile/)
