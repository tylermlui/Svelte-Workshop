# SvelteKit Demo

### Going to github first
Creating new repo
cloning it

Create App<br>
``` npm create svelte@latest my-app```<br>
<br>cd<br>
```cd my-app```<br>
<br>npm i <br>
```npm install```<br><br>
running it locally<br>
```npm run dev```<br>


![image](https://github.com/user-attachments/assets/7cad23b9-438f-42e8-8799-1db8f4fd5d1d)


CHANGING HOME PAGE / BASE ROUTE
![image](https://github.com/user-attachments/assets/0ed03548-f222-4498-86b2-c2f19d6695a4)

ADDING COUNTER ROUTE

![image](https://github.com/user-attachments/assets/16ad9712-7e96-48cb-a411-3c8a0b05aa17)


BASE SCRIPT FOR COUNTER --- THIS IS REACTIVE AS COUNT IS CHANGED AUTOMATICALLY AND WE DO NOT NEED TO UPDATE THE DOM
```
<script>
    let count = 0;
</script>

<button on:click={() => count++}>
    count is {count}
</button>
```

CHANGE THE SCRIPT TO LOOK NICER
```
<script>
    let count = 0;
</script>

<div> 
    count is {count}
</div>

<button on:click={() => count++}>
    add
</button>

<button on:click={() => count--}>
    subtract
</button>
```

# Components

add components folder and add component

![image](https://github.com/user-attachments/assets/cdbe82e1-c44f-450f-bfe6-501f8f7e9213)

# Now adding it in the other pages
```
<script>
    import Nav from "$lib/components/nav.svelte";
</script>
<Nav/>
<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
```


# looping 


```
<script>
    let array = [1,2,3,4]
    import Nav from "$lib/components/nav.svelte";
</script>
<Nav/>
<div> ABOUT</div>
{#each array as i }
    {#if i >2 }
    <h1> {i}</h1>
    {/if}
    <div> {i} </div>
{/each}
```

