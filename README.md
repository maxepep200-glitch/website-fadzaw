<!DOCTYPE html>
<html lang="id">

<head>

    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Fadza — Portfolio</title>

    <style>

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            background: #0b0b0d;
            color: #f5f5f5;
            font-family: Arial, Helvetica, sans-serif;
            line-height: 1.6;
        }


        /* =========================
           NAVBAR
        ========================= */

        nav {
            position: fixed;
            top: 0;
            width: 100%;

            padding: 20px 7%;

            display: flex;
            justify-content: space-between;
            align-items: center;

            background: rgba(11, 11, 13, 0.75);
            backdrop-filter: blur(15px);

            z-index: 100;
        }

        .logo {
            font-size: 22px;
            font-weight: 800;
            letter-spacing: -1px;
        }

        nav a {
            color: #888;
            text-decoration: none;

            margin-left: 25px;

            font-size: 14px;

            transition: 0.3s;
        }

        nav a:hover {
            color: white;
        }


        /* =========================
           HERO
        ========================= */

        .hero {
            min-height: 100vh;

            padding: 150px 7% 80px;

            display: flex;
            align-items: center;
        }

        .hero-content {
            max-width: 850px;
        }

        .tag {
            color: #777;

            font-size: 13px;

            letter-spacing: 3px;

            margin-bottom: 20px;
        }

        h1 {
            font-size: clamp(60px, 10vw, 125px);

            line-height: 0.9;

            letter-spacing: -7px;

            margin-bottom: 30px;
        }

        h1 span {
            color: #666;
        }

        .description {
            max-width: 600px;

            color: #999;

            font-size: 18px;

            margin-bottom: 35px;
        }


        /* =========================
           BUTTON
        ========================= */

        .button {
            display: inline-block;

            padding: 13px 23px;

            background: white;
            color: black;

            border-radius: 30px;

            text-decoration: none;

            font-weight: bold;
            font-size: 14px;

            transition: 0.3s;
        }

        .button:hover {
            transform: translateY(-3px);
        }


        /* =========================
           SECTION
        ========================= */

        section {
            padding: 110px 7%;
        }

        .section-title {
            font-size: 45px;

            letter-spacing: -2px;

            margin-bottom: 45px;
        }


        /* =========================
           ABOUT
        ========================= */

        .about {
            display: grid;

            grid-template-columns: 1fr 1fr;

            gap: 50px;
        }

        .about p {
            color: #999;

            font-size: 18px;
        }

        .skills {
            display: flex;

            flex-wrap: wrap;

            gap: 12px;
        }

        .skill {
            border: 1px solid #29292d;

            padding: 11px 17px;

            border-radius: 30px;

            color: #ccc;
        }


        /* =========================
           PROJECTS
        ========================= */

        .projects {
            display: grid;

            grid-template-columns: repeat(2, 1fr);

            gap: 20px;
        }

        .project {
            position: relative;

            height: 320px;

            overflow: hidden;

            border: 1px solid #252529;

            border-radius: 22px;

            background: #151518;

            transition: 0.3s;
        }

        .project:hover {
            transform: translateY(-7px);

            border-color: #555;
        }

        .project img {
            width: 100%;
            height: 100%;

            object-fit: cover;

            display: block;

            transition: 0.4s;
        }

        .project:hover img {
            transform: scale(1.05);
        }

        .project-info {
            position: absolute;

            bottom: 0;
            left: 0;

            width: 100%;

            padding: 50px 25px 25px;

            background: linear-gradient(
                transparent,
                rgba(0, 0, 0, 0.95)
            );
        }

        .project-info small {
            color: #aaa;
        }

        .project-info h3 {
            font-size: 25px;
        }

        .project-info p {
            color: #bbb;

            font-size: 14px;
        }


        /* =========================
           CONTACT
        ========================= */

        .contact {
            border-top: 1px solid #222;
        }

        .contact p {
            color: #888;

            margin-bottom: 25px;
        }


        /* =========================
           FOOTER
        ========================= */

        footer {
            padding: 30px 7%;

            color: #555;

            border-top: 1px solid #222;

            font-size: 13px;
        }


        /* =========================
           MOBILE
        ========================= */

        @media (max-width: 700px) {

            nav {
                padding: 18px 5%;
            }

            nav div:last-child {
                display: none;
            }

            .hero {
                padding: 130px 5% 70px;
            }

            h1 {
                letter-spacing: -4px;
            }

            section {
                padding: 80px 5%;
            }

            .about,
            .projects {
                grid-template-columns: 1fr;
            }

            .project {
                height: 280px;
            }

        }

    </style>

</head>


<body>


    <!-- =========================
         NAVBAR
    ========================= -->

    <nav>

        <div class="logo">
            FADZA.
        </div>

        <div>

            <a href="#about">
                About
            </a>

            <a href="#work">
                Work
            </a>

            <a href="#contact">
                Contact
            </a>

        </div>

    </nav>



    <!-- =========================
         HERO
    ========================= -->

    <header class="hero">

        <div class="hero-content">

            <div class="tag">
                CREATIVE DESIGNER / EDITOR
            </div>

            <h1>

                Making ideas
                <br>

                <span>look better.</span>

            </h1>

            <p class="description">

                Portfolio personal untuk menampilkan
                karya desain, editing, fotografi,
                dan berbagai project kreatif.

            </p>

            <a
                class="button"
                href="#work"
            >

                Lihat Karya ↓

            </a>

        </div>

    </header>



    <!-- =========================
         ABOUT
    ========================= -->

    <section id="about">

        <h2 class="section-title">
            About me.
        </h2>


        <div class="about">

            <p>

                Halo, aku Fadza.

                Aku suka mengeksplorasi dunia visual
                dan membuat sesuatu yang sederhana
                terlihat lebih menarik.

            </p>


            <div class="skills">

                <div class="skill">
                    Graphic Design
                </div>

                <div class="skill">
                    Photo Editing
                </div>

                <div class="skill">
                    Photography
                </div>

                <div class="skill">
                    Video Editing
                </div>

                <div class="skill">
                    GFX
                </div>

            </div>

        </div>

    </section>



    <!-- =========================
         PROJECTS
    ========================= -->

    <section id="work">

        <h2 class="section-title">
            Selected work.
        </h2>


        <div class="projects">


            <!-- PROJECT 1 -->

            <div class="project">

                <img
                    src="images/poster.jpg"
                    alt="Poster Design"
                >

                <div class="project-info">

                    <small>
                        01 / DESIGN
                    </small>

                    <h3>
                          Design
                    </h3>

                    <p>
                        Poster event dengan
                        konsep visual minimalis.
                    </p>

                </div>

            </div>



            <!-- PROJECT 2 -->

            <div class="project">

                <img
                    src="images/photo.jpg"
                    alt="Photo Editing"
                >

                <div class="project-info">

                    <small>
                        02 / PHOTO
                    </small>

                    <h3>
                        Photo Editing
                    </h3>

                    <p>
                        Eksplorasi warna dan
                        editing fotografi.
                    </p>

                </div>

            </div>



            <!-- PROJECT 3 -->

            <div class="project">

                <img
                    src="images/esport.jpg"
                    alt="Esports Project"
                >

                <div class="project-info">

                    <small>
                        03 / ESPORT
                    </small>

                    <h3>
                        Esports Project
                    </h3>

                    <p>
                        Visual design untuk
                        project esports.
                    </p>

                </div>

            </div>



            <!-- PROJECT 4 -->

            <div class="project">

                <img
                    src="images/creative.jpg"
                    alt="Creative Project"
                >

                <div class="project-info">

                    <small>
                        04 / CREATIVE
                    </small>

                    <h3>
                        Creative Work
                    </h3>

                    <p>
                        Eksperimen visual dan
                        berbagai karya kreatif.
                    </p>

                </div>

            </div>


        </div>

    </section>



    <!-- =========================
         CONTACT
    ========================= -->

    <section
        id="contact"
        class="contact"
    >

        <h2 class="section-title">
            Let's create.
        </h2>

        <p>
            Punya project atau sekadar
            ingin ngobrol?
        </p>


        <!-- GANTI NOMOR DI SINI -->

        <a
            class="button"
            href="https://wa.me/6281234567890"
            target="_blank"
        >

            Contact Me

        </a>

    </section>



    <!-- =========================
         FOOTER
    ========================= -->

    <footer>

        © 2026 Fadza.
        Built with curiosity.

    </footer>


</body>

</html>
