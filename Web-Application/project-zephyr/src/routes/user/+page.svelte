<script lang="ts">
    import UserProfile from 'clerk-sveltekit/client/UserProfile.svelte';
    import * as Breadcrumb from "$lib/components/ui/breadcrumb/index.js";
  </script>
  
  <style lang="postcss">
    :global(body) {
      margin: 0;
      font-family: system-ui, sans-serif;
      background-color: hsl(var(--background));
      color: hsl(var(--foreground));
    }
  
    .breadcrumb-container {
      display: flex;
      align-items: center;
      justify-content: center;
      margin-top: 2rem;
    }
  
    .breadcrumb-container a,
    .breadcrumb-container span {
      font-size: 20px; /* Apply the font size to anchor and span elements */
    }
  
    .container {
      display: flex;
      justify-content: center;
      align-items: flex-start; /* Ensure content starts from the top */
      padding-top: 3rem;
      padding-bottom: 6rem;
    }
  </style>
  
  <div class="breadcrumb-container">
    <Breadcrumb.Root>
      <Breadcrumb.List>
        <Breadcrumb.Item>
          <Breadcrumb.Link href="/">Home</Breadcrumb.Link>
        </Breadcrumb.Item>
        <Breadcrumb.Separator />
        <Breadcrumb.Item>
          <Breadcrumb.Page>User Settings</Breadcrumb.Page>
        </Breadcrumb.Item>
      </Breadcrumb.List>
    </Breadcrumb.Root>
  </div>
  
  <div class="container">
    <UserProfile />
  </div>  