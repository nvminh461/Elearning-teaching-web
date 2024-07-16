# Project Structure

This document outlines the directory structure for the `nodejs-typescript` project. The structure is designed to organize the project in a way that separates concerns and enhances maintainability.

## Directory Structure

```plaintext
📦Elearning-teaching-web/
├── 📂dist/
├── 📂src/
│   ├── 📂constants/
│   │   ├── enum.ts
│   │   ├── httpStatus.ts
│   │   └── message.ts
│   ├── 📂controllers/
│   │   └── users.controllers.ts
│   ├── 📂middlewares/
│   │   ├── error.middlewares.ts
│   │   ├── file.middlewares.ts
│   │   ├── users.middlewares.ts
│   │   └── validation.middlewares.ts
│   ├── 📂models/
│   │   ├── 📂database/
│   │   │   ├── Blacklist.ts
│   │   │   ├── Bookmark.ts
│   │   │   ├── Follower.ts
│   │   │   ├── Hashtag.ts
│   │   │   ├── Like.ts
│   │   │   ├── Media.ts
│   │   │   ├── Tweet.ts
│   │   │   └── User.ts
│   │   ├── Error.ts
│   │   └── Success.ts
│   ├── 📂routes/
│   │   └── users.routes.ts
│   ├── 📂services/
│   │   ├── bookmarks.services.ts
│   │   ├── database.services.ts
│   │   ├── followers.services.ts
│   │   ├── hashtags.services.ts
│   │   ├── likes.services.ts
│   │   ├── medias.services.ts
│   │   ├── tweets.services.ts
│   │   └── users.services.ts
│   ├── 📂utils/
│   │   ├── crypto.ts
│   │   ├── email.ts
│   │   ├── file.ts
│   │   ├── helpers.ts
│   │   └── jwt.ts
│   ├── 📜index.ts
│   └── 📜type.d.ts
├── 📜.editorconfig
├── 📜.env
├── 📜.eslintignore
├── 📜.eslintrc
├── 📜.gitignore
├── 📜.prettierignore
├── 📜.prettierrc
├── 📜nodemon.json
├── 📜package.json
├── 📜tsconfig.json
└── 📜yarn.lock
```
## Directory Descriptions

- `dist`: Contains the build files.
- `src`: The source code of the project.
  - `src/constants`: Holds constant values such as enums, HTTP status codes, and messages.
  - `src/controllers`: Contains files that receive requests, call services to process business logic, and return responses.
  - `src/middlewares`: Includes middleware functions for validation, token checking, etc.
  - `src/models`: Contains model files.
  - `src/routes`: Holds the route files.
  - `src/services`: Contains files with methods that interact with the database to process business logic.
  - `src/utils`: Includes utility functions, such as encryption, email sending, file handling, etc.

## Configuration Files

- `.editorconfig`, `.env`, `.eslintignore`, `.eslintrc`, `.gitignore`, `.prettierignore`, `.prettierrc`, `nodemon.json`, `package.json`, `tsconfig.json`, and `yarn.lock` are configuration files for various tools and environments to ensure consistency and proper setup across development environments.
