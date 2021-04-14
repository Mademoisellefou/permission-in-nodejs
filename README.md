# permission-in-nodejs

## Explained

### 1. User

**app.get("/admin") for access to _adminPage_ it has 2 functions.**

_AuthUser_ if user is null send 403 for else next

_AuthUser_ if check the user role is the same as required

---

- Note

an user is set credentials at first line of code in **setUser** function .
