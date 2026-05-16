# ☕ Java Naming Conventions

A quick reference guide for Java naming conventions following standard Java coding guidelines.

---

## 📦 Packages

| Type | Example | Style |
|------|---------|-------|
| Package | `com.myapp.service` | all lowercase |
| Sub-package | `com.myapp.dto` | all lowercase |

> **Rule:** Always lowercase, separated by dots — never underscores or hyphens.

---

## 🏛️ Classes

| Type | Example | Style |
|------|---------|-------|
| Class | `UserService` | PascalCase |
| Abstract class | `AbstractRepository` | PascalCase |
| Interface | `Serializable` | PascalCase |
| Enum | `DayOfWeek` | PascalCase |
| Record | `UserRecord` | PascalCase |
| Annotation | `@Override` | PascalCase |

> **Rule:** Every class name starts with a capital letter. The `.java` filename must exactly match the public class name inside it.

---

## ⚙️ Methods

| Type | Example | Style |
|------|---------|-------|
| Regular method | `getUserById()` | camelCase |
| Getter | `getName()` | `get` + PascalCase |
| Setter | `setName()` | `set` + PascalCase |
| Boolean getter | `isActive()` | `is` / `has` prefix |
| Factory method | `of()` / `from()` | camelCase |
| Builder method | `withName()` | camelCase |

---

## 🔤 Variables

| Type | Example | Style |
|------|---------|-------|
| Local variable | `userName` | camelCase |
| Instance field | `private int age` | camelCase |
| Static field | `static int count` | camelCase |
| Constant (`static final`) | `MAX_SIZE` | SCREAMING_SNAKE_CASE |
| Enum value | `MONDAY`, `TUESDAY` | SCREAMING_SNAKE_CASE |

> **Rule:** `static final` constants are the **only** case that uses `SCREAMING_SNAKE_CASE`.

---

## 🔠 Generics & Type Parameters

| Type | Example | Style |
|------|---------|-------|
| Generic type | `T` | Single uppercase letter |
| Element type | `E` | Single uppercase letter |
| Key / Value | `K`, `V` | Single uppercase letter |
| Number type | `N` | Single uppercase letter |
| Method parameter | `userId` | camelCase |
| Varargs parameter | `String... args` | camelCase |

---

## 🗂️ Files & Common Suffixes

| Type | Example | Style |
|------|---------|-------|
| Source file | `UserService.java` | Matches class name |
| Test class | `UserServiceTest` | PascalCase + `Test` |
| Exception class | `UserNotFoundException` | PascalCase + `Exception` |
| Utility class | `StringUtils` | PascalCase + `Utils` |
| DAO / Repository | `UserRepository` | PascalCase + `Repository` |
| Service | `PaymentService` | PascalCase + `Service` |
| Controller | `UserController` | PascalCase + `Controller` |
| DTO | `UserDto` | PascalCase + `Dto` |
| Builder | `UserBuilder` | PascalCase + `Builder` |
| Implementation | `UserServiceImpl` | PascalCase + `Impl` |

---

## 🧠 Quick Summary

| Style | Used For |
|-------|----------|
| `PascalCase` | Classes, interfaces, enums, annotations, records |
| `camelCase` | Methods, variables, parameters, instance fields |
| `SCREAMING_SNAKE_CASE` | Constants (`static final`), enum values |
| `lowercase` | Package names only |
| Single letter (`T`, `E`, `K`, `V`) | Generic type parameters |

---

## ✅ Golden Rules

1. **Packages** are always all lowercase with dots — no underscores (`com.company.project`).
2. **Constants** (`static final`) are the only identifiers written in `SCREAMING_SNAKE_CASE`.
3. **File name must match the class name** exactly — `UserService.java` must contain `public class UserService`.
4. **One public class per `.java` file.**
5. **Boolean methods** start with `is` or `has` — never `get` (e.g. `isEnabled()`, not `getEnabled()`).
