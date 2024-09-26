# SvelteKit Demo

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
