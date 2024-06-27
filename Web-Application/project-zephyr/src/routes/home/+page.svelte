<script lang="ts">
  import NavBar from '$lib/NavBar.svelte';
  import { Separator } from "$lib/components/ui/separator";
  import * as Tooltip from "$lib/components/ui/tooltip";
  import * as HoverCard from "$lib/components/ui/hover-card";
  import * as Avatar from "$lib/components/ui/avatar";
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
            <HoverCard.Root>
              <HoverCard.Trigger>
                <Avatar.Root class="h-14 w-14">
                  <Avatar.Image src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80" alt="Leslie Alexander" />
                  <Avatar.Fallback>LA</Avatar.Fallback>
                </Avatar.Root>
              </HoverCard.Trigger>
              <HoverCard.Content class="w-80">
                <div class="flex justify-between space-x-4">
                  <Avatar.Root class="h-14 w-14">
                    <Avatar.Image src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80" alt="Leslie Alexander" />
                    <Avatar.Fallback>LA</Avatar.Fallback>
                  </Avatar.Root>
                  <div class="space-y-1">
                    <h4 class="text-sm font-semibold">Leslie Alexander</h4>
                    <p class="text-sm">Living life</p>
                    <div class="flex items-center pt-2">
                      <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="size-6 mr-2 h-4 w-4 opacity-70">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M6.75 3v2.25M17.25 3v2.25M3 18.75V7.5a2.25 2.25 0 0 1 2.25-2.25h13.5A2.25 2.25 0 0 1 21 7.5v11.25m-18 0A2.25 2.25 0 0 0 5.25 21h13.5A2.25 2.25 0 0 0 21 18.75m-18 0v-7.5A2.25 2.25 0 0 1 5.25 9h13.5A2.25 2.25 0 0 1 21 11.25v7.5m-9-6h.008v.008H12v-.008ZM12 15h.008v.008H12V15Zm0 2.25h.008v.008H12v-.008ZM9.75 15h.008v.008H9.75V15Zm0 2.25h.008v.008H9.75v-.008ZM7.5 15h.008v.008H7.5V15Zm0 2.25h.008v.008H7.5v-.008Zm6.75-4.5h.008v.008h-.008v-.008Zm0 2.25h.008v.008h-.008V15Zm0 2.25h.008v.008h-.008v-.008Zm2.25-4.5h.008v.008H16.5v-.008Zm0 2.25h.008v.008H16.5V15Z" />
                      </svg>
                      <span class="text-xs text-muted-foreground">Joined September 2022</span>
                    </div>
                  </div>
                </div>
              </HoverCard.Content>
            </HoverCard.Root>
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
            <Avatar.Root class="h-14 w-14">
              <Avatar.Image src="https://images.unsplash.com/photo-1519244703995-f4e0f30006d5?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80" alt="Michael Foster" />
              <Avatar.Fallback>MF</Avatar.Fallback>
            </Avatar.Root>
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
            <Avatar.Root class="h-14 w-14">
              <Avatar.Image src="https://images.unsplash.com/photo-1506794778202-cad84cf45f1d?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80" alt="Dries Vincent" />
              <Avatar.Fallback>DV</Avatar.Fallback>
            </Avatar.Root>
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
            <Avatar.Root class="h-14 w-14">
              <Avatar.Image src="https://images.unsplash.com/photo-1517841905240-472988babdf9?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80" alt="Lindsay Walton" />
              <Avatar.Fallback>LW</Avatar.Fallback>
            </Avatar.Root>
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
            <Avatar.Root class="h-14 w-14">
              <Avatar.Image src="https://images.unsplash.com/photo-1438761681033-6461ffad8d80?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80" alt="Courtney Henry" />
              <Avatar.Fallback>CH</Avatar.Fallback>
            </Avatar.Root>
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
            <Avatar.Root class="h-14 w-14">
              <Avatar.Image src="https://images.unsplash.com/photo-1472099645785-5658abf4ff4e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80" alt="Tom Cook" />
              <Avatar.Fallback>TC</Avatar.Fallback>
            </Avatar.Root>
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
      <div class="content">

      </div>
      <div class="text-input">
        <div class="input-container">
          <input placeholder="Type a message">
          <Tooltip.Root>
            <Tooltip.Trigger>
              <button class="send-button">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="size-6">
                  <path stroke-linecap="round" stroke-linejoin="round" d="M6 12 3.269 3.125A59.769 59.769 0 0 1 21.485 12 59.768 59.768 0 0 1 3.27 20.875L5.999 12Zm0 0h7.5" />
                </svg>
              </button>
            </Tooltip.Trigger>
            <Tooltip.Content>
              <p>Send message</p>
            </Tooltip.Content>
          </Tooltip.Root>
        </div>
      </div>
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
    -webkit-user-select: none;
    -ms-user-select: none;
    user-select: none;
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

  .custom-avatar-size {
    width: 3rem;  /* Increase width */
    height: 3rem; /* Increase height */
  }

.custom-avatar-size img {
  width: 100%;
  height: 100%;
  border-radius: 50%; /* Ensure the image remains circular */
}


  .chat-item:hover {
    background-color: #080733;
    cursor: pointer;
  }

  .conversation-box {
    display: flex;
    flex-direction: column;
    flex: 2;
    flex-grow: 2;
    background-color: #050d25;
    border-radius: 1.5rem;
    padding: 0.75rem;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    height: 76vh;
    width: 80rem;
  }

  .content {
    flex: 1;
  }

  .input-container {
    display: flex;
    align-items: center;
  }

  .text-input {
    padding: 0.5rem;
    border-radius: 0 0 1.5rem 1.5rem; /* Match the bottom corners with the conversation box */
  }

  .text-input input {
    width: 100%;
    padding: 0.75rem;
    background: #091844;
    border: none;
    border-radius: 1rem;
    height: 3rem;
    color: white;
  }

  .text-input input::placeholder {
    color: theme(colors.slate.400);
  }

  .send-button {
    background: none;
    border: none;
    padding: 0.5rem;
    margin-left: 0.5rem;
    cursor: pointer;
  }

  .send-button svg {
    width: 24px;
    height: 24px;
    color: white;
  }
</style>