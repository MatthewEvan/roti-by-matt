<script lang="ts">
    import Icon from "svelte-awesome";
    // Icons Needed
    import externalLink from 'svelte-awesome/icons/externalLink';
    import shoppingCart from 'svelte-awesome/icons/shoppingCart';
    import instagram from 'svelte-awesome/icons/instagram'
    import facebookSquare from 'svelte-awesome/icons/facebookSquare';
    import githubSquare from 'svelte-awesome/icons/githubSquare';
    import star from 'svelte-awesome/icons/star';


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
            Roti Hangat</span> Langsung Dipanggang dari <span>Oven</span>
        </h1>
        <div class="image-showcase-header">
            <img src={Image1} alt="Produk Roti 1">
            <img src={Image2} alt="Produk Roti 2">
            <img src={Image3} alt="Produk Roti 3">
        </div>
        <h2>Roti yang hangat dan harum, dipadukan dengan kelezatan dan berbagai bahan yang telah teruji kualitasnya. Roti-roti yang bervariasi sesuai keinginan dan permintaan berbagai pelanggan kami. Hanya tersedia di Roti</h2>
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
    <section id="mengapa-kami">
        <h2>Mengapa Kami ?</h2>
        <ul class="poin-mengapa-kami">
            <li>
                <h3>1. Kualitas Terjamin</h3>
                <p>Semua bahan yang kami gunakan adalah bahan yang berkualitas dan telah teruji kebersihan serta keamanannya untuk dikonsumsi</p>
            </li>
            <li>
                <h3>2. Baru Dipanggang</h3>
                <p>Roti-roti yang kami sajikan merupakan roti yang baru dipanggang dari oven dan disajikan langsung dalam keadaan hangat</p>
            </li>
            <li>
                <h3>3. Lezat & Bervariasi</h3>
                <p>Kami menyediakan berbagai jenis roti sesuai dengan keinginan pelanggan yang dipadukan dengan kelezatan dan aroma yang khas</p>
            </li>
        </ul>
    </section>
    <section id="produk-unggulan">
        <div class="produk-tile">
            <div class="produk-header">
                <h4>Produk Unggulan Kami</h4>
                <h3>Roti Boy</h3>
                <div class="produk-ratings">
                    <div class="stars-icon">
                        <Icon data="{star}" scale={1.1} style="color: #FFF844"/>
                        <Icon data="{star}" scale={1.1} style="color: #FFF844"/>
                        <Icon data="{star}" scale={1.1} style="color: #FFF844"/>
                        <Icon data="{star}" scale={1.1} style="color: #FFF844"/>
                        <Icon data="{star}" scale={1.1} style="color: #FFF844"/>
                        <span>(152)</span>
                    </div>
                    <span>&#x2022;</span>
                    <div class="produk-penjualan">
                        <Icon data="{shoppingCart}"/>
                        <span>(1284+)</span>
                    </div>
                </div>
            </div>
            <p class="produk-desc">Roti panggang hangat dengan isian krim rasa kopi yang dilengkapi dengan topping berupa krim cokelat yang manis pada bagian atas roti</p>
        </div>
        <img src={Image4} alt="Produk Andalan Kami: RotiBoy">
    </section>
    <section id="produk-lainnya">
        <h3>Produk Lainnya</h3>
        <div class="produk-lainnya-images">
            <div>
                <img src="https://images.unsplash.com/photo-1509440159596-0249088772ff?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8Mnx8YnJlYWR8ZW58MHx8MHx8fDA%3D&auto=format&fit=crop&w=600&q=60" alt="Produk 1">
                <img src="https://images.unsplash.com/photo-1530610476181-d83430b64dcd?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8Mnx8Y3JvaXNzYW50fGVufDB8fDB8fHww&auto=format&fit=crop&w=600&q=60" alt="Produk 2">
            </div>
            <div>
                <img src="https://images.unsplash.com/photo-1528735602780-2552fd46c7af?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8Mnx8c2FuZHdpY2h8ZW58MHx8MHx8fDA%3D&auto=format&fit=crop&w=600&q=60" alt="Produk 3">
                <img src="https://images.unsplash.com/photo-1550507992-eb63ffee0847?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8MTZ8fHNhbmR3aWNofGVufDB8fDB8fHww&auto=format&fit=crop&w=600&q=60" alt="Produk 4">
            </div>
        </div>
    </section>
    <section id="footer-section">
        <p class="footer-desc">Roti adalah merek tidak resmi dan situs web ini hanyalah prototipe untuk mempromosikan beberapa produk roti dengan cara yang lebih modern daripada melakukannya secara tradisional. Dibuat hanya untuk teks prosedur kompleks. Semua foto dan video diambil secara manual atau dari Unsplash</p>
        <div class="footer-logos">
            <img src={LogoRoti} alt="Roti Logo">
            <img src={LogoRotiInverted} alt="Roti Logo Inverted">
        </div>
        <span class="social-logos">
            <a href="https://github.com/MatthewEvan" target="_blank"><Icon data="{githubSquare}" scale={2} class="github-logo"/></a>
            <a href="https://www.instagram.com/evano_888/" target="_blank"><Icon data="{instagram}" scale={2} class="instagram-logo"/></a>
        </span>
        <p class="trademark">Made by Matthew &#x2022; 2023</p>
    </section>
</div>

<style>
    .main-page {
        display: flex;
        flex-direction: column;
        align-items: center;
        gap: 2rem;
    }
    #header {
        padding: 6rem 6rem 3rem;
        display: flex;
        flex-direction: column;
        align-items: center;
        gap: 1.25rem;
        background-size: cover;
        background-position: top;
        background-repeat: no-repeat;
    }
    #header .logo-roti-header {
        width: 10vw;
    }

    #header > h1 {
        font-family: "Bricolage Grotesque", sans-serif;
        font-size: 3rem;
        font-weight: 700;
        text-align: center;
        text-wrap: balance;
    }
    #header > h1 span {
        font-family: "Bricolage Grotesque", sans-serif;
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
        width: 18vw;
        aspect-ratio: 5/2.5;
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


    /* Mengapa Kami Section */
    /* Mengapa Kami Section */
    /* Mengapa Kami Section */
    #mengapa-kami {
        margin-inline: 6rem;
        display: flex;
        flex-direction: column;
        align-items: center;
        gap: 1rem;
    }
    #mengapa-kami > h2 {
        font-family: "Bricolage Grotesque", sans-serif;
        font-size: 3.5rem;
        font-weight: 700;
    }
    .poin-mengapa-kami {
        display: flex;
        align-items: strecth;
        gap: 2rem;
        list-style-type: none;
    }
    .poin-mengapa-kami li {
        flex: 1;
        background-color: hsl(43, 55%, 66%);
        padding: 1rem 1.5rem;
        border-radius: 0.5rem;
        display: flex;
        flex-direction: column;
        align-items: start;
        gap: 0.5rem;
    }
    .poin-mengapa-kami li:nth-child(2) {
        background-color: hsl(46, 100%, 91%);
    }
    .poin-mengapa-kami li h3 {
        font-size: 2rem;
        font-family: "Bricolage Grotesque", sans-serif;
        font-weight: 700;
        color: #2F241D;
    }
    .poin-mengapa-kami li p {
        font-size: 1.35rem;
        color: #2F241D;
    }

    /* PRODUK UNGGULAN */
    /* PRODUK UNGGULAN */
    /* PRODUK UNGGULAN */
    #produk-unggulan {
        margin: 1rem 6rem;
        display: flex;
        align-items: center;
        gap: 2rem;
    }
    #produk-unggulan > img {
        width: 45vw;
        aspect-ratio: 2/1;
        object-fit: cover;
        object-position: center;
        border-radius: 2rem;
    }

    .produk-tile {
        display: flex;
        flex-direction: column;
        align-items: start;
        gap: 1rem;
    }
    .produk-tile p {
        font-size: 1.2rem;
        font-weight: 500;
        text-wrap: balance;
    }

    .produk-header {
        display: flex;
        flex-direction: column;
        align-items: start;
    }
    .produk-header > h4 {
        font-size: 1.35rem;
        font-weight: 700;
    }
    .produk-header > h3 {
        font-size: 5rem;
        font-family: "Bricolage Grotesque", sans-serif;
        letter-spacing: 2px;
    }
    .produk-ratings {
        display: flex;
        align-items: center;
        gap: 0.5rem;
    }
    .stars-icon {
        display: flex;
        align-items: center;
        gap: 0.2rem;
    }
    .stars-icon span {
        font-size: 1.15rem;
        padding-left: 0.5rem;
    }

    .produk-penjualan {
        display: flex;
        align-items: center;
        gap: 0.5rem;
    }
    .produk-penjualan span {
        font-size: 1.15rem;
    }

    /* PRODUK LAINNYA */
    /* PRODUK LAINNYA */
    /* PRODUK LAINNYA */
    #produk-lainnya {
        display: flex;
        flex-direction: column;
        align-items: center;
        gap: 1.5rem;
        margin: 1rem 5rem;
    }
    #produk-lainnya h3 {
        font-size: 3rem;
        font-family: "Bricolage Grotesque", sans-serif;
        font-weight: 700;
    }
    .produk-lainnya-images,
    .produk-lainnya-images div {
        display: flex;
        align-items: center;
        gap: 1.5rem;
    }
    .produk-lainnya-images div img {
        width: 20vw;
        aspect-ratio: 3/2;
        object-fit: cover;
        object-position: center;
        border-radius: 0.25rem;
        opacity: 0.85;
        transition: all 350ms ease-in-out;
    }
    .produk-lainnya-images div img:hover {
        opacity: 1;
        scale: 1.1;
    }

    /* FOOTER */
    /* FOOTER */
    /* FOOTER */
    #footer-section {
        padding: 2rem 6rem 1rem;
        background-color: hsl(23, 21%, 7%);
        display: flex;
        flex-direction: column;
        align-items: center;
        gap: 1rem;
    }
    #footer-section > p {
        text-wrap: balance;
        font-size: 1.125rem;
        color: #CCCCCC;
        text-align: center;
    }
    .footer-logos {
        display: flex;
        align-items: center;
        gap: 1rem;
        margin-bottom: 0.75rem;
    }
    #footer-section .footer-logos img {
        width: 5rem;
    }
    .social-logos {
        display: flex;
        flex-direction: row;
        align-items: center;
        gap: 0.5rem;
    }
    .social-logos a {
        color: #CCCCCC;
        transition: all 350ms ease-in-out
    }
    .social-logos a:hover, .social-logos a:active{
        color: #FEFEFE;
    }

    /* RESPONSIVE CODE */
    /* RESPONSIVE CODE */
    /* RESPONSIVE CODE */
    @media screen and (max-width: 1024px) {
        #header {
            padding: 6rem 4rem 3rem;
        }
    }
    @media screen and (max-width: 768px) {
        #header {
            padding: 6rem 2rem 3rem;
        }
        .image-showcase-header {
            flex-direction: column;
        }
        .image-showcase-header > img {
            width: 50vw;
            aspect-ratio: 5/1.75;
            border-radius: 0.5rem;
        }
        .cta-buttons {
            flex-direction: column;
        }

        /* MENGAPA KAMI */
        #mengapa-kami {
            margin-inline: 3rem;
        }
        .poin-mengapa-kami {
            flex-direction: column
        }

        /* PRODUK UNGGULAN KAMI */
        #produk-unggulan {
            flex-direction: column;
            margin: 1rem 3rem;
        }
        #produk-unggulan > img {
            width: 80vw;
            aspect-ratio: 2/0.75
        }
        .produk-tile {
            flex-direction: row;
            padding: 0 4rem 0;
            align-items: center;
        }
        .produk-header {
            flex: 1;
        }
        .produk-tile > p {
            flex: 1;
        }
        .produk-header > h3 {
            font-size: 3.5rem;
        }

        /* PRODUK LAINNYA  */
        #produk-lainnya {
            margin: 1rem 3rem;
        }
        .produk-lainnya-images {
            flex-direction: column;
        }
        .produk-lainnya-images div img {
            width: 40vw;
        }
    }

    @media screen and (max-width: 640px) {
        /* HEADER HEADER  */
        #header .logo-roti-header {
            width: 20vw;
        }
        /* PRODUK UNGGULAN KAMI */
        .produk-tile {
            flex-direction: column;
            padding: 0 2rem 0;
            align-items: start;
        }
        #produk-unggulan > img {
            aspect-ratio: 2/1.25
        }
        .produk-header .produk-ratings {
            flex-direction: column;
            align-items: start;
        }
        .produk-ratings > span {
            display: none;
        }

        /* PRODUK LAINNYA  */
        .produk-lainnya-images div {
            flex-direction: column;
        }
        .produk-lainnya-images div img {
            width: 75vw;
            border-radius: 0.75rem;
            aspect-ratio: 2/1;
        }
    }
</style>