# Micro SaaS App

This project is a Micro SaaS application built with [Next.js](https://nextjs.org/), a popular React framework for web development. The application allows users to manage tasks (todos) efficiently and intuitively.

## Getting Started

Before you begin, make sure you have [Node.js](https://nodejs.org/) installed on your system. We recommend using the [pnpm](https://pnpm.io/) package manager, but you can also use npm or yarn.

1. Install project dependencies:

   ```bash
   pnpm install
   ```

2. Run the Prisma command to generate data models:

   ```bash
   pnpm prisma generate
   ```

3. Start the development server:

   ```bash
   pnpm dev
   ```

**Note:** Remember to configure the environment variables for MailTrap to enable MagicLink authentication. These variables should include details such as SMTP host, port, username, password, etc., required for sending emails containing magic links for authentication.

After starting the server, open [http://localhost:3000](http://localhost:3000) in your browser to see the result.

You can begin editing the page by modifying `src/app/app/(main)/page.tsx`. The page updates automatically as you edit the file.

## Authentication

Authentication in this application is done via Magic Link. Upon registration or login, users receive an email containing a magic link. Clicking on this link automatically logs them into the application, providing a seamless and secure authentication experience.
