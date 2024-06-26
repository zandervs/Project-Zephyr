<script lang="ts">
    // Optionally, you can add TypeScript logic here if needed
  </script>
  
  <style lang="postcss">
    :global(body) {
      margin: 0;
      font-family: system-ui, sans-serif;
    }
    main {
      display: grid;
      min-height: 100vh;
      place-items: center;
      background-color: hsl(var(--background));
      padding: 6rem 1.5rem;
    }
    .text-center {
      text-align: center;
    }
    .text-indigo-600 {
      color: hsl(222.2, 84%, 4.9%);
    }
    .text-gray-900 {
      color: hsl(0, 0%, 10%);
    }
    .text-gray-600 {
      color: hsl(0, 0%, 60%);
    }
    .bg-indigo-600 {
      background-color: hsl(222.2, 84%, 4.9%);
    }
    .hover\:bg-indigo-500:hover {
      background-color: hsl(222.2, 84%, 5.9%);
    }
    .focus-visible\:outline {
      outline: 2px solid hsl(222.2, 84%, 4.9%);
    }
    .focus-visible\:outline-2 {
      outline-width: 2px;
    }
    .focus-visible\:outline-offset-2 {
      outline-offset: 2px;
    }
    .rounded-md {
      border-radius: 0.375rem;
    }
    .shadow-sm {
      box-shadow: 0 1px 2px 0 rgba(0, 0, 0, 0.05);
    }
    .font-semibold {
      font-weight: 600;
    }
    .font-bold {
      font-weight: 700;
    }
    .tracking-tight {
      letter-spacing: -0.015em;
    }
    .leading-7 {
      line-height: 1.75rem;
    }
    .text-base {
      font-size: 1rem;
    }
    .text-sm {
      font-size: 0.875rem;
    }
    .mt-4 {
      margin-top: 1rem;
    }
    .mt-6 {
      margin-top: 1.5rem;
    }
    .mt-10 {
      margin-top: 2.5rem;
    }
    .flex {
      display: flex;
    }
    .gap-x-6 {
      column-gap: 1.5rem;
    }
    .px-3\.5 {
      padding-left: 0.875rem;
      padding-right: 0.875rem;
    }
    .py-2\.5 {
      padding-top: 0.625rem;
      padding-bottom: 0.625rem;
    }
    .sm\:py-32 {
      padding-top: 8rem;
      padding-bottom: 8rem;
    }
    .lg\:px-8 {
      padding-left: 2rem;
      padding-right: 2rem;
    }
    .sm\:text-5xl {
      font-size: 3rem;
      line-height: 1;
    }
  </style>
  
  <main class="grid min-h-full place-items-center bg-white px-6 py-24 sm:py-32 lg:px-8">
    <div class="text-center">
      <p class="text-base font-semibold text-indigo-400">404</p>
      <h1 class="mt-4 text-3xl font-bold tracking-tight text-gray-600 sm:text-5xl">Page not found</h1>
      <p class="mt-6 text-base leading-7 text-gray-600">Sorry, we couldn’t find the page you’re looking for.</p>
      <div class="mt-10 flex items-center justify-center gap-x-6">
        <a href="/home" class="rounded-md bg-indigo-500 px-3.5 py-2.5 text-sm font-semibold text-white shadow-sm hover:bg-indigo-400 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600">Go back home</a>
        <a href="/support" class="text-sm font-semibold">Contact support <span aria-hidden="true">&rarr;</span></a>
      </div>
    </div>
  </main>  