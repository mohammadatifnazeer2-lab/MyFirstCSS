# Complete Next.js SaaS Dashboard with Tailwind CSS

A practical guide with code examples for styling a Next.js application using Tailwind CSS, including App Router layouts, Server and Client Components, responsive navigation, dashboard UI, authentication screens, loading and error states, not-found pages, and responsive SEO-friendly layouts.

## Tailwind CSS Setup

### `app/globals.css`

Tailwind CSS v4 uses the following import:

```css
@import "tailwindcss";

:root {
  --background: #ffffff;
  --foreground: #171717;
}

body {
  background: var(--background);
  color: var(--foreground);
}
```

Import the stylesheet in your root layout.

## App Router Styling

### `app/layout.js`

The root layout wraps every page in the application.

```jsx
import "./globals.css";
import Navbar from "../components/Navbar";

export const metadata = {
  title: "SaaS Dashboard",
  description: "A responsive dashboard built with Next.js and Tailwind CSS.",
};

export default function RootLayout({ children }) {
  return (
    <html lang="en">
      <body className="min-h-screen bg-gray-50 text-gray-900 antialiased">
        <Navbar />
        <main>{children}</main>
      </body>
    </html>
  );
}
```

## Server Component Styling

Server Components are the default in the App Router. They can use Tailwind classes without the `"use client"` directive.

### `app/page.js`

```jsx
export default function HomePage() {
  return (
    <section className="mx-auto max-w-6xl px-4 py-16 sm:px-6 lg:px-8">
      <div className="rounded-2xl bg-white p-8 shadow-sm sm:p-12">
        <p className="text-sm font-semibold uppercase tracking-wider text-blue-600">
          Next.js + Tailwind CSS
        </p>

        <h1 className="mt-4 text-3xl font-bold tracking-tight sm:text-5xl">
          Build your SaaS dashboard
        </h1>

        <p className="mt-4 max-w-2xl text-gray-600">
          Create modern, responsive user interfaces with reusable components.
        </p>

        <a
          href="/dashboard"
          className="mt-8 inline-block rounded-lg bg-blue-600 px-6 py-3 font-medium text-white hover:bg-blue-700"
        >
          View Dashboard
        </a>
      </div>
    </section>
  );
}
```

## Client Component Styling

Client Components are useful when you need state, event handlers, or browser interactions.

### `components/Counter.jsx`

```jsx
"use client";

import { useState } from "react";

export default function Counter() {
  const [count, setCount] = useState(0);

  return (
    <div className="rounded-xl border bg-white p-6 shadow-sm">
      <h2 className="text-xl font-semibold">Interactive Counter</h2>

      <p className="my-4 text-3xl font-bold text-blue-600">
        {count}
      </p>

      <button
        onClick={() => setCount((value) => value + 1)}
        className="rounded-lg bg-blue-600 px-4 py-2 text-white hover:bg-blue-700"
      >
        Increase
      </button>
    </div>
  );
}
```

Use it in a page:

```jsx
import Counter from "../components/Counter";

export default function CounterPage() {
  return (
    <section className="p-8">
      <Counter />
    </section>
  );
}
```

## Layout Styling

Layouts provide consistent page structure and shared UI.

### `app/dashboard/layout.js`

```jsx
export default function DashboardLayout({ children }) {
  return (
    <div className="min-h-screen bg-gray-100">
      <header className="border-b bg-white px-6 py-4">
        <h1 className="text-xl font-bold">My SaaS Dashboard</h1>
      </header>

      <div className="mx-auto max-w-7xl px-4 py-6 sm:px-6 lg:px-8">
        {children}
      </div>
    </div>
  );
}
```

This layout applies to routes inside `/dashboard`.

## Page Styling

### `app/dashboard/page.js`

```jsx
const stats = [
  { title: "Total Users", value: "1,250" },
  { title: "Revenue", value: "$8,450" },
  { title: "Orders", value: "320" },
  { title: "Growth", value: "12.5%" },
];

export default function DashboardPage() {
  return (
    <section>
      <h2 className="text-2xl font-bold">Dashboard Overview</h2>

      <p className="mt-2 text-gray-600">
        Monitor your application performance.
      </p>

      <div className="mt-6 grid grid-cols-1 gap-4 sm:grid-cols-2 lg:grid-cols-4">
        {stats.map((stat) => (
          <article
            key={stat.title}
            className="rounded-xl border bg-white p-5 shadow-sm"
          >
            <p className="text-sm text-gray-500">{stat.title}</p>
            <p className="mt-2 text-2xl font-bold">{stat.value}</p>
          </article>
        ))}
      </div>
    </section>
  );
}
```

## Responsive Next.js Navbar

### `components/Navbar.jsx`

This component uses Tailwind responsive utilities and React state for the mobile menu.

```jsx
"use client";

import { useState } from "react";
import Link from "next/link";

export default function Navbar() {
  const [menuOpen, setMenuOpen] = useState(false);

  const links = [
    { href: "/", label: "Home" },
    { href: "/dashboard", label: "Dashboard" },
    { href: "/login", label: "Login" },
  ];

  return (
    <nav className="border-b bg-white">
      <div className="mx-auto flex max-w-7xl items-center justify-between px-4 py-4">
        <Link href="/" className="text-xl font-bold text-blue-600">
          SaaS App
        </Link>

        <button
          type="button"
          aria-label="Toggle navigation"
          aria-expanded={menuOpen}
          onClick={() => setMenuOpen((open) => !open)}
          className="rounded-md border px-3 py-2 md:hidden"
        >
          {menuOpen ? "Close" : "Menu"}
        </button>

        <div
          className={`${
            menuOpen ? "flex" : "hidden"
          } absolute left-0 right-0 top-16 z-10 flex-col gap-4 border-b bg-white p-4 md:static md:flex md:flex-row md:items-center md:border-0 md:p-0`}
        >
          {links.map((link) => (
            <Link
              key={link.href}
              href={link.href}
              onClick={() => setMenuOpen(false)}
              className="text-gray-700 hover:text-blue-600"
            >
              {link.label}
            </Link>
          ))}
        </div>
      </div>
    </nav>
  );
}
```

## Dashboard Layout

A responsive dashboard can use a sidebar on desktop and a stacked layout on smaller screens.

### Example dashboard section

```jsx
export default function DashboardSection() {
  return (
    <div className="grid min-h-[70vh] grid-cols-1 md:grid-cols-[220px_1fr]">
      <aside className="bg-gray-900 p-5 text-white">
        <h2 className="mb-6 text-lg font-bold">Workspace</h2>

        <nav className="space-y-3">
          <a href="/dashboard" className="block rounded-lg bg-gray-800 p-3">
            Overview
          </a>
          <a href="/dashboard" className="block rounded-lg p-3 hover:bg-gray-800">
            Analytics
          </a>
          <a href="/dashboard" className="block rounded-lg p-3 hover:bg-gray-800">
            Settings
          </a>
        </nav>
      </aside>

      <main className="p-5 sm:p-8">
        <h1 className="text-3xl font-bold">Welcome Back</h1>
        <p className="mt-2 text-gray-600">
          Here is your workspace overview.
        </p>
      </main>
    </div>
  );
}
```

## Authentication UI

### `app/login/page.js`

This example provides a styled login interface. It is a UI demonstration, not a complete authentication system.

```jsx
export const metadata = {
  title: "Login | SaaS Dashboard",
  description: "Sign in to your SaaS dashboard.",
};

export default function LoginPage() {
  return (
    <main className="flex min-h-[80vh] items-center justify-center px-4 py-12">
      <form className="w-full max-w-md space-y-5 rounded-2xl border bg-white p-8 shadow-sm">
        <div>
          <h1 className="text-2xl font-bold">Welcome Back</h1>
          <p className="mt-2 text-sm text-gray-500">
            Sign in to access your account.
          </p>
        </div>

        <div>
          <label htmlFor="email" className="mb-2 block text-sm font-medium">
            Email Address
          </label>
          <input
            id="email"
            name="email"
            type="email"
            autoComplete="email"
            required
            className="w-full rounded-lg border px-4 py-3 outline-none focus:ring-2 focus:ring-blue-500"
            placeholder="you@example.com"
          />
        </div>

        <div>
          <label htmlFor="password" className="mb-2 block text-sm font-medium">
            Password
          </label>
          <input
            id="password"
            name="password"
            type="password"
            autoComplete="current-password"
            required
            className="w-full rounded-lg border px-4 py-3 outline-none focus:ring-2 focus:ring-blue-500"
            placeholder="Enter your password"
          />
        </div>

        <button
          type="submit"
          className="w-full rounded-lg bg-blue-600 py-3 font-semibold text-white hover:bg-blue-700"
        >
          Sign In
        </button>
      </form>
    </main>
  );
}
```

**Important:** To make authentication work, connect the form to a secure authentication provider or backend. Add server-side validation, secure sessions, and appropriate authorization checks.

## Loading UI

### `app/loading.js`

Next.js automatically displays this UI while a route segment is loading.

```jsx
export default function Loading() {
  return (
    <div
      role="status"
      className="flex min-h-64 flex-col items-center justify-center gap-4"
    >
      <div className="h-10 w-10 animate-spin rounded-full border-4 border-gray-200 border-t-blue-600" />

      <p className="text-gray-600">Loading dashboard...</p>
      <span className="sr-only">Loading</span>
    </div>
  );
}
```

## Error UI

### `app/error.js`

Error boundaries must be Client Components. Next.js displays this UI when a handled error occurs in the route segment.

```jsx
"use client";

export default function Error({ error, reset }) {
  return (
    <div className="flex min-h-64 flex-col items-center justify-center px-4 text-center">
      <h2 className="text-2xl font-bold text-red-600">
        Something went wrong
      </h2>

      <p className="mt-3 text-gray-600">
        We could not load this page. Please try again.
      </p>

      <button
        onClick={() => reset()}
        className="mt-6 rounded-lg bg-blue-600 px-5 py-3 text-white hover:bg-blue-700"
      >
        Try Again
      </button>
    </div>
  );
}
```

## Not-found UI

### `app/not-found.js`

Next.js uses this component for a custom not-found page when the route does not exist or `notFound()` is called.

```jsx
import Link from "next/link";

export default function NotFound() {
  return (
    <main className="flex min-h-[70vh] flex-col items-center justify-center px-4 text-center">
      <p className="text-7xl font-extrabold text-blue-600">404</p>

      <h1 className="mt-4 text-2xl font-bold">
        Page Not Found
      </h1>

      <p className="mt-3 text-gray-600">
        The page you are looking for does not exist.
      </p>

      <Link
        href="/"
        className="mt-6 rounded-lg bg-blue-600 px-5 py-3 text-white hover:bg-blue-700"
      >
        Return Home
      </Link>
    </main>
  );
}
```

## SEO-friendly Responsive Layouts

Next.js supports metadata through the Metadata API.

### `app/layout.js`

Add metadata to improve page titles and descriptions:

```jsx
export const metadata = {
  title: {
    default: "SaaS Dashboard",
    template: "%s | SaaS Dashboard",
  },
  description:
    "A responsive SaaS dashboard built with Next.js and Tailwind CSS.",
  applicationName: "SaaS Dashboard",
};
```

Place this export in the root layout alongside the existing `RootLayout` component. Do not declare a second `metadata` export if one already exists.

### Responsive design example

```jsx
export default function ResponsiveSection() {
  return (
    <section className="mx-auto max-w-7xl px-4 py-12 sm:px-6 lg:px-8">
      <div className="grid grid-cols-1 gap-6 md:grid-cols-2 lg:grid-cols-3">
        <article className="rounded-xl bg-white p-6 shadow-sm">
          <h2 className="text-xl font-bold">Responsive Design</h2>
          <p className="mt-3 text-gray-600">
            Adapt the layout to mobile, tablet, and desktop screens.
          </p>
        </article>

        <article className="rounded-xl bg-white p-6 shadow-sm">
          <h2 className="text-xl font-bold">Reusable Components</h2>
          <p className="mt-3 text-gray-600">
            Build consistent user interfaces from reusable components.
          </p>
        </article>

        <article className="rounded-xl bg-white p-6 shadow-sm">
          <h2 className="text-xl font-bold">SEO Ready</h2>
          <p className="mt-3 text-gray-600">
            Use meaningful page titles, descriptions, and semantic HTML.
          </p>
        </article>
      </div>
    </section>
  );
}
```

Tailwind's responsive prefixes include:

- `sm:` — small screens and larger
- `md:` — medium screens and larger
- `lg:` — large screens and larger
- `xl:` — extra-large screens and larger
- `2xl:` — very large screens and larger
