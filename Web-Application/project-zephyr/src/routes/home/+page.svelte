<script lang="ts">
  import NavBar from '$lib/NavBar.svelte';
  import { Separator } from "$lib/components/ui/separator";
</script>

<NavBar />

<main>
  <h1 class="prevent-select">
    Messages
  </h1>

  <Separator />

  <div class="container prevent-select">
    <div class="conversation-list">
      <ul role="list" class="divide-y divide-slate-700">
        <li class="chat-item flex justify-between gap-x-6 py-5">
          <div class="flex min-w-0 gap-x-4">
            <img class="h-12 w-12 flex-none rounded-full bg-gray-50" src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80" alt="">
            <div class="min-w-0 flex-auto">
              <p class="text-sm font-semibold leading-6">Leslie Alexander</p>
              <p class="mt-1 truncate text-xs leading-5 text-gray-500">leslie.alexander@example.com</p>
            </div>
          </div>
          <div class="hidden shrink-0 sm:flex sm:flex-col sm:items-end">
            <p class="mt-1 text-xs leading-5 text-gray-500">Last seen <time datetime="2023-01-23T13:23Z">3h ago</time></p>
          </div>
        </li>
        <li class="chat-item flex justify-between gap-x-6 py-5">
          <div class="flex min-w-0 gap-x-4">
            <img class="h-12 w-12 flex-none rounded-full bg-gray-50" src="https://images.unsplash.com/photo-1519244703995-f4e0f30006d5?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80" alt="">
            <div class="min-w-0 flex-auto">
              <p class="text-sm font-semibold leading-6">Michael Foster</p>
              <p class="mt-1 truncate text-xs leading-5 text-gray-500">michael.foster@example.com</p>
            </div>
          </div>
          <div class="hidden shrink-0 sm:flex sm:flex-col sm:items-end">
            <p class="mt-1 text-xs leading-5 text-gray-500">Last seen <time datetime="2023-01-23T13:23Z">3h ago</time></p>
          </div>
        </li>
        <li class="chat-item flex justify-between gap-x-6 py-5">
          <div class="flex min-w-0 gap-x-4">
            <img class="h-12 w-12 flex-none rounded-full bg-gray-50" src="https://images.unsplash.com/photo-1506794778202-cad84cf45f1d?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80" alt="">
            <div class="min-w-0 flex-auto">
              <p class="text-sm font-semibold leading-6">Dries Vincent</p>
              <p class="mt-1 truncate text-xs leading-5 text-gray-500">dries.vincent@example.com</p>
            </div>
          </div>
          <div class="hidden shrink-0 sm:flex sm:flex-col sm:items-end">
            <div class="mt-1 flex items-center gap-x-1.5">
              <div class="flex-none rounded-full bg-emerald-500/20 p-1">
                <div class="h-1.5 w-1.5 rounded-full bg-emerald-500"></div>
              </div>
              <p class="text-xs leading-5 text-gray-500">Online</p>
            </div>
          </div>
        </li>
        <li class="chat-item flex justify-between gap-x-6 py-5">
          <div class="flex min-w-0 gap-x-4">
            <img class="h-12 w-12 flex-none rounded-full bg-gray-50" src="https://images.unsplash.com/photo-1517841905240-472988babdf9?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80" alt="">
            <div class="min-w-0 flex-auto">
              <p class="text-sm font-semibold leading-6">Lindsay Walton</p>
              <p class="mt-1 truncate text-xs leading-5 text-gray-500">lindsay.walton@example.com</p>
            </div>
          </div>
          <div class="hidden shrink-0 sm:flex sm:flex-col sm:items-end">
            <p class="mt-1 text-xs leading-5 text-gray-500">Last seen <time datetime="2023-01-23T13:23Z">3h ago</time></p>
          </div>
        </li>
        <li class="chat-item flex justify-between gap-x-6 py-5">
          <div class="flex min-w-0 gap-x-4">
            <img class="h-12 w-12 flex-none rounded-full bg-gray-50" src="https://images.unsplash.com/photo-1438761681033-6461ffad8d80?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80" alt="">
            <div class="min-w-0 flex-auto">
              <p class="text-sm font-semibold leading-6">Courtney Henry</p>
              <p class="mt-1 truncate text-xs leading-5 text-gray-500">courtney.henry@example.com</p>
            </div>
          </div>
          <div class="hidden shrink-0 sm:flex sm:flex-col sm:items-end">
            <p class="mt-1 text-xs leading-5 text-gray-500">Last seen <time datetime="2023-01-23T13:23Z">3h ago</time></p>
          </div>
        </li>
        <li class="chat-item flex justify-between gap-x-6 py-5">
          <div class="flex min-w-0 gap-x-4">
            <img class="h-12 w-12 flex-none rounded-full bg-gray-50" src="https://images.unsplash.com/photo-1472099645785-5658abf4ff4e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80" alt="">
            <div class="min-w-0 flex-auto">
              <p class="text-sm font-semibold leading-6">Tom Cook</p>
              <p class="mt-1 truncate text-xs leading-5 text-gray-500">tom.cook@example.com</p>
            </div>
          </div>
          <div class="hidden shrink-0 sm:flex sm:flex-col sm:items-end">
            <div class="mt-1 flex items-center gap-x-1.5">
              <div class="flex-none rounded-full bg-emerald-500/20 p-1">
                <div class="h-1.5 w-1.5 rounded-full bg-emerald-500"></div>
              </div>
              <p class="text-xs leading-5 text-gray-500">Online</p>
            </div>
          </div>
        </li>
      </ul>
    </div>

    <div class="conversation-box">
    </div>
  </div>
</main>

<style lang="postcss">
  h1 {
    margin-top: 1rem;
    margin-left: 6rem;
    margin-bottom: 1rem;
    font-size: 45px;
    font-weight: 600;
  }

  .prevent-select {
    -webkit-user-select: none; /* Safari */
    -ms-user-select: none; /* IE 10 and IE 11 */
    user-select: none; /* Standard syntax */
  }

  .container {
    display: flex;
    flex-direction: row;
    margin-top: 2rem;
    width: 100%;
  }

  .conversation-list {
    flex: 1;
    margin-right: 2rem;
    margin-left: 0rem;
  }

  .chat-item {
    width: 35rem;
    padding: 1rem;
    border-radius: 1rem;
    margin-left: -12rem;
  }

  .chat-item:hover {
    background-color: #080733;
    cursor: pointer;
  }

  .conversation-box {
    flex: 2;
    flex-grow: 2;
    background-color: #050d25;
    border-radius: 1.5rem;
    padding: 1rem;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    height: 76vh;
    width: 80rem;
  }
</style>