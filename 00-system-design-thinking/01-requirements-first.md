# Requirements First

## Don't draw boxes until you understand the problem.

### 1.The Hook

**Start with something memorable.**
- Establish the philosophy that architecture should not begin with technology.
```text 
The first mistake in system design is drawing the architecture too early.

Before choosing Kafka, Kubernetes, Redis, PostgreSQL, microservices, or an AI model, understand the problem.

A system can be technically sophisticated and still be the wrong system.
```
```text
Business Problem
       ↓
Users
       ↓
Use Cases
       ↓
Requirements
       ↓
Constraints
       ↓
Scale
       ↓
Architecture
```

**Key principle:**

>Architecture is a response to requirements—not a collection of technologies looking for a problem.
---
## 2. Why Requirements Come Before Architecture
### Different requirements can produce completely different architectures.
**For example:**

#### Requirement A

***Internal application used by 100 employees.***

Potential architecture:
```text
Browser
   ↓
Application
   ↓
Database
```
#### Requirement B

***Public platform serving 100 million users globally.***

Now you may need:
```text
Users
 ↓
CDN
 ↓
Global Traffic Management
 ↓
Load Balancers
 ↓
Distributed Services
 ↓
Cache
 ↓
Databases
 ↓
Async Processing
```
The technology isn't the starting point.

The requirements changed the architecture.
### Functional Requirements
> What must the system actually do?

#### Functional requirements describe system behavior.

***For example, an e-commerce system might need to:***

- Create an account
- Search products
- View product details
- Add products to cart
- Place an order
- Process payment
- Reserve inventory
- Send confirmation
- Track order status

You should explain that functional requirements should be expressed as capabilities, not implementation choices.

### Bad

> The system must use Kafka.

That's not a functional requirement.

### Better

> The system must process order events asynchronously.

Kafka may become an architectural decision later.

### Non-Functional Requirements

### Users and Actors

### Core Use Cases

### Business Constraints

### Technical Constraints

### Scale Expectations

### Availability Requirements

### Latency Requirements

### Data Requirements

### Security Requirements

### Compliance Requirements

### Growth Expectations

### Scope Definition

### In Scope
### Out of Scope

### Clarifying Questions

### Turning Requirements Into Engineering Constraints

### Example: URL Shortener

### Example: Notification Platform

### Example: E-Commerce Platform

### Common Mistakes

### Requirements Checklist