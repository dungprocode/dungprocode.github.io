<DOCTYPE html>
    <html lang="th">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta charset="utf-8">
    <title>Nguyễn Trọng Dũng</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="https://pro.fontawesome.com/releases/v5.10.0/css/all.css">
    <!--img-->
    <link rel="shortcut icon"
        href="https://cdn.discordapp.com/attachments/933914501999394909/934834832918347817/-removebg-preview.png">
    <link rel="apple-touch-icon"
        href="https://cdn.discordapp.com/attachments/933914501999394909/934834832918347817/-removebg-preview.png">
    <link rel="apple-touch-icon-precomposed"
        href="https://cdn.discordapp.com/attachments/933914501999394909/934834832918347817/-removebg-preview.png">
    <!--end-->
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
            scroll-behavior: smooth;
        }

        section {
            padding: 100px;
        }

        .banner {
            position: relative;
            min-height: 100vh;
            background: url(https://thongtincanhan.hianime.repl.co/img/banner.jpg);
            background-size: cover;
            background-position: right;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .banner h2 {
            font-size: 3em;
            color: #fff;
            font-weight: 500;
            line-height: 1.5em;
        }

        .banner h2 span {
            font-size: 1.5em;
            font-weight: 700;
        }

        .banner h3 {
            font-size: 1.5em;
            color: #fff;
            font-weight: 500;
        }

        .btn {
            position: relative;
            background: #46449e;
            display: inline-block;
            color: #fff;
            margin-top: 20px;
            padding: 10px 30px;
            text-transform: uppercase;
            text-decoration: none;
            letter-spacing: 2px;
            font-weight: 500;
        }

        header {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            padding: 40px 100px;
            z-index: 1000;
            display: flex;
            justify-content: space-between;
            align-items: center;
            transition: 0.5s;
        }

        header.sticky {
            background: #fff;
            padding: 20px 100px;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.1);
        }

        header.sticky .logo {
            color: #111;
        }

        header .logo {
            color: #fff;
            font-size: 24px;
            text-transform: uppercase;
            text-decoration: none;
            font-weight: 700;
            letter-spacing: 2px;
        }

        header ul {
            position: relative;
            display: flex;
        }

        header ul li {
            position: relative;
            list-style: none;
        }

        header ul li a {
            position: relative;
            display: inline-block;
            margin: 0 15px;
            color: #fff;
            text-decoration: none;
        }

        header.sticky ul li a {
            color: #111;
        }

        .heading {
            width: 100%;
            text-align: center;
            margin-bottom: 30px;
            color: #111;
        }

        .heading h2 {
            font-weight: 600;
            font-size: 30px;
        }

        .content {
            display: flex;
            justify-content: space-between;
        }

        .contentBx h3 {
            font-size: 24px;
            margin-bottom: 10px;
        }

        .w50 {
            min-width: 50%;
        }

        img {
            max-width: 100%;
        }

        .services {
            background: #111;
        }

        .heading.white {
            color: #fff;
        }

        .services .content {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            flex-direction: row;
        }

        .services .content .servicesBx {
            padding: 40px 20px;
            background: #222;
            color: #fff;
            max-width: 340px;
            margin: 20px;
            text-align: center;
            transition: 0.5s;
        }

        .services .content .servicesBx:hover {
            background: #46449e;
        }

        .services .content .servicesBx img {
            max-width: 80px;
            filter: invert(1);
        }

        .services .content .servicesBx h2 {
            font-size: 20px;
            font-weight: 600;
        }

        .work .content {
            display: flex;
            justify-content: space-between;
            flex-wrap: wrap;
        }

        .work .content .workBx {
            width: 50%;
            padding: 20px;
        }

        .work .content .workBx img {
            max-width: 100%;
        }

        .testimonial {
            background: #f7f7f7;
        }

        .testimonial .content {
            display: flex;
            justify-content: space-between;
            flex-wrap: wrap;
        }

        .testimonial .content .testimonialBx {
            max-width: calc(50% - 40px);
            padding: 60px 40px;
            margin: 20px;
            background: #46449e;
        }

        .testimonial .content .testimonialBx p {
            color: #fff;
            font-style: italic;
            font-size: 16px;
            font-weight: 300;
        }

        .testimonial .content .testimonialBx h3 {
            margin-top: 40px;
            text-align: end;
            color: #fff;
            font-weight: 600;
            font-size: 20px;
            line-height: 1em;
        }

        .testimonial .content .testimonialBx h3 span {
            font-size: 14px;
            font-weight: 400;
        }

        .contact {
            background: #111;
        }

        .formBx {
            min-width: 60%;
        }

        .formBx form {
            display: flex;
            flex-direction: column;
        }

        .formBx form h3,
        .contactInfo h3 {
            color: #fff;
            font-size: 20px;
            font-weight: 500;
            margin-bottom: 10px;
        }

        .formBx form input,
        .formBx form textarea {
            margin-bottom: 20px;
            padding: 15px;
            font-size: 16px;
            border: none;
            outline: none;
            background: #222;
            color: #fff;
            resize: none;
        }

        .formBx form textarea {
            min-height: 200px;
        }

        .formBx form input::placeholder,
        .formBx form textarea::placeholder {
            color: #999;
        }

        .formBx form input[type="submit"] {
            max-width: 100px;
            background: #46449e;
            cursor: pointer;
            text-transform: uppercase;
            letter-spacing: 2px;
        }

        .contactInfo {
            min-width: 40%;
        }

        .contactInfoBox {
            position: relative;
        }

        .contactInfoBox .box {
            position: relative;
            padding: 20px 0;
            display: flex;
        }

        .contactInfoBox .box .icon {
            min-width: 40px;
            padding-top: 4px;
            color: #fff;
            display: flex;
            justify-content: center;
            align-items: flex-start;
            font-size: 24px;
        }

        .contactInfoBox .box .text {
            display: flex;
            margin-left: 20px;
            font-size: 16px;
            color: #fff;
            flex-direction: column;
            font-weight: 300;
        }

        .contactInfoBox .box .text h3 {
            font-weight: 500;
            color: #46449e;
            margin-bottom: 0;
        }

        .copyright {
            background: #000;
            color: #fff;
            text-align: center;
            padding: 10px;
        }

        /*Responsive - Phone view*/
        @media (max-width: 991px) {

            header,
            header.sticky {
                padding: 20px 50px;
                z-index: 1000;
            }

            .menu {
                position: fixed;
                top: 75px;
                left: -100%;
                display: block;
                padding: 100px 50px;
                text-align: center;
                width: 100%;
                height: 100vh;
                background: #fff;
                transition: 0.5s;
                z-index: 999;
                border-top: 1px solid rgba(0, 0, 0, 0.2);
            }

            .menu.active {
                left: 0;
            }

            header ul li a {
                color: #111;
                font-size: 24px;
                margin: 10px;
            }

            .toggle {
                width: 40px;
                height: 40px;
                background: url(img/menu.png);
                background-position: center;
                background-repeat: no-repeat;
                background-size: 30px;
                cursor: pointer;
            }

            .toggle.active {
                background: url(img/close.png);
                background-position: center;
                background-repeat: no-repeat;
                background-size: 25px;
                cursor: pointer;
            }

            header.sticky .toggle {
                filter: invert(1);
            }

            section {
                padding: 100px 50px;
            }

            .banner {
                padding: 150px 50px 100px;
            }

            .banner h2 {
                font-size: 1.5em;
            }

            .btm {
                margin-top: 10px;
                padding: 10px 20px;
                font-size: 16px;
            }

            .heading h2 {
                font-size: 24px;
            }

            .contentBx h3 {
                font-size: 20px;
            }

            .content {
                flex-direction: column;
            }

            .w50 {
                margin-bottom: 20px;
            }

            .services .content .servicesBx {
                margin: 10px;
            }

            .work .content .workBx {
                width: 100%;
                padding: 10px;
            }

            .testimonial .content .testimonialBx {
                max-width: calc(100% - 20px);
                padding: 40px 20px;
                margin: 10px;
                background: #46449e;
            }

            .testimonial .content .testimonialBx h3 {
                margin-top: 20px;
            }

            .contactInfo {
                margin: 20px 0;
            }
        }

        @media (max-width: 600px) {

            header,
            header.sticky {
                padding: 20px 20px;
            }

            .banner {
                padding: 150px 20px 100px;
            }

            section {
                padding: 100px 20px;
            }
        }
    </style>
    </head>

    <body>
        <header>
            <a href="#services" class="logo">Nguyễn Dũng</a>
            <div class="toggle" onclick="toggleMenu();"></div>
            <ul class="menu">
                <li><a href="#home" onclick="toggleMenu();">HOME</a></li>
                <li><a href="#about" onclick="toggleMenu();">ABOUT</a></li>
                <li><a href="#services" onclick="toggleMenu();">SERVICES</a></li>
                <li><a href="#work" onclick="toggleMenu();">WORK</a></li>
                <li><a href="#testimonial" onclick="toggleMenu();">FACEBOOK</a></li>
                <li><a href="#contact" onclick="toggleMenu();">CONTACT</a></li>
            </ul>
        </header>
        <section class="banner" id="home">

            <div class="textBx">
                <h2>dũng depzaii<br><span>Nguyen TRong Dung</span></h2>
                <h3>dũng blue </h3>
                <a href="#about" class="btn">ABOUT</a>
                <a href="https://www.facebook.com/nguyentrongdung37.NA/" class="btn">fACEBOOK</a>
                <a href="https://www.youtube.com/channel/UCPO173XLj8ItPvpHkHKKcfw" class="btn">YOUTUBE</a>
            </div>
        </section>
        <section class="about" id="about">
            <div class="heading">
                <h2>GIỚI THIỆU BẢN THÂN</h2>
            </div>
            <div class="content">
                <div class="contentBx w50">
                    <h3>Nguyễn Trọng Dũng</h3>
                    <!--Lorem is text in put-->
                    <p>Tên Đầy Đủ: Nguyễn <a href="https://www.facebook.com/nguyentrongdung37.NA/"
                            onclick="toggleMenu();">(nguyễn dũng)</a>
                        <br>
                        Ngày Tháng Năm Sinh:
                        <a href="https://www.facebook.com/nguyentrongdung37.NA/" onclick="toggleMenu();">05/03/2010</a>
                        <br>Nơi Ở: Nghệ An , Việt Nam
                        <br>Công Việc: Học sinh , Admin bot
                        <br>Sở Thích: Chơi Game, Nghe Nhạc,...
                        <br>Ước Mơ: Giàu
                        <br>Người yêu: chx có ny mấy pa ơi ( kiếm ny )
                        <br><br>Liên Hệ tại Facebook <a href="https://www.facebook.com/nguyentrongdung37.NA/">
                            https://www.facebook.com/nguyentrongdung37.NA/</a><br>
                    </p>
                    <img class="hoverZoomLink"
                        src="https://scontent.fvii1-1.fna.fbcdn.net/v/t39.30808-1/297251644_124396680320075_7958584249139765172_n.jpg?stp=c0.78.200.200a_dst-jpg_p200x200&_nc_cat=102&ccb=1-7&_nc_sid=f67be1&_nc_ohc=FYNKv74o1m4AX9beK7T&_nc_ht=scontent.fvii1-1.fna&oh=00_AfB-FdOUNbCMBoMaCwHUIfuXQMrePxV1FjUfzaHklz4BjQ&oe=63988572">

                </div>
                <div class="w50">
                    <img src="https://thongtincanhan.hianime.repl.co/img/img1.gif" class="img">
                </div>
            </div>
        </section>
        <section class="services" id="services">
            <div class="heading white">
                <h2>CONTACT</h2>
                <p>Nguyễn TRọng Dũng</p>
            </div>
            <a href="https://www.facebook.com/nguyentrongdung37.NA/">
            </a>
            <div class="content"><a href="https://www.facebook.com/nguyentrongdung37.NA/">
                </a>
                <div class="servicesBx"><a href="https://www.facebook.com/nguyentrongdung37.NA/">
                        <img src="https://thongtincanhan.hianime.repl.co/img/fb.png">
                    </a>
                    <h2>Facebook</h2>
                    <p>Nguyễn TRọng Dũng</p>
                </div>
                <a href="https://www.tiktok.com/@nggphuongvy605">
                    <div class="servicesBx">
                        <img src="https://thongtincanhan.hianime.repl.co/img/tiktok.jpg">
                        <h2>TikTok</h2>
                        <p>Nguyễn Dũng</p>
                    </div>
                </a><a href="https://www.youtube.com/channel/UCPO173XLj8ItPvpHkHKKcfw">
                    <div class="servicesBx">
                        <img src="https://thongtincanhan.hianime.repl.co/img/ytb.png">
                        <h2>Youtube</h2>
                        <p>Nguyễn Dũng</p>
                    </div>

                </a>
            </div>
        </section><a href="https://www.youtube.com/channel/UCPO173XLj8ItPvpHkHKKcfw">
        </a>
        <section class="work" id="work"><a href="https://www.youtube.com/channel/UCPO173XLj8ItPvpHkHKKcfw">
                <div class="heading">
                    <h2>Mạng Xã Hội</h2>
                    <p>Nguyễn Dũng</p>
                </div>
            </a>
            <div class="content"><a href="https://www.youtube.com/channel/UCPO173XLj8ItPvpHkHKKcfw">
                </a>
                <div class="workBx"><a href="https://www.youtube.com/channel/UCPO173XLj8ItPvpHkHKKcfw">
                    </a><a href="https://www.facebook.com/nguyentrongdung37.NA/">
                        <img src="https://thongtincanhan.hianime.repl.co/img/fb.png">
                    </a>
                </div>
                <div class="workBx">
                    <a href="https://www.youtube.com/channel/UCPO173XLj8ItPvpHkHKKcfw">
                        <img src="https://thongtincanhan.hianime.repl.co/img/ytb.png">
                    </a>
                </div>
                <div class="workBx">
                    <a href="https://www.facebook.com/messages/t/100082492307716">
                        <img src="https://thongtincanhan.hianime.repl.co/img/mes.jpg">
                    </a>
                </div>
                <div class="workBx">
                    <a href="https://www.tiktok.com/@nggphuongvy605">
                        <img src="https://thongtincanhan.hianime.repl.co/img/tiktok.jpg">
                    </a>
                </div>
            </div>
            <div class="heading">
                <a href="#" class="btn">HOME</a>
            </div>
        </section>
        <section class="testimonial" id="testimonial">
            <div class="heading">
                <h2>Liên Hệ | SUPPORT</h2>
                <p>𝗖𝗼𝗽𝘆𝗿𝗶𝗴𝗵𝘁 Nguyen Trong Dung</p>
            </div>
            <div class="content">
                <div class="testimonialBx">
                    <p>Gmail: dn4831627@Gmail.com
                        <br><br>Số Điện Thoại: 0362385831
                        <br>Github: nguyendung5310
                        <br><br><br><br>𝗖𝗼𝗽𝘆𝗿𝗶𝗴𝗵𝘁: Nguyen Trong Dung
                    </p>
                    <h3><a href="https://dsc.gg/nomyen4" class="btn">Nguyen Dung| Support Bot</a><br><span>Liên Hệ Zalo
                            : 0362385831</span>
                    </h3>

                </div>
            </div>
        </section>
        <section class="contact" id="contact">
            <div class="heading">
                <h2></h2>
                <p></p>
            </div>
            <div class="content">
                <div class="contactInfo">
                    <h3>CONTACT</h3>
                    <div class="contactInfoBox">
                        <div class="box">
                            <div class="icon">
                                <i class="fab fa-discord"></i>
                            </div>
                            <div class="text">
                                <h3>Discord</h3>
                                <p>- <a href="https://discord.com/channels/@me" class="btn">DISCORD</a>
                                </p>
                            </div>
                        </div>
                        <div class="box">
                            <div class="icon">
                                <i class="fab fa-facebook"></i>
                            </div>
                            <div class="text">
                                <h3>FaceBook</h3>
                                <p>- <a href="https://www.facebook.com/nguyentrongdung37.NA/" class="btn">FACEBOOK</a>
                                </p>
                            </div>
                        </div>
                        <div class="box">
                            <div class="icon">
                                <i class="fas fa-envelope"></i>
                            </div>
                            <div class="text">
                                <h3>Email</h3>
                                <p>dn4831627@gmail.com</p>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="formBx">
                    <form>
                        <h3>Lời Nhắn</h3>
                        <input type="text" class="" placeholder="text">
                        <input type="email" class="" placeholder="email">
                        <textarea placeholder="Nội Dung"></textarea>
                        <input type="submit" value="Gửi">
                    </form>
                </div>
            </div>
        </section>
        <div class="copyright">
            <p>©copyright: Nguyễn Trọng Dũng</p>
        </div>
        <style>
            html,
            body {
                cursor: url("https://i.imgur.com/5v5M8gh.png"), auto;
            }

            a:hover {
                cursor: url("https://i.imgur.com/IXULuQ1.png"), auto;
            }
        </style>
        <script type="text/javascript">
            window.addEventListener('scroll', function () {
                var header = document.querySelector('header');
                header.classList.toggle('sticky', window.scrollY > 0);
            });

            function toggleMenu() {
                var menuToggle = document.querySelector('.toggle');
                var menu = document.querySelector('.menu');
                menuToggle.classList.toggle('active')
                menu.classList.toggle('active')
            }
        </script>


    </body>
    <div style="position: absolute; top: 0px; display: block !important;"></div>

    </html>
