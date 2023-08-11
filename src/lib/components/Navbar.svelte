<script lang=ts>
    import Icon from "svelte-awesome";
    import signIn from 'svelte-awesome/icons/signIn';
    import shoppingCart from 'svelte-awesome/icons/shoppingCart';
    import userPlus from 'svelte-awesome/icons/userPlus';
    import LogoRoti from "$assets/Logo-Roti.png"
</script>

<nav>
    <img src={LogoRoti} alt="Roti Logo">
    <ul>
        <li>
            <!-- svelte-ignore a11y-invalid-attribute -->
            <a href="#">
                <span>ADD TO CART</span>
                <Icon data="{shoppingCart}" scale={1.1}/>
            </a>
        </li>
        <li>
            <!-- svelte-ignore a11y-invalid-attribute -->
            <a href="#">
                <span>SIGN UP</span>
                <Icon data="{userPlus}" scale={1.1}/>
            </a>
        </li>
        <li>
            <!-- svelte-ignore a11y-invalid-attribute -->
            <a href="#">
                <span>LOG IN</span>
                <Icon data="{signIn}" scale={1.1}/>
            </a>
        </li>
    </ul>
</nav>

<style>
    nav {
        width: 100%;
        height: 3.5rem;
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 1rem 5rem;
        background-color: hsla(23, 36%, 25%, 0.5);
        backdrop-filter: blur(5px);
        position: sticky;
        top: 0;
    }

    nav > img {
        height: 2.5rem;
    }
    nav > ul {
        display: flex;
        align-items: center;
        list-style-type: none;
    }
    nav ul li {
        display: flex;
        align-items: center;
    }

    nav ul li a {
        color: #FEFEFE;
        font-weight: 700;
        display: flex;
        align-items: center;
        height: 3.5rem;
        padding: 0 1.5rem;
        transition: all 250ms ease-in-out;
        border-left: 0.1rem solid #FEFEFE;
    }
    nav ul li:nth-child(3) a {
        border-right: 0.1rem solid #FEFEFE;
    }
    nav ul li a:hover {
         background-color: hsla(21, 96%, 72%, 0.5);
    }
    nav ul li a span {
        padding-right: 0.5rem;
    }

</style>