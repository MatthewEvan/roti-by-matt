<script lang="ts">
    import Icon from "svelte-awesome";
    // Icons Needed
    import externalLink from 'svelte-awesome/icons/externalLink';
    import shoppingCart from 'svelte-awesome/icons/shoppingCart';
    import instagram from 'svelte-awesome/icons/instagram'
    import facebookSquare from 'svelte-awesome/icons/facebookSquare';
    import githubSquare from 'svelte-awesome/icons/githubSquare'


    //Importing Images
    import BGHeader from "$assets/Background-Header.png";
    import Image1 from "$assets/Image-1.jpg"
    import Image2 from "$assets/Image-2.jpg"
    import Image3 from "$assets/Image-3.jpg"
    import Image4 from "$assets/Image-4.jpg"
    import LogoRoti from "$assets/Logo-Roti.png"
    import LogoRotiInverted from "$assets/Logo-Roti-Inverted.png"
</script>

<div class="main-page">
    <section id="header" style="background-image: url({BGHeader})">
        <img src={LogoRoti} alt="Logo Roti" class="logo-roti-header">
        <h1>
            <span>Melayani</span> dan 
            <span>Menyediakan</span> Berbagai <span>
            Roti Hangat</span> Langsung dari <span>Oven</span>
        </h1>
        <div class="image-showcase-header">
            <img src={Image1} alt="Produk Roti 1">
            <img src={Image2} alt="Produk Roti 2">
            <img src={Image3} alt="Produk Roti 3">
        </div>
        <h2>Roti yang hangat dan harum, dipadukan dengan kelezatan yang telah teruji kualitasnya. Roti-roti yang bervariasi sesuai keinginandan permintaan berbagai pelanggan kami. Hanya tersedia di Roti</h2>
        <div class="cta-buttons">
            <!-- svelte-ignore a11y-invalid-attribute -->
            <a href="#" class="pesan-sekarang">
                <span>PESAN SEKARANG</span>
                <Icon data="{externalLink}" scale={1.2}/>
            </a>
            <!-- svelte-ignore a11y-invalid-attribute -->
            <a href="#" class="tambahkan-keranjang">
                <span>LIHAT KERANJANG</span>
                <Icon data="{shoppingCart}" scale={1.2}/>
            </a>
        </div>
    </section>
    <section id="logo-showcase-carousel">
        <p>The next section is coming through</p>
    </section>   
</div>

<style>
    #header {
        padding: 3rem 0;
        display: flex;
        flex-direction: column;
        align-items: center;
        gap: 1.25rem;
        background-size: 100vw;
        background-position: top;
    }
    #header .logo-roti-header {
        width: 10vw;
    }

    #header > h1 {
        font-family: "Bricolage Grotesque", display;
        font-size: 3rem;
        font-weight: 700;
        text-align: center;
        text-wrap: balance;
    }
    #header > h1 span {
        font-family: "Bricolage Grotesque", display;
        font-size: 3rem;
        font-weight: 700;
    }
    #header > h1 span:nth-child(1) {
        text-decoration: solid underline #D5754E 5px;
    }
    #header > h1 span:nth-child(2) {
        text-decoration: solid underline #FFC113 5px;
    }
    #header > h1 span:nth-child(3) {
        text-decoration: solid underline #6BBB5F 5px;
    }
    #header > h1 span:nth-child(4) {
        text-decoration: solid underline #5F6EBB 5px;
    }

    .image-showcase-header {
        display: flex;
        align-items: center;
        gap: 1.25rem;
        padding-top: 1.25rem;
        border-top: 0.2rem solid #FEFEFE;
    }
    .image-showcase-header > img {
        width: 13vw;
        aspect-ratio: 5/3;
        object-fit: cover;
        border-radius: 0.25rem;
        opacity: 0.8;
        transition: all 350ms ease-in-out;
    }
    .image-showcase-header > img:hover {
        scale: 1.1;
        opacity: 1;
    }

    #header > h2 {
        font-size: 1.3rem;
        font-weight: 500;
        text-align: center;
        text-wrap: balance;
    }

    .cta-buttons {
        display: flex;
        align-items: center;
        gap: 1.5rem;
    }

    .pesan-sekarang {
        background: linear-gradient(120deg, #A6511F, #F2AF5C);
        padding: 1rem 2rem;
        border-radius: 0.5rem;
        transition: all 350ms ease-in-out;
        display: flex;
        align-items: center;
        justify-content: center;
        gap: 0.75rem;
        color: #FEFEFE;
    }
    .pesan-sekarang:hover {
        background: linear-gradient(165deg, #A6511F, #F2AF5C);
    }
    .pesan-sekarang span {
        font-weight: 500;
        font-size: 1.2rem;
    }

    .tambahkan-keranjang {
        border: 0.2rem solid #F2AF5C;
        padding: 1rem 2rem;
        border-radius: 0.5rem;
        transition: all 350ms ease-in-out;
        display: flex;
        align-items: center;
        justify-content: center;
        gap: 0.75rem;
        color: #FEFEFE;
    }
    .tambahkan-keranjang:hover {
        background: #ad704d;
    }
    .tambahkan-keranjang span {
        font-weight: 500;
        font-size: 1.2rem;
    }

</style>