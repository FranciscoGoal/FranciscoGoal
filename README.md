# Francisco González Álvarez

**Software Developer** · Java & Spring Boot · Abu Dhabi, UAE

I build backend services in Java and Spring Boot: REST APIs, authentication and the data models behind them. I'm currently developing **[Crewmoor](https://www.crewmoor.com/)**, a product that helps teams coordinate tasks and day-to-day operations. I'm drawn to software that replaces scattered messages and spreadsheets with one clear, shared view of the work.

[LinkedIn](https://www.linkedin.com/in/francisco-augusto-gonz%C3%A1lez-%C3%A1lvarez-0666893b8) · [crewmoor.com](https://www.crewmoor.com/) · Open to junior backend roles and internships

---

## About

Most of my work is on the server side. I model a domain, expose it through a REST API and secure it with Spring Security. My public repositories show how that has progressed, from a first Spring Boot CRUD service to a stateless JWT authentication API with role-based access control.

I document each project so it can be run and reviewed without asking me questions: setup steps, configuration, endpoints and known limitations.

I'm studying for the Higher Vocational Diploma in Multiplatform Application Development (DAM). My current focus is automated testing with JUnit 5 and real-time messaging with WebSocket/STOMP.

## Stack

<p>
  <img src="https://skillicons.dev/icons?i=java,spring,mysql,maven,docker,git,githubactions" alt="Java, Spring, MySQL, Maven, Docker, Git and GitHub Actions" height="40" />
</p>

**Languages:** Java · SQL · HTML, CSS and JavaScript for simple front ends  
**Backend:** Spring Boot · Spring Security · Spring Data JPA / Hibernate · JWT · REST APIs  
**Databases:** MySQL  
**Tooling:** Maven · Git & GitHub · GitHub Actions · Docker

## Featured projects

### Crewmoor

`In development` · Independent product · [Website](https://www.crewmoor.com/) · [Interactive prototype](https://demo.crewmoor.com/) · [Showcase repository](https://github.com/FranciscoGoal/crewmoor-showcase)

A workspace where a team assigns work, follows its progress step by step and discusses it in context.

- **Interactive prototype** covering teams, task assignment with checklists, an operations dashboard, an activity timeline, a calendar, per-task chat and report exports (PDF, Excel, CSV). It runs on sample data.
- **Backend in early development** with Java and Spring Boot. So far it has a task domain model with enforced status transitions, JWT authentication and a WebSocket messaging foundation, covered by unit tests and CI. The source code is private.
- **Not yet a production service.** The prototype is not connected to the backend, and there are no live customer workspaces.

<a href="https://demo.crewmoor.com/">
  <img src="https://raw.githubusercontent.com/FranciscoGoal/crewmoor-showcase/main/assets/screenshots/operations-dashboard.webp" alt="Crewmoor prototype: operations dashboard with task status, progress by assignee and recent activity (sample data)" width="100%" />
</a>

### Spring Security JWT Auth API

[Repository](https://github.com/FranciscoGoal/spring-security-jwt-auth-api) · Java 21 · Spring Boot 4 · Spring Security · Spring Data JPA · MySQL

A stateless authentication service for registration, login, signed JWT access tokens and role-based authorization.

- Validates tokens with Spring Security's OAuth2 Resource Server (HS256) instead of a hand-written filter.
- Maps roles from a `roles` claim to Spring Security authorities. `/admin/**` requires `ROLE_ADMIN`.
- Stores users and roles in a many-to-many MySQL schema and hashes passwords with a delegating encoder (bcrypt).
- Documents the architecture, the registration and login flows and the data model with diagrams.

### Task Manager

[Repository](https://github.com/FranciscoGoal/Task-Manager) · Java 25 · Spring Boot 4 · Spring Security · jjwt · MySQL · Docker

My first Spring Boot project: a task API with JWT login and a small vanilla-JS web interface.

- Create, read, update and delete tasks, with a `/task/my` endpoint that returns only the authenticated user's tasks.
- Implements a custom `OncePerRequestFilter` that validates JWTs with jjwt.
- Migrated from in-memory H2 to MySQL. Includes a multi-stage Dockerfile and a GitHub Actions build that runs against a MySQL service container.
- Known limitations, such as missing per-task ownership checks, are listed in the README.

## Contact

- **LinkedIn:** [Francisco Augusto González Álvarez](https://www.linkedin.com/in/francisco-augusto-gonz%C3%A1lez-%C3%A1lvarez-0666893b8)
- **GitHub:** [@FranciscoGoal](https://github.com/FranciscoGoal)
- **Crewmoor:** [crewmoor.com](https://www.crewmoor.com/) · [Prototype](https://demo.crewmoor.com/)
