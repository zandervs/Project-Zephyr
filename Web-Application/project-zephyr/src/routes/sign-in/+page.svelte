<svelte:head>
  <title>Sign In - Project Zephyr</title>
</svelte:head>

<script lang="ts">
  import SignIn from 'clerk-sveltekit/client/SignIn.svelte';
  import ClerkLoading from 'clerk-sveltekit/client/ClerkLoading.svelte';
  import ClerkLoaded from 'clerk-sveltekit/client/ClerkLoaded.svelte';
  import LoadingSpinner from '$lib/LoadingSpinner.svelte';
</script>

<style lang="postcss">
  :global(html) {
    background-color: hsl(var(--background));
    color: hsl(var(--foreground));
    height: 100%;
  }

  :global(body) {
    margin: 0;
    height: 100%;
    background-color: hsl(var(--background));
    color: hsl(var(--foreground));
  }

  .container {
    display: flex;
    height: 100vh; /* Full viewport height */
  }

  .left-half {
    flex: 1;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 1rem; /* Add padding to ensure some space around the image */
  }

  .left-half img {
    max-width: 100%;
    max-height: 100%;
    object-fit: contain;
  }

  .right-half {
    flex: 1;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .sign-in-container {
    width: 100%;
    max-width: 400px;
    display: flex;
    align-items: center;
    justify-content: center;
  }
</style>

<div class="container">
  <div class="left-half">
    <img src="smart-phone-screen-with-messages.png" alt="Phone screen with messages">
  </div>

  <div class="right-half">
    <div class="sign-in-container">
      <ClerkLoading>
        <LoadingSpinner className="text-neutral-50" />
      </ClerkLoading>
      <ClerkLoaded>
        <SignIn redirectUrl="/" />
      </ClerkLoaded>
    </div>
  </div>
</div>