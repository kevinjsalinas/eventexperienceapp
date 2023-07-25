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
    <h2>
        Welcome User
    </h2>
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
	h2 {
		color: white;
		margin: 0.25em 0;
	}

    img {
        flex: auto;
    }

    button {

        flex: auto;
    }
</style>


