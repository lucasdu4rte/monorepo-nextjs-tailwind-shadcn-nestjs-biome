# Full Stack Monorepo with Turbopack, Biome, Next.js, Nest.js, Tailwind CSS, and shadcn

This repository is a full-stack monorepo starter template that integrates several modern web development tools and libraries, including **Turbopack**, **Biome**, **Next.js**, **Nest.js**, **Tailwind CSS**, and **shadcn**. It follows the tutorial from [The Halftime Code](https://www.thehalftimecode.com/building-a-full-stack-monorepo-with-turbopack-biome-next-js-nest-js-tailwind-css-and-shadcn/) on how to set up a full-stack monorepo, combining both frontend and backend services in a single codebase.

## Features

- **Monorepo Architecture**: Organizes both frontend (Next.js) and backend (Nest.js) in a single repository using Turbopack to manage and optimize builds.
- **Next.js**: A powerful React framework for building server-rendered web applications with API routes.
- **Nest.js**: A minimalist Node.js framework for building backend services and REST APIs.
- **Turbopack**: A fast incremental bundler and build system, ideal for monorepo setups.
- **Tailwind CSS**: A utility-first CSS framework for building responsive, modern UI components.
- **shadcn**: A component library that integrates seamlessly with Tailwind CSS, providing elegant UI components.
- **Biome**: A fast and versatile tool for linting, formatting, and ensuring code quality across the entire monorepo.

## Project Structure

The monorepo is organized as follows:

```
/apps
  /web (Next.js)
  /api (Nest.js)

/packages
  /tsconfig (Shared configuration files such as Biome, Tailwind, and Turbopack)
  /types (Shared types)
  /ui (Shared UI components and styles using shadcn component library with TailwindCSS)
  /utils (Shared util methods)
```

- **/apps/web**: Contains the Next.js application responsible for the frontend.
- **/apps/api**: Contains the Nest.js application responsible for the backend.
- **/packages/tsconfig**: Contains shared configurations (e.g., Biome, Tailwind, Turbopack) to enforce consistency across the monorepo.
- **/packages/types**: Contains shared types (e.g. responses, api clients, etc).
- **/packages/ui**: Houses the shared UI components built with shadcn and Tailwind CSS.
- **/packages/utils**: Contains shared utils methods that will be used in multiple apps or packages.

## Getting Started

1. **Clone the repository**

   ```bash
   git clone https://github.com/ivesfurtado/next-nest-biome-turborepo.git
   cd next-nest-biome-turborepo
   ```

2. **Install Dependencies**

   Use `pnpm` package manager:

   ```bash
   pnpm install
   ```

3. **Run the Development Server**

   You can start both the web and api services with Turbopack's parallelism:

   ```bash
   pnpm dev
   ```

   - Frontend is served at `http://localhost:3000` (Next.js)
   - Backend is served at `http://localhost:3001` (Nest.js)

4. **Build for Production**

   > TODO

## Tools and Technologies

- **Next.js**: Provides the frontend framework with server-side rendering, API routes, and static generation.
- **Nest.js**: Handles the backend, including API endpoints and server logic.
- **Turbopack**: Ensures fast builds and optimal performance for monorepos.
- **Tailwind CSS**: Simplifies styling with a utility-first approach.
- **shadcn**: Offers pre-designed components for building clean and modern UIs.
- **Biome**: Enforces code standards by handling linting and formatting across the project.

## Deployment

You can deploy your full-stack monorepo using platforms like Vercel for the frontend and any Node.js hosting service for the backend (e.g., Heroku, AWS, DigitalOcean).

## Contributing

Contributions are welcome! Please open an issue or submit a pull request if you have suggestions or improvements.

## License

This project is licensed under the MIT License. Feel free to use and modify it according to your needs.

---

For further details on building and setting up this monorepo, check out the original tutorial on [The Halftime Code](https://www.thehalftimecode.com/building-a-full-stack-monorepo-with-turbopack-biome-next-js-nest-js-tailwind-css-and-shadcn/).