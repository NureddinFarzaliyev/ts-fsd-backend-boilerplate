# Basic Typescript boilerplate for node.js applications

## Folder Structure

All source code is in the `src` folder.
After building, the compiled JavaScript files will be in the `dist` folder.

**`/entities/`**

- Contains database models, validation schemas, and types. Files are grouped by the name of the entity (e.g., `user`).

**`/features/`**

- Contains controllers, services, routers and all other feature-specific logic. Files are grouped by the name of the feature (e.g., `auth`).

**`/shared/`**

- Contains shared logic.

**`/shared/middlewares/`**

- Contains middlewares that can be used in multiple places.

**`/shared/utils/`**

- Contains utility functions that can be used in multiple places.

## Importing Files With Alias

Project is configured to use absolute imports with the `@` alias pointing to the `src` folder.

Insead of writing:

```typescript
import { User } from "../../entities/user";
```

You can write:

```typescript
import { User } from "@/entities/user";
```

## NPM Functions

`npm run dev` - start development server with nodemon

`npm run build` - build the project

`npm run start` - start the project
