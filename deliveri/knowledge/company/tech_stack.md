# Deliveri Technology Architecture

Deliveri is built with an **API-first** and **AI-enabled** architecture to ensure scalability and integration with future agentic workflows.

## Technology Stack
- **Backend Framework**: Python + FastAPI.
- **Data Layers**:
    - **Postgres**: Primary transactional database.
    - **DuckDB + Polars**: High-performance data processing and analytics.
    - **Redis/Celery**: Asynchronous task queues for logistics operations.

## Security & Authentication
- **Authentication (AuthN)**: AWS Cognito.
- **Authorization (AuthZ)**: App-level multi-tenant RBAC (Role-Based Access Control).

### Multi-Tenant Model
- Centrally tracked through a `tenant_memberships` table.
- All queries are tenant-scoped for security.
- **Available Roles**:
    - Owner
    - Admin
    - Operator
    - ReadOnly

## AI Strategy
- **Assistive → Autonomous**: Start with AI assisting human operators, then transition to autonomous logistics decisioning.
- **Logistics OS Layer**: Unified control layer for both human operators and AI agents.
- **Model Context Protocol (MCP)**: Support for native AI-driven workflows and tools.
- **Embedded Intelligence**: AI-assisted systems for HS Code lookups, workflow optimization, and routing decisions.

## Infrastructure
- **Cloud Platform**: AWS.
- **Token Security**: API-first with secure token handling (24-hour lifetimes).
