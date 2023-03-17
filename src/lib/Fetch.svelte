<script>
    import { onMount } from "svelte";

    let users = [];
    onMount(async () => {
        try {
            const response = await fetch(
                "https://jsonplaceholder.typicode.com/users"
            );
            users = await response.json();
        } catch (error) {
            console.log(error);
        }
    });
</script>

<!-- <p>{JSON.stringify(users)}</p> -->

{#each users as user}
    <p>{JSON.stringify(user)}</p>
{/each}
