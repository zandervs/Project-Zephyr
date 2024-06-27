<script lang="ts">
    import NavBar from '$lib/NavBar.svelte';
    import { Separator } from "$lib/components/ui/separator";
    import { Progress } from "$lib/components/ui/progress";
    import { ScrollArea } from "$lib/components/ui/scroll-area/index.js";
    import * as Card from "$lib/components/ui/card";
  </script>
  
  <NavBar />
  
  <main class="prevent-select">
    <div class="heading">
      <h1>
        Server Status
      </h1>
      <h4 class="text-muted-foreground">
        A summary of storage usage and the state of feature functionality.
      </h4>
    </div>
  
    <Separator />

    <div class="container">
      <div class="left-half">
        <div class="card">
          <div class="storage">
            <div class="card-title">
              Total storage used
            </div>
  
            <div class="capacity-used">
              <h2>12.36 / 30GB</h2>
            </div>
      
            <Progress value={41} />
      
            <p class="text-muted-foreground">
              AWS EC2 t3.micro
            </p>
          </div>
        </div>
      </div>

      <div class="right-half">
        <ScrollArea>
          <div class="card-container">
            <div class="feature-card">
              <h1>Send and receive messages</h1>
              <div class="card-end">
                <p class="text-muted-foreground">Under development</p>

                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="size-6">
                  <path stroke-linecap="round" stroke-linejoin="round" d="M9.75 3.104v5.714a2.25 2.25 0 0 1-.659 1.591L5 14.5M9.75 3.104c-.251.023-.501.05-.75.082m.75-.082a24.301 24.301 0 0 1 4.5 0m0 0v5.714c0 .597.237 1.17.659 1.591L19.8 15.3M14.25 3.104c.251.023.501.05.75.082M19.8 15.3l-1.57.393A9.065 9.065 0 0 1 12 15a9.065 9.065 0 0 0-6.23-.693L5 14.5m14.8.8 1.402 1.402c1.232 1.232.65 3.318-1.067 3.611A48.309 48.309 0 0 1 12 21c-2.773 0-5.491-.235-8.135-.687-1.718-.293-2.3-2.379-1.067-3.61L5 14.5" />
                </svg>
              </div>              
            </div>
          </div>
        </ScrollArea>
      </div>
    </div>
  </main>

  <style lang="postcss">
    .heading {
      margin-left: 6rem;
      margin-bottom: 1rem;
    }

    .heading h1 {
      margin-top: 1rem;
      font-size: 45px;
      font-weight: 600;
    }

    .container {
      display: flex;
      flex-direction: row;
      align-items: center;
    }

    .card-container {
      display: flex;
      flex-direction: column;
    }

    .left-half {
      margin-top: 1rem;
      width: 50%;
    }

    .card {
      border-radius: 1rem;
      padding: 2rem;
      background: #050e29;
    }

    .storage {
      display: flex;
      flex-direction: column;
      justify-content: flex-start;
      align-items: flex-start;
      width: 20rem;
      padding: 0.5rem;
    }

    .capacity-used h2{
      color: theme(colors.neutral.50);
      font-size: 40px;
      font-weight: 600;
    }

    .right-half {
      margin-top: -7rem;
      width: 90%;
      display: flex;
      flex-direction: column;
      justify-content: flex-end;
    }

    .feature-card {
      display: flex;
      flex-direction: row;
      justify-content: space-between;
      align-items: center;
      width: 40rem;
      border-radius: 1rem;
      padding: 2rem;
      background: #050e29;
      height: 3rem;
      margin-left: 22rem;
    }

    .card-end {
      display: flex;
      flex-direction: row;
    }

    .card-end svg {
      margin-left: 0.5rem;
    }
  
    .prevent-select {
      -webkit-user-select: none;
      -ms-user-select: none;
      user-select: none;
    }
  </style>