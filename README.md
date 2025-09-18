#  Online Ordering & Integration System

##  Project Background
During Taiwan’s labor shortage in the service industry, many restaurants faced severe staffing challenges, creating high demand for **self-service ordering and payment systems**.  
However, most commercial solutions at the time adopted a **high-cost leasing model** (tens of thousands of NT dollars annually), while systems were isolated and **unable to integrate operations across multiple restaurants**.  

These “flashy but impractical” systems increased expenses without truly reducing labor or operational pressure.  

---

##  Project Overview
This project was developed with **PHP, MySQL, MongoDB, and JavaScript**, integrated with **Google Maps API, Taiwan Pay, and ENIVTurnkey (Taiwan Ministry of Finance e-Invoice Transmission Software)**.  
The goal was to create a **cost-effective and integrated online ordering system** that reduces reliance on manpower while providing a unified management platform for multiple restaurants.  

The system includes **User Module, Vendor Module, and Backend Management Module**, supporting multi-store operations and real-time data flow.  


#### EINVTurnkey
EINVTurnkey is the **official e-Invoice transmission software provided by Taiwan’s Ministry of Finance (MOF)**.  
It ensures secure and standardized electronic invoice submission, making the system compliant with Taiwan’s taxation and e-invoice regulations.
---

##  System Modules

### 1. Login & Registration
- **JavaScript-based switching** between **User Mode** and **Vendor Mode**.  
- **Separate MySQL tables** for users and vendors.  
- Supports account registration, login, and permission management.  

<img width="525" height="253" alt="image" src="https://github.com/user-attachments/assets/9382003b-5b4e-4a77-8b07-f54ebded0d72" />

---

### 2. Ordering Homepage
- **Google Maps API integration**: Displays store distance from the user’s location.  
- **One-click navigation**: Directly redirects to Google Maps for route planning.  

<p align="center"><img width="508" height="244" alt="image" src="https://github.com/user-attachments/assets/af2c6cc3-566e-4365-8757-3666c3afd9ac" />
</p>
---

### 3. Store Product Page
- One of the most complex parts, with **1,000+ lines of code**.  
- **Multi-layer options**: e.g., drinks require choices for sugar, ice, and size, with all possible combinations supported.  
- **Relational database design**: Ensures product, options, pricing, and inventory remain consistent and flexible.  


<p align="center"><img width="528" height="255" alt="image" src="https://github.com/user-attachments/assets/95fdbcef-2663-44e2-86bb-031aea45bf95" />
</p>
---

### 4. Checkout & Payment
- **Order modes**: Dine-in, takeaway, or reservation (with time setting).  
- **Payment**: Integrated with **Taiwan Pay** for secure transfers.  


<p align="center"><img width="496" height="238" alt="image" src="https://github.com/user-attachments/assets/3bbc11c7-d43a-4a07-ae34-2dc2fbc63b8c" />
</p>
---

### 5. Store Management (Vendor Side)
- **Multi-store management**: A single vendor can register and manage multiple branches.  
- **Unified Business Number validation**: Vendors must provide company ID to comply with regulations.  


<p align="center"><img width="518" height="249" alt="image" src="https://github.com/user-attachments/assets/90af8644-b559-4cf6-86e7-f932ff2a0684" />
</p>
---

### 6. Backend Order System
- **Real-time notifications**: Implemented with **Ajax** to instantly push orders to vendors.  
- **Future plan**: Replace Ajax with **WebSocket** for improved real-time performance.  


<p align="center"><img width="527" height="253" alt="image" src="https://github.com/user-attachments/assets/fdfd8801-2f55-467e-9803-9e7128f4ae13" />
</p>
---

### 7. Backend Revenue System
- **Revenue analysis**: Tracks completed orders and displays revenue and item counts by date/time.  
- **Data visualization**: Provides graphical reports for quick insights.  


<p align="center"><img width="518" height="249" alt="image" src="https://github.com/user-attachments/assets/dbc1d983-f0ca-47ff-8279-12316a59eec1" />
</p>
---

## ⚙️ Technical Highlights
- **Backend**: PHP + MySQL  
- **Frontend**: JavaScript + Ajax + Google Maps API  
- **Payment Integration**: Taiwan Pay  
- **E-Invoice Integration**: EINV Turnkey (Taiwan MOF e-Invoice system)  
- **Real-time**: Currently Ajax-based, with WebSocket planned for future upgrades  

---

## 🚀 Results
- Successfully piloted in **three restaurants** with positive feedback.  
- Reduced manpower burden and offered a **lower-cost alternative** to existing leasing models.  
- Although the project was paused due to academic workload, it provided **valuable hands-on experience in system integration and practical deployment**.  
