<!-- confirmed: this project uses svelte material ui @smui -->

<script>
    import Form from './Form.svelte'
    import profile_icon from "./assets/profile_icon.jpg"


    let toggle = false;

    function toggleProfile() {
        toggle = !toggle
    }

</script>

<div class="container">
    <h1>
        Welcome User
    </h1>
    <div>
        <img src={profile_icon} alt="profile_image">
    </div>

    <button on:click={toggleProfile}>Edit profile</button>
        
    {#if toggle}
       <div>
            <Form/>
            <button on:click={toggleProfile}>Save</button>
        </div>
    {/if}
    
</div>

<!-- testing git contribution -->

<style>
    h1 {
        font-size: 2em;
    }

    img {
        flex: auto;
    }

    button {

        flex: auto;
    }
</style>


