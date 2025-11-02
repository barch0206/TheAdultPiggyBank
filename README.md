
# The Adult Piggy Bank

**Adult Piggy Bank** is a smart personal finance web app that helps users analyze their spending, plan savings goals, and make informed money decisions without storing personal data.
Built using a modern microservice architecture — it’s fast, modular, and scalable.

---

## 🏗️ Architecture Overview

```

React Frontend  →  Node.js API Gateway  →  Spring Boot Microservices

```

**Frontend (React)**  
- User-facing web interface  
- Collects financial inputs and shows visual analytics  
- Calls the Node.js backend via REST APIs  

**Backend (Node.js)**  
- Acts as a middleware / API gateway  
- Handles request validation, routing, and user session management  
- Communicates securely with Spring Boot microservices  

**Microservices (Spring Boot)**  
- Each financial calculator or module (e.g., affordability, emergency fund, debt payoff) is an independent service  
- Exposes REST endpoints used by the Node backend  
- Deployed independently for better scalability and fault isolation  

**Deployment**  
- All services hosted on **Render** with environment-based configuration  
- Uses HTTPS for secure data communication  

---

## 🧠 Tech Stack

| Layer | Technology |
|-------|-------------|
| Frontend | React.js, Tailwind CSS |
| API Gateway | Node.js, Express |
| Microservices | Spring Boot (Java) |
| Hosting | Render Cloud |
| Version Control | GitHub |

---

## 📁 Project Structure

```

adult-piggy-bank/
│
├── frontend/                 # React app (UI components & pages)
│   ├── src/
│   ├── public/
│   └── package.json
│
├── backend-node/             # Node.js API Gateway
│   ├── src/
│   └── package.json
│
└── backend-spring/           # Spring Boot microservices
├── affordability-service/
├── lifestyle-burn-service/
├── impulse-check-service/
└── ...

````

---

## 📸 Screenshots
<img width="903" height="432" alt="apb1" src="https://github.com/user-attachments/assets/00fb67da-d6b2-43d5-8da7-11e362b6a3bb" />
<img width="947" height="428" alt="apb2" src="https://github.com/user-attachments/assets/81f17153-ac4c-43bf-b574-253a283c1e68" />
<img width="948" height="441" alt="apb3" src="https://github.com/user-attachments/assets/79c936d2-8a61-4541-b82d-4b5c719cd05d" />
<img width="913" height="429" alt="apb4" src="https://github.com/user-attachments/assets/ccccf99f-cbe9-4e97-b152-6eea147f2567" />
<img width="893" height="434" alt="apb5" src="https://github.com/user-attachments/assets/62beabbd-a840-4da1-8255-c00ad30baa87" />
<img width="635" height="437" alt="apb" src="https://github.com/user-attachments/assets/12e22719-4491-466d-bfd6-175d96fae7ce" />
<img width="632" height="433" alt="apb6" src="https://github.com/user-attachments/assets/0b5a670f-ce7b-4c16-9f4c-eb864b21f381" />

---

## 💡 Future Enhancements

* User authentication & role-based dashboards
* Expense categorization via OCR or bank statement upload
* PWA (Progressive Web App) support for mobile

---
