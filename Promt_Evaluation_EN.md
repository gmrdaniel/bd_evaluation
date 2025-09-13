# Prompt for Comparative Database Analysis of Projects

## Context and Role
Act as an **expert database architecture consultant** and **software project auditor** with specialization in TypeScript and Supabase. Your objective is to perform an exhaustive and comparative analysis of two projects being developed by different teams, based on **database design best practices** and **role and permission systems for scalable applications**.

## Files to Analyze

### Project A
- **Source code path**: `[INSERT_PROJECT_A_CODE_PATH]`
- **ERD diagram path**: `[INSERT_PROJECT_A_ERD_PATH]`
- **Database schema path**: `[INSERT_PROJECT_A_SCHEMA_PATH]`

### Project B
- **Source code path**: `[INSERT_PROJECT_B_CODE_PATH]`
- **ERD diagram path**: `[INSERT_PROJECT_B_ERD_PATH]`
- **Database schema path**: `[INSERT_PROJECT_B_SCHEMA_PATH]`

## Main Objectives

### 1. Comparative Database Analysis
Compare both schemas evaluating:
- **Structure and normalization**
- **Entity relationships**
- **Indexes and optimizations**
- **Scalability and maintainability**
- **Security and access control**

### 2. FOMO Analysis (Fear of Missing Out)
Identify for each project:
- **Critical features missing** compared to the other
- **Functionalities that could compromise project success**
- **Lost opportunities** in current design
- **Technical obsolescence risks**

### 3. Critical Component Evaluation

#### Users, Roles, and Permissions Tables
- **Expandability**: Ability to add new roles without structural modifications
- **Maintainability**: Ease of managing permissions and updates
- **Flexibility**: Support for hierarchical roles and granular permissions
- **Security**: Implementation of least privilege principles

#### Campaign Tables
- **Installability**: Ease of configuration in different environments
- **Functionality**: Feature completeness for campaign management
- **Integrability**: Ability to connect with other modules
- **Performance**: Optimization for frequent operations

## Evaluation Criteria (Best Practices)

### TypeScript Development
- **Strong typing** and interface usage
- **Generics** for code reusability
- **Appropriate decorators** for validation
- **Robust error handling**
- **Design patterns** implementation
- **Testing** and code coverage

### Supabase Implementation
**Evaluation based on best practices for scalable applications:**
- **Row Level Security (RLS)** correctly configured with granular policies
- **Security policies** well-defined for each critical table
- **Real-time subscriptions** optimized and appropriately filtered
- **Database triggers and functions** for business logic
- **Versioned and reversible migrations** with rollback strategy
- **Edge Functions** when appropriate for distributed processing
- **Seamless auth integration** with custom role system
- **Performance monitoring** and query optimization
- **Connection pooling** configured for high concurrency

### Database Architecture
**Analysis based on best practices for scalable applications:**

#### Critical Table Analysis
**Users Table:**
- **Structure and fields**: email, password_hash, created_at, updated_at, status
- **Validations**: email uniqueness, format constraints
- **Security**: password hashing, protected sensitive fields
- **Scalability**: prepared for millions of users

**Roles Table:**
- **Hierarchy**: parent/child role support
- **Flexibility**: dynamic vs static roles
- **Extensibility**: ability to add new roles without schema changes
- **Granularity**: level of detail in role definition

**Permissions Table:**
- **RBAC Model**: Role-Based Access Control correctly implemented
- **Granularity**: resource/action level permissions
- **Inheritance**: permissions inherited from parent roles
- **Expandability**: ease of adding new permissions

**Campaigns Table:**
- **Metadata**: complete configuration information
- **States**: well-defined state workflow
- **Relational**: connections with users, roles, and permissions
- **Performance**: optimized for frequent queries

#### Row Level Security (RLS) - Detailed Analysis
**RLS Implementation:**
- **Defined policies**: access policies per table
- **Granularity**: row-level control based on user context
- **Performance**: impact on query performance
- **Maintainability**: ease of managing and updating policies
- **Testing**: test coverage for different access scenarios
- **Debugging**: ability to troubleshoot complex policies

**RLS Best Practices Evaluated:**
- Policies by role/user context
- Efficient use of `auth.uid()` and `auth.jwt()`
- Combination with application-level security
- Policies for specific CRUD operations
- Exception handling and edge cases

#### Design Principles Evaluated
- **Appropriate normalization** (3NF minimum, BCNF when applicable)
- **Strategic indexes** for frequent queries
- **Constraints** and database-level validations
- **Auditing** and change logging (created_at, updated_at, deleted_at)
- **Soft deletes** vs hard deletes by use case
- **Partitioning** for large tables (users, logs, metrics)
- **Triggers** for process automation
- **Views** for complex query simplification

#### SWOT Analysis by Project
**Strengths - Weaknesses - Opportunities - Threats:**

**Project A:**
- **Strengths**: [Outstanding technical elements]
- **Weaknesses**: [Identified architectural limitations]
- **Opportunities**: [Improvement and growth
