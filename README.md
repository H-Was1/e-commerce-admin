# Full Stack E-Commerce + Dashboard & CMS: Next.js 14 App Router, React, Tailwind, Prisma, PostgreSQL, 2024


For DEMO, use [Stripe Testing Cards](https://stripe.com/docs/testing)

This is a repository for a Full Stack E-Commerce + Dashboard & CMS: Next.js 14 App Router, React, Tailwind, Prisma, PostgreSQL

Key Features:

- Shadcn UI for the Admin!
- CMS, Admin and API!
- create, update and delete categories!
- create, update and delete products!
- upload multiple images for products, and change them whenever you want!
- create, update and delete filters such as "Color" and "Size", and then match them in the "Product" creation form.
- create, update and delete "Billboards" which are these big texts on top of the page. attach them to a single category, or use them standalone (Our Admin generates API for all of those cases!)
- Search through all categories, products, sizes, colors, billboards with included pagination!
- control which products are "featured" so they show on the homepage!
- see your orders, sales, etc.
- see graphs of your revenue etc.
- Clerk Authentication!
- Order creation
- Stripe checkout
- Stripe webhooks
- PostgreSQL + Prisma + Neon.Tech

### Prerequisites

**Node version 20.x**

### Cloning the repository

```shell
git clone https://github.com/H-Was1/e-commerce-admin.git
```

### Install packages

```shell
npm i
```

### Setup .env file

```js
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/

# This was inserted by `prisma init`:
# Environment variables declared in this file are automatically made available to Prisma.
# See the documentation for more detail: https://pris.ly/d/prisma-schema#accessing-environment-variables-from-the-schema

# Prisma supports the native connection string format for PostgreSQL, MySQL, SQLite, SQL Server, MongoDB and CockroachDB.
# See the documentation for all the connection string options: https://pris.ly/d/connection-strings

DATABASE_URL=''
NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME=""
STRIPE_API_KEY=
FRONTEND_STORE_URL=http://localhost:3001
STRIPE_WEBHOOK_SECRET=
```

### Connect to Neon.Tech and Push Prisma

```shell
npx prisma generate
npx prisma db push
```

### Start the app

```shell
npm run dev
```

## Available commands

Running commands with npm `npm run [command]`

| command | description                              |
| :------ | :--------------------------------------- |
| `dev`   | Starts a development instance of the app |
