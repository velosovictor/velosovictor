<div align="center">

# 🚀 RationalBloks

### Backend-as-a-Service for Modern Applications

**Upload a JSON schema. Get a production API in 2 minutes.**

[![Website](https://img.shields.io/badge/🌐_Try_It_Free-rationalbloks.com-blue?style=for-the-badge)](https://rationalbloks.com)

---

</div>

## The Problem

Every time you build an app, you spend weeks on the same things:
- Writing database models
- Building CRUD endpoints  
- Setting up authentication
- Configuring deployments
- Managing migrations

**I built RationalBloks to eliminate all of that.**

---

## How It Works

```
📝 Define          →    ⚙️ We Generate           →    🚀 You Ship
Your JSON Schema        Complete FastAPI App          Production API
```

<table>
<tr>
<td width="50%">

**You write this:**

```json
{
  "products": {
    "name": { "type": "string" },
    "price": { "type": "decimal" },
    "stock": { "type": "integer" }
  },
  "orders": {
    "user_id": { "foreign_key": "app_users.id" },
    "total": { "type": "decimal" },
    "status": { "type": "string" }
  }
}
```

</td>
<td width="50%">

**You get this:**

```
✅ FastAPI application generated
✅ SQLAlchemy models created
✅ PostgreSQL database provisioned
✅ Alembic migrations applied
✅ JWT authentication integrated
✅ REST API endpoints ready
✅ Deployed to Kubernetes
✅ SSL certificates configured
```

</td>
</tr>
</table>

---

## What's Included

| Feature | Description |
|---------|-------------|
| **🔧 Code Generation** | Complete FastAPI + SQLAlchemy codebase from your schema |
| **🗄️ Database** | PostgreSQL with automatic migrations when you update schema |
| **🔐 Authentication** | JWT tokens, Google OAuth, password hashing—all built-in |
| **🚀 Deployment** | Kubernetes with auto-scaling, health checks, zero-downtime |
| **📊 Dashboard** | Monitor your API performance and usage in real-time |

---

## Try It

<div align="center">

### **[rationalbloks.com](https://rationalbloks.com)**

*Define your data. We handle the rest.*

---

Built by **Victor Veloso**

</div>
