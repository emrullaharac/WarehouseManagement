# 📦 Warehouse Management  

Live Demo: [https://warehousemanagement-3num.onrender.com/](https://warehousemanagement-3num.onrender.com/)

Our warehouse management app is the perfect solution to organize your inventory and keep an overview of your stock.  
With this user-friendly application, you can effortlessly record, manage, and organize all your goods.  
Maintain a structured and well-organized warehouse – with ease.

---

## 👨‍💻 Team  
- Daniel Töpel  
- Deniz Altun  
- Emrullah Arac  

---

## 🚀 Technologies  

**Backend**  
- Spring Boot  
- MongoDB  

**Frontend**  
- React (TypeScript, Vite)  

**CI/CD & Code Quality**  
- GitHub Actions (build & test)  
- SonarQube (code quality checks)  
- Docker (containerization)  
- Render (deployment)  

---

## 📂 Project Structure  

**Backend (Spring Boot)**  
- `controller` – REST endpoints (`/api/products`)  
- `service` – business logic  
- `repository` – MongoDB data access  
- `model` – domain & DTOs  
- `exceptions` – global error handling  

**Frontend (React + Vite + TS)**  
- `components` – UI components (AddProduct, Home, ProductDetailsCard …)  
- `service` – API client  
- `types` – TypeScript models  

---

## ⚡ Features  

- List all products with search  
- Add new product (form)  
- **Edit product with prefilled form**  
- Show product details (with created/updated timestamps)  
- Delete product (with confirmation)  
- Responsive UI  

---

## 🔗 API Endpoints  

| Method | Endpoint              | Description              |
|--------|----------------------|--------------------------|
| GET    | `/api/products`       | Get all products         |
| GET    | `/api/products/{id}`  | Get product by ID        |
| POST   | `/api/products/add`   | Add new product          |
| PUT    | `/api/products/{id}`  | **Update product**       |
| DELETE | `/api/products/{id}`  | Delete product           |

---

## 🛠️ Development & Setup  

**Backend**  
```bash
# run mongodb via docker
docker run -d -p 27017:27017 --name mongo mongo

# build & run spring boot app
mvn clean install
mvn spring-boot:run
```

**Frontend**  
```bash
cd frontend
npm install
npm run dev
```

---

## ✅ CI/CD Flow  

1. Developer opens a Pull Request  
2. GitHub Actions run unit tests & SonarQube checks  
3. At least **1 reviewer approval** required  
4. On merge → Docker image build & push  
5. Deployment to Render  

---

## 📜 License  

MIT License  
