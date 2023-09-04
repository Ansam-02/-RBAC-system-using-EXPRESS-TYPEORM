# RBAC System using Express & Typeorm

This is a simple Express.js and TypeORM-based User Management API. It allows you to create, update, retrieve, and delete user records in a MySQL database.

## Prerequisites

Before you begin, ensure you have met the following requirements:

- Node.js and npm installed
- MySQL database server installed and running
- TypeScript installed (you can install it globally using `npm install -g typescript`)

## Getting Started

1. Install Dependencies
```bash
  npm install express typeorm mysql2 reflect-metadata uuid
  npm install --save-dev @types/express @types/node @types/uuid ts-node typescript nodemon concurrently
```
2. Configure Database
create app-data-source.ts where we set up initial database connection options:
```ts
import { DataSource } from "typeorm"

const myDataSource = new DataSource({
    type: "mysql",
    host: "localhost",
    port: 3000,
    username: "test",
    password: "test",
    database: "test",
    entities: ["src/entity/*.js"],
    logging: true,
    synchronize: true,
})
```
3. Create a user.entity.ts entity 
4. establish database connection and start using myDataSource
5. 




