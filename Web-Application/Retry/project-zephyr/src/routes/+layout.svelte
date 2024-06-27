<script>
  import "../app.css";

  import { onMount } from 'svelte';

  onMount(() => {
    if (typeof document !== 'undefined') {
      document.documentElement.classList.add('dark');
    }
  });
</script>

<slot />