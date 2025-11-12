# WaveUp Backend (MVP)

**WaveUp** is a social network (MVP) where users can register and create posts.
This version currently includes basic authentication and CRUD functionality for posts.

## Stack

* Nest.js
* TypeScript
* TypeORM
* PostgreSQL
* class-validator / class-transformer
* JWT / bcrypt
* ESLint + Prettier + simple-import-sort

## Setup Instructions

1. **Clone the repository**

```bash
git clone <REPO_URL>
cd waveup-backend
```

2. **Install dependencies**

```bash
npm install
```

3. **Configure environment variables**

* Create a `.env` file based on `.env.example`
* Set your PostgreSQL credentials and JWT secret

4. **Run locally**

```bash
npm run start:dev
```

5. **Linting and formatting**

```bash
npm run lint        # Check code for issues
npm run lint:fix    # Auto-fix linting issues
npm run format      # Format code with Prettier
```

## Project Structure

```
src/
 ├── modules/
 │    ├── auth/      # Register, Login
 │    ├── posts/     # CRUD for posts
 │    └── users/     # User entity and logic
 ├── database/       # TypeORM configuration and PostgreSQL connection
 ├── config/         # Environment variables
 └── common/         # Decorators, filters, pipes, shared utilities
```

## Modules

* `AuthModule` — User registration and login
* `PostsModule` — Create, read, update, delete posts
* `UsersModule` — User logic, relations to posts

## License

MIT License
