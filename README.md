# CRMS Backend

Spring Boot REST API for the Campus Recruitment Management System.

## Run locally

Requirements: Java 21, MySQL 8+, and Maven 3.9+ (or the included Maven
wrapper).

```powershell
Copy-Item .env.example .env
.\mvnw.cmd spring-boot:run
```

Configure the database, JWT, frontend origin, and bootstrap administrator in
`.env`. Import `../database/schema.sql` before first use when working from the
monorepo. The API listens at `http://localhost:8080`.

When this directory is published as its own repository, copy the `database/`
folder or keep the schema in a separate database/documentation repository and
update the setup reference accordingly.

This directory can be pushed as its own GitHub repository. Commit
`.env.example`, `pom.xml`, and the Maven wrapper; do not commit `.env`,
`uploads/`, or `target/`.
