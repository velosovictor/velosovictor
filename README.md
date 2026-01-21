<div align="center">

# RationalBloks

### The Industrial Powerhouse of Backend Infrastructure

</div>

## How It Works

### Step 1: Define Your Data Model

Write a simple JSON schema describing your tables and fields:

```json
{
  "products": {
    "name": { "type": "string", "required": true },
    "price": { "type": "decimal", "required": true },
    "stock": { "type": "integer", "default": 0 },
    "is_active": { "type": "boolean", "default": true }
  },
  "orders": {
    "user_id": { "type": "uuid", "foreign_key": "app_users.id" },
    "product_id": { "type": "uuid", "foreign_key": "products.id" },
    "quantity": { "type": "integer", "required": true },
    "total": { "type": "decimal", "required": true },
    "status": { "type": "string", "default": "pending" }
  }
}
```

### Step 2: We Generate & Deploy Everything

Upload your schema and we automatically:

| What We Generate | Description |
|------------------|-------------|
| ✅ **FastAPI Application** | Complete Python backend with all CRUD endpoints |
| ✅ **SQLAlchemy Models** | Database models with relationships and constraints |
| ✅ **PostgreSQL Database** | Production database provisioned and configured |
| ✅ **Alembic Migrations** | Schema changes automatically generate migrations |
| ✅ **JWT Authentication** | Login, register, password reset, Google OAuth |
| ✅ **FK-Based Authorization** | Add `user_id → app_users.id` and users only access their own data |
| ✅ **Docker Image** | Containerized and pushed to registry |
| ✅ **Kubernetes Deployment** | Deployed with auto-scaling and health checks |
| ✅ **SSL Certificates** | HTTPS configured automatically |

### Step 3: Your Production API is Live

Your API is ready to use immediately:

```
🟢 POST   https://yourapp.rationalbloks.com/api/products      → Create
🟢 GET    https://yourapp.rationalbloks.com/api/products      → List all
🟢 GET    https://yourapp.rationalbloks.com/api/products/{id} → Get one
🟢 PUT    https://yourapp.rationalbloks.com/api/products/{id} → Update
🟢 DELETE https://yourapp.rationalbloks.com/api/products/{id} → Delete
```

Plus full Swagger/OpenAPI documentation at `/docs`.

---

## 🛠️ Complete Feature Set

### 🔧 Code Generation Engine
- Complete FastAPI applications generated from JSON schemas
- SQLAlchemy ORM models with proper relationships
- Pydantic validation for all request/response models
- Automatic CRUD endpoints for every table
- OpenAPI/Swagger documentation generated automatically

### 🗄️ Database & Migrations
- PostgreSQL database provisioned automatically
- Alembic migrations generated when you update your schema
- Foreign key relationships handled automatically
- Indexes and constraints applied from schema
- Zero manual SQL required

### 🔐 Authentication & Authorization
- JWT token-based authentication built into every API
- Google OAuth integration ready to use
- Secure password hashing with bcrypt
- **FK-based authorization**: add `foreign_key: "app_users.id"` to any field and users automatically only access their own records
- Multiple user FKs generate OR-based access (e.g., sender OR receiver can see a message)

### 🚀 Production Infrastructure
- Kubernetes deployment with auto-scaling
- Health checks and automatic restarts
- Zero-downtime deployments
- SSL/HTTPS certificates configured automatically
- Staging and production environments

### 📊 Dashboard & Monitoring
- Real-time API performance metrics
- Request/response logging
- Error tracking and alerts
- Usage analytics per endpoint
- System health monitoring

<br />

---

<div align="center">

## 🎯 Ready to Ship Your Backend in 2 Minutes?

**Stop writing boilerplate. Start building your product.**

[<img src="https://img.shields.io/badge/🚀%20GET%20STARTED%20FREE-rationalbloks.com-1e40af?style=for-the-badge" />](https://rationalbloks.com)

---

**Built with precision by Victor Veloso**

</div>






