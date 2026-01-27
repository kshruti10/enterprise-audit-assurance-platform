# Backend Architecture

The backend follows **Clean / Layered Architecture** to ensure:
- Separation of concerns
- Scalability
- Maintainability
- Testability

---

## Layers Overview

### API Layer (Audit.API)
- Exposes REST endpoints
- Handles HTTP requests/responses
- Delegates logic to Application layer

### Application Layer (Audit.Application)
- Contains business logic
- Implements use cases
- Uses interfaces for repositories

### Domain Layer (Audit.Domain)
- Core business entities
- Domain rules & enums
- No dependency on frameworks

### Data Layer (Audit.Data)
- Database context
- Entity configurations
- Migrations

### Infrastructure Layer (Audit.Infrastructure)
- Repository implementations
- External service integrations
- Azure Key Vault & logging


Dependencies always point **inward**.

---

## Key Patterns Used
- Repository Pattern
- Dependency Injection
- SOLID Principles
- Separation of Concerns

---

## Dependency Flow

