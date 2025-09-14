# Design Patterns in Node.js – Simple Guide with Real Life Examples

Design patterns are like **recipes** or **blueprints**.  
They aren’t strict code, but proven solutions for common software problems.  
Below are some popular patterns explained simply with real-life analogies.

---

## 1. Singleton Pattern
**What it does:**  
Ensures only one instance of a class/object exists and everyone uses the same one.

**Real Life Example:**  
A **family car** – there’s only one car, and all family members share it.

---

## 2. Factory Pattern
**What it does:**  
Creates objects without exposing the creation logic. You just ask, and it delivers.

**Real Life Example:**  
A **restaurant kitchen** – you order pizza or burger, and the kitchen (factory) prepares it.  
You don’t need to know the recipe.

---

## 3. Observer Pattern
**What it does:**  
When one object changes, it notifies all other subscribed objects.

**Real Life Example:**  
A **school principal’s announcement** – when the principal sends a notice, all teachers and students get it.

---

## 4. Middleware Pattern
**What it does:**  
A chain of functions where each processes something and then passes control to the next.

**Real Life Example:**  
**Airport security checks** – baggage scan → ID check → body scan.  
Each step does its job, then forwards you.

---

## 5. Module Pattern
**What it does:**  
Encapsulates related code into modules and exposes only what’s needed.

**Real Life Example:**  
**Company departments** – HR handles hiring, Payroll handles salaries.  
You don’t need to know internal details, just the service they provide.

---

## 6. Decorator Pattern
**What it does:**  
Adds extra functionality to an object without changing its original structure.

**Real Life Example:**  
**Coffee order** – you start with plain coffee, then add milk, sugar, or cream.  
The base coffee remains the same, you just decorate it.

---

## 7. Dependency Injection Pattern
**What it does:**  
Instead of a class creating its own dependencies, they are passed (injected) from outside.

**Real Life Example:**  
A **contractor building a house** – you provide the tools.  
If better tools come tomorrow, you can swap them without changing the contractor.

---

## 8. Promise Pattern
**What it does:**  
Represents a value that will be available in the future (async handling).

**Real Life Example:**  
**Online shopping** – you place an order and get a tracking link (promise).  
Later, you either receive the package (resolve) or the order fails (reject).

---

## Summary
- **Singleton** → One shared instance (family car)  
- **Factory** → Simplified creation (restaurant kitchen)  
- **Observer** → Notify all subscribers (school notice)  
- **Middleware** → Step-by-step pipeline (airport security)  
- **Module** → Encapsulation (company departments)  
- **Decorator** → Add features dynamically (coffee toppings)  
- **Dependency Injection** → External resources provided (contractor’s tools)  
- **Promise** → Future result (online shopping)

---

<!-- for ref -->
<!-- https://medium.com/@techsuneel99/design-patterns-in-node-js-31211904903e -->