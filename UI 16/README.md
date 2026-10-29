## NAVBAR
```
<header class="sticky top-0 z-50 border-b bg-white shadow-sm">
  <nav class="mx-auto flex max-w-7xl items-center justify-between px-5 py-4">

    <a href="#home" class="text-2xl font-extrabold text-indigo-600">
      CloudFlow
    </a>

    <div class="hidden items-center gap-6 md:flex">
      <a href="#home" class="hover:text-indigo-600">Home</a>
      <a href="#features" class="hover:text-indigo-600">Features</a>
      <a href="#pricing" class="hover:text-indigo-600">Pricing</a>

      <!-- Mega menu trigger -->
      <button onclick="toggleMegaMenu()" class="hover:text-indigo-600">
        Solutions ▾
      </button>

      <a href="#dashboard" class="hover:text-indigo-600">Dashboard</a>
      <a href="#login" class="hover:text-indigo-600">Login</a>

      <a href="#signup"
         class="rounded-lg bg-indigo-600 px-5 py-2.5 text-white hover:bg-indigo-700">
        Get Started
      </a>
    </div>

    <button onclick="toggleMobileMenu()"
            class="rounded-lg border px-3 py-2 md:hidden"
            aria-label="Toggle navigation">
      ☰
    </button>
  </nav>
```

  ## MEGA MENU
  ```
  <div id="megaMenu" class="hidden border-t bg-white">
    <div class="mx-auto grid max-w-7xl gap-6 px-5 py-8 sm:grid-cols-2 lg:grid-cols-4">

      <a href="#features" class="rounded-xl p-4 hover:bg-indigo-50">
        <h3 class="font-bold">Analytics</h3>
        <p class="mt-2 text-sm text-slate-500">Understand your business data.</p>
      </a>

      <a href="#dashboard" class="rounded-xl p-4 hover:bg-indigo-50">
        <h3 class="font-bold">Dashboard</h3>
        <p class="mt-2 text-sm text-slate-500">Manage projects and performance.</p>
      </a>

      <a href="#pricing" class="rounded-xl p-4 hover:bg-indigo-50">
        <h3 class="font-bold">Subscriptions</h3>
        <p class="mt-2 text-sm text-slate-500">Choose a plan for your team.</p>
      </a>

      <a href="#faq" class="rounded-xl p-4 hover:bg-indigo-50">
        <h3 class="font-bold">Help Center</h3>
        <p class="mt-2 text-sm text-slate-500">Find answers to common questions.</p>
      </a>
    </div>
  </div>

  <!-- Mobile navigation -->
  <div id="mobileMenu" class="hidden space-y-3 border-t px-5 py-5 md:hidden">
    <a class="block" href="#home">Home</a>
    <a class="block" href="#features">Features</a>
    <a class="block" href="#pricing">Pricing</a>
    <a class="block" href="#dashboard">Dashboard</a>
    <a class="block" href="#profile">Profile</a>
    <a class="block" href="#settings">Settings</a>
    <a class="block" href="#login">Login</a>
    <a class="block" href="#signup">Sign Up</a>
  </div>
</header>
```

## HERO SECTION
```
<section id="home" class="bg-gradient-to-br from-indigo-50 via-white to-blue-50">
  <div class="mx-auto grid max-w-7xl items-center gap-12 px-5 py-24 md:grid-cols-2">

    <div>
      <span class="rounded-full bg-indigo-100 px-4 py-2 text-sm font-semibold text-indigo-700">
        The smarter way to work
      </span>

      <h1 class="mt-7 text-4xl font-extrabold leading-tight tracking-tight md:text-6xl">
        Manage Your Business
        <span class="text-indigo-600">With Confidence.</span>
      </h1>

      <p class="mt-6 text-lg leading-8 text-slate-600">
        Bring your projects, team, analytics, and workflow together
        in one simple platform designed for growing businesses.
      </p>

      <div class="mt-8 flex flex-wrap gap-4">
        <a href="#signup"
           class="rounded-lg bg-indigo-600 px-6 py-3 font-semibold text-white hover:bg-indigo-700">
          Start Free
        </a>

        <a href="#features"
           class="rounded-lg border border-slate-300 bg-white px-6 py-3 font-semibold hover:bg-slate-50">
          Explore Features
        </a>
      </div>

      <p class="mt-5 text-sm text-slate-500">
        No credit card required for this demo.
      </p>
    </div>

    <div class="rounded-3xl border bg-white p-5 shadow-2xl">
      <div class="rounded-2xl bg-slate-900 p-7 text-white">
        <p class="text-sm text-slate-400">Monthly Overview</p>
        <h2 class="mt-4 text-4xl font-bold">$24,680</h2>
        <p class="mt-2 text-sm text-emerald-400">↑ 12.8% from last month</p>

        <div class="mt-8 grid grid-cols-2 gap-4">
          <div class="rounded-xl bg-white/10 p-4">
            <p class="text-sm text-slate-300">Active Users</p>
            <h3 class="mt-2 text-2xl font-bold">1,284</h3>
          </div>

          <div class="rounded-xl bg-white/10 p-4">
            <p class="text-sm text-slate-300">Projects</p>
            <h3 class="mt-2 text-2xl font-bold">36</h3>
          </div>
        </div>
      </div>
    </div>

  </div>
</section>
```
## FEATURE CARDS
```
<section id="features" class="mx-auto max-w-7xl px-5 py-24">

  <div class="mx-auto max-w-2xl text-center">
    <p class="font-semibold text-indigo-600">OUR FEATURES</p>
    <h2 class="mt-3 text-3xl font-bold md:text-4xl">
      Everything Your Team Needs
    </h2>
    <p class="mt-4 text-slate-600">
      Powerful tools that make daily work easier.
    </p>
  </div>

  <div class="mt-14 grid gap-6 md:grid-cols-2 lg:grid-cols-3">

    <article class="rounded-2xl border p-7 transition hover:-translate-y-1 hover:shadow-xl">
      <div class="text-4xl">📊</div>
      <h3 class="mt-5 text-xl font-bold">Analytics</h3>
      <p class="mt-3 leading-7 text-slate-600">
        Track performance and understand your business with clear reports.
      </p>
    </article>

    <article class="rounded-2xl border p-7 transition hover:-translate-y-1 hover:shadow-xl">
      <div class="text-4xl">👥</div>
      <h3 class="mt-5 text-xl font-bold">Team Collaboration</h3>
      <p class="mt-3 leading-7 text-slate-600">
        Help your team communicate and work together efficiently.
      </p>
    </article>

    <article class="rounded-2xl border p-7 transition hover:-translate-y-1 hover:shadow-xl">
      <div class="text-4xl">⚡</div>
      <h3 class="mt-5 text-xl font-bold">Automation</h3>
      <p class="mt-3 leading-7 text-slate-600">
        Simplify repetitive tasks and spend more time on important work.
      </p>
    </article>

    <article class="rounded-2xl border p-7 transition hover:-translate-y-1 hover:shadow-xl">
      <div class="text-4xl">🔒</div>
      <h3 class="mt-5 text-xl font-bold">Security</h3>
      <p class="mt-3 leading-7 text-slate-600">
        Build a secure experience with appropriate access controls.
      </p>
    </article>

    <article class="rounded-2xl border p-7 transition hover:-translate-y-1 hover:shadow-xl">
      <div class="text-4xl">☁️</div>
      <h3 class="mt-5 text-xl font-bold">Cloud Access</h3>
      <p class="mt-3 leading-7 text-slate-600">
        Access your workspace from supported devices and locations.
      </p>
    </article>

    <article class="rounded-2xl border p-7 transition hover:-translate-y-1 hover:shadow-xl">
      <div class="text-4xl">🎯</div>
      <h3 class="mt-5 text-xl font-bold">Goal Tracking</h3>
      <p class="mt-3 leading-7 text-slate-600">
        Organize goals, follow progress, and keep projects moving.
      </p>
    </article>

  </div>
</section>
```
## PRICING CARDS
```
<section id="pricing" class="bg-slate-50 px-5 py-24">

  <div class="mx-auto max-w-7xl">
    <div class="text-center">
      <p class="font-semibold text-indigo-600">PRICING</p>
      <h2 class="mt-3 text-3xl font-bold md:text-4xl">
        Choose Your Perfect Plan
      </h2>
      <p class="mt-4 text-slate-600">
        Sample prices for this UI demo.
      </p>
    </div>

    <div class="mt-14 grid gap-7 lg:grid-cols-3">

      <article class="rounded-2xl border bg-white p-8 shadow-sm">
        <h3 class="text-xl font-bold">Starter</h3>
        <p class="mt-3 text-slate-500">For individuals</p>
        <p class="mt-6 text-4xl font-extrabold">$0<span class="text-sm font-normal text-slate-500"> / month</span></p>

        <ul class="mt-8 space-y-4 text-slate-600">
          <li>✓ Basic dashboard</li>
          <li>✓ Up to 3 projects</li>
          <li>✓ Basic analytics</li>
        </ul>

        <a href="#signup" class="mt-8 block rounded-lg border py-3 text-center font-semibold hover:bg-slate-50">
          Get Started
        </a>
      </article>

      <article class="relative rounded-2xl border-2 border-indigo-600 bg-white p-8 shadow-xl">
        <span class="rounded-full bg-indigo-100 px-3 py-1 text-xs font-bold text-indigo-700">
          MOST POPULAR
        </span>
        <h3 class="mt-5 text-xl font-bold">Professional</h3>
        <p class="mt-3 text-slate-500">For growing teams</p>
        <p class="mt-6 text-4xl font-extrabold">$19<span class="text-sm font-normal text-slate-500"> / month</span></p>

        <ul class="mt-8 space-y-4 text-slate-600">
          <li>✓ Unlimited projects</li>
          <li>✓ Advanced analytics</li>
          <li>✓ Priority support</li>
        </ul>

        <a href="#signup" class="mt-8 block rounded-lg bg-indigo-600 py-3 text-center font-semibold text-white hover:bg-indigo-700">
          Choose Professional
        </a>
      </article>

      <article class="rounded-2xl border bg-white p-8 shadow-sm">
        <h3 class="text-xl font-bold">Business</h3>
        <p class="mt-3 text-slate-500">For larger organizations</p>
        <p class="mt-6 text-4xl font-extrabold">$49<span class="text-sm font-normal text-slate-500"> / month</span></p>

        <ul class="mt-8 space-y-4 text-slate-600">
          <li>✓ Team permissions</li>
          <li>✓ Custom reports</li>
          <li>✓ Dedicated support</li>
        </ul>

        <a href="#signup" class="mt-8 block rounded-lg border py-3 text-center font-semibold hover:bg-slate-50">
          Choose Business
        </a>
      </article>

    </div>
  </div>
</section>
```

## TESTIMONIALS
```
<section class="mx-auto max-w-7xl px-5 py-24">

  <div class="text-center">
    <p class="font-semibold text-indigo-600">TESTIMONIALS</p>
    <h2 class="mt-3 text-3xl font-bold md:text-4xl">
      What Our Customers Say
    </h2>
  </div>

  <div class="mt-12 grid gap-6 md:grid-cols-3">

    <article class="rounded-2xl border p-7">
      <p class="text-xl text-amber-500">★★★★★</p>
      <p class="mt-4 leading-7 text-slate-600">
        "CloudFlow helps our team stay organized and focus on priorities."
      </p>
      <h3 class="mt-6 font-bold">Jordan Lee</h3>
      <p class="text-sm text-slate-500">Project Manager</p>
    </article>

    <article class="rounded-2xl border p-7">
      <p class="text-xl text-amber-500">★★★★★</p>
      <p class="mt-4 leading-7 text-slate-600">
        "The dashboard gives us a quick overview of our work."
      </p>
      <h3 class="mt-6 font-bold">Sam Rivera</h3>
      <p class="text-sm text-slate-500">Business Owner</p>
    </article>

    <article class="rounded-2xl border p-7">
      <p class="text-xl text-amber-500">★★★★★</p>
      <p class="mt-4 leading-7 text-slate-600">
        "The simple layout makes it easy for new team members to start."
      </p>
      <h3 class="mt-6 font-bold">Taylor Morgan</h3>
      <p class="text-sm text-slate-500">Product Designer</p>
    </article>

  </div>

  <p class="mt-4 text-center text-xs text-slate-400">
    Sample testimonials for demonstration only.
  </p>
</section>
```

## FAQ
```
<section id="faq" class="bg-slate-50 px-5 py-24">

  <div class="mx-auto max-w-3xl">
    <div class="text-center">
      <h2 class="text-3xl font-bold md:text-4xl">
        Frequently Asked Questions
      </h2>
      <p class="mt-4 text-slate-600">
        Find answers to common questions.
      </p>
    </div>

    <div class="mt-10 space-y-4">

      <details class="rounded-xl border bg-white p-5">
        <summary class="cursor-pointer font-semibold">
          Can I start for free?
        </summary>
        <p class="mt-4 leading-7 text-slate-600">
          Yes, this demo includes a sample free plan. Configure your actual
          product pricing and trial rules before launch.
        </p>
      </details>

      <details class="rounded-xl border bg-white p-5">
        <summary class="cursor-pointer font-semibold">
          Can I change my plan later?
        </summary>
        <p class="mt-4 leading-7 text-slate-600">
          A production application can support plan changes when connected
          to a billing service.
        </p>
      </details>

      <details class="rounded-xl border bg-white p-5">
        <summary class="cursor-pointer font-semibold">
          Is my data secure?
        </summary>
        <p class="mt-4 leading-7 text-slate-600">
          Security depends on your implementation. Add secure authentication,
          authorization, validation, and data storage.
        </p>
      </details>

      <details class="rounded-xl border bg-white p-5">
        <summary class="cursor-pointer font-semibold">
          Can I use CloudFlow on mobile?
        </summary>
        <p class="mt-4 leading-7 text-slate-600">
          This layout is responsive and adapts to mobile, tablet, and desktop
          screens.
        </p>
      </details>

    </div>
  </div>
</section>
```

## CALL TO ACTION
```
<section class="px-5 py-20">
  <div class="mx-auto max-w-7xl rounded-3xl bg-indigo-600 px-6 py-16 text-center sm:px-12">

    <h2 class="text-3xl font-extrabold text-white md:text-5xl">
      Ready to Grow Your Business?
    </h2>

    <p class="mx-auto mt-5 max-w-2xl leading-7 text-indigo-100">
      Bring your projects, people, and insights together in one workspace.
    </p>

    <a href="#signup"
       class="mt-8 inline-block rounded-lg bg-white px-7 py-3 font-bold text-indigo-700 hover:bg-indigo-50">
      Start Today
    </a>

  </div>
</section>
```

 ## FOOTER
 ```
<footer class="border-t bg-white">

  <div class="mx-auto grid max-w-7xl gap-10 px-5 py-14 sm:grid-cols-2 lg:grid-cols-4">

    <div>
      <h2 class="text-2xl font-extrabold text-indigo-600">CloudFlow</h2>
      <p class="mt-4 max-w-xs leading-7 text-slate-500">
        A simple workspace for modern teams and growing businesses.
      </p>
    </div>

    <div>
      <h3 class="font-bold">Product</h3>
      <div class="mt-4 space-y-3 text-slate-500">
        <a href="#features" class="block hover:text-indigo-600">Features</a>
        <a href="#pricing" class="block hover:text-indigo-600">Pricing</a>
        <a href="#dashboard" class="block hover:text-indigo-600">Dashboard</a>
      </div>
    </div>

    <div>
      <h3 class="font-bold">Company</h3>
      <div class="mt-4 space-y-3 text-slate-500">
        <a href="#home" class="block hover:text-indigo-600">About</a>
        <a href="#faq" class="block hover:text-indigo-600">Help Center</a>
        <a href="#home" class="block hover:text-indigo-600">Contact</a>
      </div>
    </div>

    <div>
      <h3 class="font-bold">Account</h3>
      <div class="mt-4 space-y-3 text-slate-500">
        <a href="#login" class="block hover:text-indigo-600">Login</a>
        <a href="#signup" class="block hover:text-indigo-600">Create Account</a>
        <a href="#settings" class="block hover:text-indigo-600">Settings</a>
      </div>
    </div>

  </div>

  <div class="border-t px-5 py-5 text-center text-sm text-slate-500">
    © <span id="year"></span> CloudFlow. All rights reserved.
  </div>
</footer>
```

## DASHBOARD
```
<section id="dashboard" class="border-t bg-slate-50 px-4 py-16 sm:px-6 lg:px-8">

  <div class="mx-auto max-w-7xl">
    <div class="flex flex-col justify-between gap-4 sm:flex-row sm:items-center">
      <div>
        <p class="text-sm text-slate-500">Workspace / Overview</p>
        <h1 class="mt-2 text-3xl font-bold">Dashboard</h1>
        <p class="mt-2 text-slate-500">Welcome back! Here is your overview.</p>
      </div>

      <button onclick="alert('Connect this button to your project creation form.')"
              class="rounded-lg bg-indigo-600 px-5 py-3 font-semibold text-white hover:bg-indigo-700">
        + New Project
      </button>
    </div>

    <div class="mt-8 grid gap-5 sm:grid-cols-2 lg:grid-cols-4">

      <article class="rounded-2xl border bg-white p-6 shadow-sm">
        <p class="text-sm text-slate-500">Total Revenue</p>
        <h2 class="mt-3 text-3xl font-bold">$24,680</h2>
        <p class="mt-2 text-sm text-emerald-600">↑ 12.8%</p>
      </article>

      <article class="rounded-2xl border bg-white p-6 shadow-sm">
        <p class="text-sm text-slate-500">Active Users</p>
        <h2 class="mt-3 text-3xl font-bold">1,284</h2>
        <p class="mt-2 text-sm text-emerald-600">↑ 8.2%</p>
      </article>

      <article class="rounded-2xl border bg-white p-6 shadow-sm">
        <p class="text-sm text-slate-500">Projects</p>
        <h2 class="mt-3 text-3xl font-bold">36</h2>
        <p class="mt-2 text-sm text-emerald-600">↑ 4.6%</p>
      </article>

      <article class="rounded-2xl border bg-white p-6 shadow-sm">
        <p class="text-sm text-slate-500">Open Tasks</p>
        <h2 class="mt-3 text-3xl font-bold">18</h2>
        <p class="mt-2 text-sm text-amber-600">Needs attention</p>
      </article>

    </div>

    <div class="mt-8 grid gap-6 lg:grid-cols-3">

      <!-- 11. SIDEBAR -->
      <aside class="rounded-2xl border bg-white p-5">
        <h2 class="text-lg font-bold">Workspace Menu</h2>

        <nav class="mt-5 space-y-2">
          <a href="#dashboard" class="block rounded-lg bg-indigo-50 px-4 py-3 font-semibold text-indigo-700">
            ▦ Overview
          </a>
          <a href="#profile" class="block rounded-lg px-4 py-3 hover:bg-slate-100">
            👤 Profile
          </a>
          <a href="#settings" class="block rounded-lg px-4 py-3 hover:bg-slate-100">
            ⚙ Settings
          </a>
          <a href="#notifications" class="block rounded-lg px-4 py-3 hover:bg-slate-100">
            🔔 Notifications
          </a>
          <a href="#login" class="block rounded-lg px-4 py-3 hover:bg-slate-100">
            ↪ Sign In
          </a>
        </nav>
      </aside>

      <div class="space-y-6 lg:col-span-2">

        <!-- 12. DATA TABLE -->
        <section class="overflow-hidden rounded-2xl border bg-white">
          <div class="border-b p-5">
            <h2 class="text-lg font-bold">Recent Projects</h2>
            <p class="mt-1 text-sm text-slate-500">An overview of your latest work.</p>
          </div>

          <div class="overflow-x-auto">
            <table class="w-full min-w-[580px] text-left text-sm">
              <thead class="bg-slate-50 text-slate-500">
                <tr>
                  <th class="px-5 py-4">Project</th>
                  <th class="px-5 py-4">Owner</th>
                  <th class="px-5 py-4">Status</th>
                  <th class="px-5 py-4">Due Date</th>
                </tr>
              </thead>

              <tbody class="divide-y">
                <tr>
                  <td class="px-5 py-4 font-semibold">Website Redesign</td>
                  <td class="px-5 py-4">Alex</td>
                  <td class="px-5 py-4">
                    <span class="rounded-full bg-blue-100 px-3 py-1 text-xs text-blue-700">
                      In Progress
                    </span>
                  </td>
                  <td class="px-5 py-4">Oct 30</td>
                </tr>

                <tr>
                  <td class="px-5 py-4 font-semibold">Mobile App</td>
                  <td class="px-5 py-4">Jamie</td>
                  <td class="px-5 py-4">
                    <span class="rounded-full bg-amber-100 px-3 py-1 text-xs text-amber-700">
                      Review
                    </span>
                  </td>
                  <td class="px-5 py-4">Nov 04</td>
                </tr>

                <tr>
                  <td class="px-5 py-4 font-semibold">Customer Portal</td>
                  <td class="px-5 py-4">Riley</td>
                  <td class="px-5 py-4">
                    <span class="rounded-full bg-emerald-100 px-3 py-1 text-xs text-emerald-700">
                      Completed
                    </span>
                  </td>
                  <td class="px-5 py-4">Oct 21</td>
                </tr>
              </tbody>
            </table>
          </div>
        </section>
```

        ## NOTIFICATION PANEL
        ```
        <section id="notifications" class="rounded-2xl border bg-white p-5">
          <div class="flex items-center justify-between">
            <h2 class="text-lg font-bold">Notifications</h2>
            <button onclick="markNotificationsRead()"
                    class="text-sm font-semibold text-indigo-600 hover:text-indigo-800">
              Mark all read
            </button>
          </div>

          <div id="notificationList" class="mt-4 divide-y">

            <article class="notification-item flex gap-3 py-4">
              <span class="mt-2 h-3 w-3 rounded-full bg-emerald-500"></span>
              <div>
                <h3 class="font-semibold">Project approved</h3>
                <p class="mt-1 text-sm text-slate-500">Website redesign moved to the next stage.</p>
                <p class="mt-2 text-xs text-slate-400">10 minutes ago</p>
              </div>
            </article>

            <article class="notification-item flex gap-3 py-4">
              <span class="mt-2 h-3 w-3 rounded-full bg-indigo-500"></span>
              <div>
                <h3 class="font-semibold">New team member</h3>
                <p class="mt-1 text-sm text-slate-500">A new member joined your workspace.</p>
                <p class="mt-2 text-xs text-slate-400">1 hour ago</p>
              </div>
            </article>

            <article class="notification-item flex gap-3 py-4">
              <span class="mt-2 h-3 w-3 rounded-full bg-amber-500"></span>
              <div>
                <h3 class="font-semibold">Deadline reminder</h3>
                <p class="mt-1 text-sm text-slate-500">A project deadline is approaching.</p>
                <p class="mt-2 text-xs text-slate-400">Yesterday</p>
              </div>
            </article>

          </div>
        </section>

      </div>
    </div>
  </div>
</section>
```

 ## PROFILE PAGE
 ```
<section id="profile" class="border-t bg-slate-50 px-5 py-20">

  <div class="mx-auto max-w-3xl">
    <h2 class="text-3xl font-bold">My Profile</h2>
    <p class="mt-2 text-slate-500">Manage your personal information.</p>

    <form onsubmit="saveDemoForm(event, 'Profile')"
          class="mt-8 space-y-6 rounded-2xl border bg-white p-6 sm:p-8">

      <div class="flex items-center gap-4">
        <div class="flex h-16 w-16 items-center justify-center rounded-full bg-indigo-100 text-2xl font-bold text-indigo-700">
          JD
        </div>
        <div>
          <h3 class="font-bold">Jordan Davis</h3>
          <p class="text-sm text-slate-500">Workspace Member</p>
        </div>
      </div>

      <div class="grid gap-5 sm:grid-cols-2">
        <label class="block text-sm font-medium">
          First Name
          <input required type="text" value="Jordan"
                 class="mt-2 w-full rounded-lg border px-4 py-3 focus:border-indigo-500 focus:outline-none focus:ring-2 focus:ring-indigo-100">
        </label>

        <label class="block text-sm font-medium">
          Last Name
          <input required type="text" value="Davis"
                 class="mt-2 w-full rounded-lg border px-4 py-3 focus:border-indigo-500 focus:outline-none focus:ring-2 focus:ring-indigo-100">
        </label>
      </div>

      <label class="block text-sm font-medium">
        Email Address
        <input required type="email" value="jordan@example.com"
               class="mt-2 w-full rounded-lg border px-4 py-3 focus:border-indigo-500 focus:outline-none focus:ring-2 focus:ring-indigo-100">
      </label>

      <label class="block text-sm font-medium">
        About Me
        <textarea rows="4"
                  class="mt-2 w-full rounded-lg border px-4 py-3 focus:border-indigo-500 focus:outline-none focus:ring-2 focus:ring-indigo-100">Product enthusiast and team collaborator.</textarea>
      </label>

      <button class="rounded-lg bg-indigo-600 px-5 py-3 font-semibold text-white hover:bg-indigo-700">
        Save Profile
      </button>
    </form>
  </div>
</section>
```


## SETTINGS PAGE
```
<section id="settings" class="border-t bg-slate-50 px-5 py-20">

  <div class="mx-auto max-w-3xl">
    <h2 class="text-3xl font-bold">Settings</h2>
    <p class="mt-2 text-slate-500">Customize your account preferences.</p>

    <form onsubmit="saveDemoForm(event, 'Settings')"
          class="mt-8 rounded-2xl border bg-white p-6 sm:p-8">

      <h3 class="text-xl font-bold">Notifications</h3>

      <div class="mt-5 divide-y">

        <label class="flex cursor-pointer items-center justify-between gap-4 py-5">
          <span>
            <span class="block font-semibold">Product Updates</span>
            <span class="mt-1 block text-sm text-slate-500">Receive news about new features.</span>
          </span>
          <input type="checkbox" checked class="h-5 w-5 accent-indigo-600">
        </label>

        <label class="flex cursor-pointer items-center justify-between gap-4 py-5">
          <span>
            <span class="block font-semibold">Weekly Summary</span>
            <span class="mt-1 block text-sm text-slate-500">Get a weekly workspace summary.</span>
          </span>
          <input type="checkbox" class="h-5 w-5 accent-indigo-600">
        </label>

        <label class="flex cursor-pointer items-center justify-between gap-4 py-5">
          <span>
            <span class="block font-semibold">Security Alerts</span>
            <span class="mt-1 block text-sm text-slate-500">Receive important security alerts.</span>
          </span>
          <input type="checkbox" checked class="h-5 w-5 accent-indigo-600">
        </label>

      </div>

      <button class="mt-5 rounded-lg bg-indigo-600 px-5 py-3 font-semibold text-white hover:bg-indigo-700">
        Save Settings
      </button>
    </form>
  </div>
</section>
```
## AUTHENTICATION PAGES
### Login
```
<section id="login" class="border-t bg-slate-100 px-5 py-20">

  <div class="mx-auto max-w-md rounded-3xl border bg-white p-8 shadow-sm">

    <h2 class="text-center text-3xl font-bold">Welcome Back</h2>
    <p class="mt-3 text-center text-slate-500">Sign in to your account.</p>

    <form onsubmit="demoLogin(event)" class="mt-8 space-y-5">

      <label class="block text-sm font-medium">
        Email Address
        <input required type="email" placeholder="you@example.com"
               class="mt-2 w-full rounded-lg border px-4 py-3 focus:border-indigo-500 focus:outline-none focus:ring-2 focus:ring-indigo-100">
      </label>

      <label class="block text-sm font-medium">
        Password
        <input required type="password" placeholder="Enter your password"
               class="mt-2 w-full rounded-lg border px-4 py-3 focus:border-indigo-500 focus:outline-none focus:ring-2 focus:ring-indigo-100">
      </label>

      <div class="text-right">
        <a href="#forgotPassword" class="text-sm font-semibold text-indigo-600">
          Forgot Password?
        </a>
      </div>

      <button class="w-full rounded-lg bg-indigo-600 py-3 font-semibold text-white hover:bg-indigo-700">
        Sign In
      </button>
    </form>

    <p class="mt-6 text-center text-sm text-slate-500">
      Don't have an account?
      <a href="#signup" class="font-semibold text-indigo-600">Sign Up</a>
    </p>
  </div>
</section>
```


### Signup
```
<section id="signup" class="border-t bg-slate-50 px-5 py-20">

  <div class="mx-auto max-w-md rounded-3xl border bg-white p-8 shadow-sm">

    <h2 class="text-center text-3xl font-bold">Create Account</h2>
    <p class="mt-3 text-center text-slate-500">Start building with CloudFlow.</p>

    <form onsubmit="saveDemoForm(event, 'Sign up')" class="mt-8 space-y-5">

      <label class="block text-sm font-medium">
        Full Name
        <input required type="text" placeholder="Your full name"
               class="mt-2 w-full rounded-lg border px-4 py-3 focus:border-indigo-500 focus:outline-none focus:ring-2 focus:ring-indigo-100">
      </label>

      <label class="block text-sm font-medium">
        Email Address
        <input required type="email" placeholder="you@example.com"
               class="mt-2 w-full rounded-lg border px-4 py-3 focus:border-indigo-500 focus:outline-none focus:ring-2 focus:ring-indigo-100">
      </label>

      <label class="block text-sm font-medium">
        Password
        <input required minlength="8" type="password" placeholder="At least 8 characters"
               class="mt-2 w-full rounded-lg border px-4 py-3 focus:border-indigo-500 focus:outline-none focus:ring-2 focus:ring-indigo-100">
      </label>

      <button class="w-full rounded-lg bg-indigo-600 py-3 font-semibold text-white hover:bg-indigo-700">
        Create Account
      </button>
    </form>

    <p class="mt-6 text-center text-sm text-slate-500">
      Already registered?
      <a href="#login" class="font-semibold text-indigo-600">Sign In</a>
    </p>
  </div>
</section>
```


### Forgot password
```
<section id="forgotPassword" class="border-t bg-slate-100 px-5 py-20">

  <div class="mx-auto max-w-md rounded-3xl border bg-white p-8 shadow-sm">

    <h2 class="text-center text-3xl font-bold">Reset Password</h2>
    <p class="mt-3 text-center text-slate-500">
      Enter your email to request a password reset.
    </p>

    <form onsubmit="saveDemoForm(event, 'Password reset request')" class="mt-8 space-y-5">
      <label class="block text-sm font-medium">
        Email Address
        <input required type="email" placeholder="you@example.com"
               class="mt-2 w-full rounded-lg border px-4 py-3 focus:border-indigo-500 focus:outline-none focus:ring-2 focus:ring-indigo-100">
      </label>

      <button class="w-full rounded-lg bg-indigo-600 py-3 font-semibold text-white hover:bg-indigo-700">
        Request Reset
      </button>
    </form>

    <p class="mt-6 text-center">
      <a href="#login" class="text-sm font-semibold text-indigo-600">Back to Login</a>
    </p>
  </div>
</section>
```
