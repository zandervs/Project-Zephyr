<script lang="ts">
  import { page } from '$app/stores';
  import { onMount, onDestroy } from 'svelte';
  import { get } from 'svelte/store';

  import UserButton from 'clerk-sveltekit/client/UserButton.svelte';
  import SignedIn from 'clerk-sveltekit/client/SignedIn.svelte';
  import SignedOut from 'clerk-sveltekit/client/SignedOut.svelte';

  let isDropdownOpen = false;
  let dropdownRef;

  function toggleDropdown() {
    isDropdownOpen = !isDropdownOpen;
  }

  function closeDropdown() {
    isDropdownOpen = false;
  }

  function handleClickOutside(event) {
    if (dropdownRef && !dropdownRef.contains(event.target)) {
      closeDropdown();
    }
  }

  onMount(() => {
    document.addEventListener('click', handleClickOutside);

    return () => {
      document.removeEventListener('click', handleClickOutside);
    };
  });

  function isActive(route) {
    const { pathname } = get(page).url;
    return pathname === route;
  }
</script>

<nav class="bg-gray-800 prevent-select">
  <div class="mx-auto max-w-7xl px-2 sm:px-6 lg:px-8">
    <div class="relative flex h-16 items-center justify-between">
      <div class="flex flex-1 items-center justify-center sm:items-stretch sm:justify-start">
        <div class="flex flex-shrink-0 items-center">
          <img class="h-10 w-auto" src="message.png" alt="Project Zephyr">
        </div>
        <div class="hidden sm:ml-6 sm:block">
          <div class="flex space-x-4">
            <a href="/" class="rounded-md px-3 py-2 text-sm font-medium" class:current-page={isActive('/home')} aria-current="page">Messages</a>
            <a href="/server" class="rounded-md px-3 py-2 text-sm font-medium" class:current-page={isActive('/server')}>Server Status</a>
          </div>
        </div>
      </div>
      <div class="flex items-center space-x-4">
        <SignedIn let:user>
          <div class="flex items-center space-x-5">
            <span class="text-gray-300 text-sm">{user.firstName} {user.lastName}</span>
            <UserButton afterSignOutUrl="/sign-in" />
          </div>
        </SignedIn>
        <SignedOut>
          <a href="/sign-in" class="rounded-md px-3 py-2 text-sm font-medium text-gray-300 hover:bg-gray-700 hover:text-white">Sign In</a>
        </SignedOut>
        <div class="develop-text">
          Developmental Preview
          <p>
            v0.0.1
          </p>
        </div>
      </div>
    </div>
  </div>
</nav>

<style>
  .develop-text {
    color: red;
    margin-left: 1rem; /* This pushes the text to the right */
    display: flex;
    flex-direction: row;
  }

  .develop-text p {
    margin-left: 1rem;
    color: slategray;
  }

  /* Styles for active links */
  .current-page {
    background-color: #4B5563; /* Darker gray */
    color: white;
  }

  /* Default link styles */
  a {
    color: #9CA3AF; /* Light gray */
    text-decoration: none;
  }

  a:hover {
    background-color: #4B5563; /* Darker gray */
    color: white;
  }

  .prevent-select {
    -webkit-user-select: none; /* Safari */
    -ms-user-select: none; /* IE 10 and IE 11 */
    user-select: none; /* Standard syntax */
  }
</style>