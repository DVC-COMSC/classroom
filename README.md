# Classroom Hub

Self-service repo provisioning for your courses — replaces GitHub Classroom.
Two steps, both started from a link on your **Canvas** course page.

## 1. Register (once per term — safe to repeat)

Open the **Register** link from Canvas and fill in:

- **Name** — your full name (First Last)
- **Email** — your school email
- **Code** — the class join code (shown on your Canvas course page)

Your GitHub username is captured automatically. You'll get a confirmation comment.
Made a typo? Just register again — it overwrites.

## 2. Request an assignment repo

Open your course's **Request** link from Canvas → pick the assignment.
You'll get:

- a private repo named `…-<assignment>-<your-username>`
- an **invitation** to accept (link is in the confirmation comment)

Accept the invite, then clone:

```
gh repo clone <owner>/<your-repo>
```

Re-requesting the same assignment is safe — it just returns your existing repo.

---

**Not registered?** A request will be rejected with the Register link — register first
(and wait nothing; it's instant once you use the class code).

**Instructor note:** all course/assignment/semester values live in `config.json`.
The org is auto-detected at runtime (`github.repository_owner`) — this hub is org-neutral.
