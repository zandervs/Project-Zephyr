<script>
  import "../app.css";
  import { goto } from '$app/navigation';
  import { page } from '$app/stores';
  import { onMount } from 'svelte';

  onMount(() => {
    if (typeof document !== 'undefined') {
      document.documentElement.classList.add('dark');
    }

    const unsubscribe = page.subscribe($page => {
      if ($page.url.pathname === '/') {
        goto('/home');
      }
    });

    // Cleanup subscription on component destroy
    return () => {
      unsubscribe();
    };
  });
</script>

<svelte:head>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
</svelte:head>

<slot />