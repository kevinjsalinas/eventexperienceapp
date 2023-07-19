<script>

    let profileImage = 'https://t4.ftcdn.net/jpg/04/83/90/95/360_F_483909569_OI4LKNeFgHwvvVju60fejLd9gj43dIcd.jpg'

</script>

<main>
    <h1>
        Welcome User
    </h1>

    <img src={profileImage} alt="profile">
    <form action="profile">
        <label for="fname">First Name:</label>
        <input type="text" id='fname' name='fname'><br><br>
        <label for="lname">Last Name:</label>
        <input type="text" id='lname' name='lname'><br><br>
        <label for="email">Email:</label>
        <input type="text" id='email' name='email'><br><br>
        <label for="password">Password:</label>
        <input type="password" id='password' name='password'><br><br>
        <!-- I want to do this in react, using state to display form only when edit profile button is clicked -->
        <button>Edit profile</button>
        <button>Save</button>
    </form>
</main>


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


