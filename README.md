# permission-in-nodejs

## Explained

### 1. User

**app.get("/admin") for access to _adminPage_ it has 2 functions.**

_AuthUser_ if user is null send 403 for else next

_AuthRole_ checks if the user role is the same as required

---

- Note

> An user is set credentials at first line of code in **setUser** function .

---

### 2. Project

**app.get("/projects") for access to a _Project_ it has 2 routes .**

- /:projectId

  - _SetProject_ search the project by id of a project .

  - _AuthUser_ Part1.

  - _AuthGetProject_ you **canviewtheProject** if projectId and userId are same .

- /

  - _scopedProject_ checks if user role is the same as ROLE.ADMIN

---

- Note

> Also you _canDeleteProject_ by the function which compares the id of both .

---
