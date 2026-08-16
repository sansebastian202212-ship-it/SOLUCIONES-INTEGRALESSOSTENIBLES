<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Soluciones Integrales Sostenibles | Limpieza y Mantenimiento</title>

<meta name="description"
content="Soluciones Integrales Sostenibles. Limpieza profesional, mantenimiento, limpieza de placas fotovoltaicas, cubiertas industriales y asesoramiento profesional.">

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&family=Montserrat:wght@500;600;700;800&display=swap" rel="stylesheet">

<style>

/* =========================================================
   VARIABLES
========================================================= */

:root{
    --azul-agua:#256d7b;
    --verde-opalo:#015d52;
    --turquesa-menta:#497e76;
    --genciana:#2a6478;
    --azul-turquesa:#3f888f;

    --verde-claro:#7aaa45;
    --blanco:#ffffff;
    --gris:#f4f8f7;
    --gris-texto:#5d6b69;
    --negro:#123330;

    --sombra:0 15px 45px rgba(1,93,82,.12);
    --radio:24px;
}

/* =========================================================
   RESET
========================================================= */

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

html{
    scroll-behavior:smooth;
}

body{
    font-family:"Inter",sans-serif;
    color:var(--negro);
    background:#fff;
    overflow-x:hidden;
}

img{
    max-width:100%;
    display:block;
}

button,
input,
textarea,
select{
    font-family:inherit;
}

a{
    text-decoration:none;
    color:inherit;
}

.container{
    width:min(1180px,92%);
    margin:auto;
}

/* =========================================================
   HEADER
========================================================= */

header{
    position:fixed;
    width:100%;
    top:0;
    left:0;
    z-index:1000;
    transition:.3s;
}

header.scrolled{
    background:rgba(255,255,255,.94);
    backdrop-filter:blur(15px);
    box-shadow:0 5px 25px rgba(0,0,0,.08);
}

.navbar{
    height:82px;
    display:flex;
    align-items:center;
    justify-content:space-between;
}

.logo{
    display:flex;
    align-items:center;
    gap:10px;
}

.logo-symbol{
    width:49px;
    height:49px;
    border:5px solid var(--verde-opalo);
    border-radius:50%;
    position:relative;
    transform:rotate(-20deg);
}

.logo-symbol::after{
    content:"";
    position:absolute;
    width:25px;
    height:13px;
    background:#65a934;
    border-radius:100% 0 100% 0;
    right:-7px;
    bottom:4px;
    transform:rotate(-20deg);
}

.logo-text{
    line-height:1;
}

.logo-text strong{
    display:block;
    font-family:"Montserrat";
    font-size:14px;
    letter-spacing:1.3px;
    color:var(--verde-opalo);
}

.logo-text span{
    display:block;
    font-size:10px;
    letter-spacing:3px;
    color:#6a963b;
    margin-top:5px;
}

.nav-links{
    display:flex;
    align-items:center;
    gap:28px;
    font-size:14px;
    font-weight:600;
}

.nav-links a{
    transition:.3s;
}

.nav-links a:hover{
    color:var(--verde-opalo);
}

.nav-actions{
    display:flex;
    gap:10px;
}

.btn{
    border:none;
    cursor:pointer;
    padding:14px 22px;
    border-radius:50px;
    font-weight:700;
    display:inline-flex;
    align-items:center;
    justify-content:center;
    gap:9px;
    transition:.3s;
}

.btn-primary{
    background:var(--verde-opalo);
    color:white;
    box-shadow:0 8px 25px rgba(1,93,82,.22);
}

.btn-primary:hover{
    transform:translateY(-3px);
    background:#00483f;
}

.btn-outline{
    border:1.5px solid var(--verde-opalo);
    color:var(--verde-opalo);
    background:white;
}

.btn-outline:hover{
    background:var(--verde-opalo);
    color:white;
}

.mobile-menu{
    display:none;
    font-size:25px;
    cursor:pointer;
}

/* =========================================================
   HERO
========================================================= */

.hero{
    min-height:760px;
    padding-top:120px;
    position:relative;
    overflow:hidden;
}

.hero::before{
    content:"";
    position:absolute;
    width:700px;
    height:700px;
    background:#eef8f5;
    border-radius:50%;
    top:-250px;
    left:-300px;
    z-index:-1;
}

.hero-grid{
    display:grid;
    grid-template-columns:45% 55%;
    align-items:center;
    min-height:620px;
}

.hero-content{
    padding-right:35px;
    animation:fadeUp .9s ease;
}

.eyebrow{
    color:var(--verde-opalo);
    font-size:14px;
    font-weight:800;
    letter-spacing:2px;
    text-transform:uppercase;
    margin-bottom:18px;
}

.hero h1{
    font-family:"Montserrat";
    font-size:clamp(42px,5vw,70px);
    line-height:1.03;
    letter-spacing:-3px;
    margin-bottom:25px;
}

.hero h1 span{
    color:var(--verde-opalo);
}

.hero p{
    color:var(--gris-texto);
    font-size:17px;
    line-height:1.8;
    margin-bottom:30px;
}

.hero-buttons{
    display:flex;
    gap:12px;
    flex-wrap:wrap;
}

.hero-image{
    height:570px;
    position:relative;
    overflow:hidden;
    border-radius:40% 0 0 40%;
}

.hero-image img{
    width:100%;
    height:100%;
    object-fit:cover;
}

.hero-card{
    position:absolute;
    bottom:35px;
    left:35px;
    background:rgba(255,255,255,.94);
    backdrop-filter:blur(10px);
    padding:20px;
    border-radius:18px;
    box-shadow:var(--sombra);
    width:230px;
}

.hero-card-item{
    display:flex;
    align-items:center;
    gap:12px;
    margin:10px 0;
    font-size:12px;
    font-weight:600;
}

.hero-card-icon{
    width:35px;
    height:35px;
    border-radius:50%;
    background:#e5f3ef;
    display:grid;
    place-items:center;
    color:var(--verde-opalo);
}

/* =========================================================
   CONTACT BAR
========================================================= */

.quick-contact{
    margin-top:-45px;
    position:relative;
    z-index:10;
}

.quick-box{
    background:linear-gradient(100deg,var(--verde-opalo),var(--azul-turquesa));
    color:white;
    border-radius:20px;
    padding:20px 30px;
    display:flex;
    align-items:center;
    justify-content:space-between;
    gap:20px;
    box-shadow:var(--sombra);
}

.contact-item{
    display:flex;
    align-items:center;
    gap:10px;
    font-size:14px;
}

.contact-item i{
    font-size:19px;
}

/* =========================================================
   SECTION
========================================================= */

section{
    padding:100px 0;
}

.section-title{
    max-width:700px;
    margin-bottom:50px;
}

.section-title.center{
    margin-left:auto;
    margin-right:auto;
    text-align:center;
}

.section-title small{
    color:var(--verde-opalo);
    font-weight:800;
    letter-spacing:2px;
    text-transform:uppercase;
}

.section-title h2{
    font-family:"Montserrat";
    font-size:clamp(32px,4vw,48px);
    margin:12px 0;
    letter-spacing:-1.5px;
}

.section-title p{
    color:var(--gris-texto);
    line-height:1.8;
}

/* =========================================================
   MISSION
========================================================= */

.mission{
    background:var(--verde-opalo);
    color:white;
    border-radius:40px;
    margin:60px auto;
    width:min(1180px,92%);
    padding:65px;
}

.mission-grid{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:60px;
    align-items:center;
}

.mission h2{
    font-family:"Montserrat";
    font-size:42px;
    margin:15px 0;
}

.mission p{
    color:#d9eeea;
    line-height:1.9;
}

.values{
    display:grid;
    grid-template-columns:repeat(2,1fr);
    gap:12px;
    margin-top:25px;
}

.value{
    padding:15px;
    border:1px solid rgba(255,255,255,.15);
    border-radius:14px;
    transition:.3s;
}

.value:hover{
    background:rgba(255,255,255,.1);
    transform:translateY(-3px);
}

/* =========================================================
   SERVICES
========================================================= */

.services{
    background:#f7faf9;
}

.service-grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:22px;
}

.service-card{
    background:white;
    border-radius:22px;
    overflow:hidden;
    box-shadow:0 8px 30px rgba(0,0,0,.06);
    transition:.4s;
}

.service-card:hover{
    transform:translateY(-8px);
    box-shadow:var(--sombra);
}

.service-image{
    height:210px;
    overflow:hidden;
}

.service-image img{
    width:100%;
    height:100%;
    object-fit:cover;
    transition:.5s;
}

.service-card:hover img{
    transform:scale(1.08);
}

.service-content{
    padding:25px;
}

.service-icon{
    width:45px;
    height:45px;
    background:#e6f4f0;
    color:var(--verde-opalo);
    border-radius:12px;
    display:grid;
    place-items:center;
    margin-bottom:15px;
    font-size:20px;
}

.service-content h3{
    font-family:"Montserrat";
    margin-bottom:10px;
}

.service-content p{
    color:var(--gris-texto);
    font-size:14px;
    line-height:1.7;
    margin-bottom:18px;
}

.more{
    color:var(--verde-opalo);
    font-weight:700;
    cursor:pointer;
}

/* =========================================================
   SOLAR FEATURE
========================================================= */

.solar{
    position:relative;
}

.solar-grid{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:50px;
    align-items:center;
}

.solar-image{
    border-radius:30px;
    overflow:hidden;
    height:480px;
}

.solar-image img{
    width:100%;
    height:100%;
    object-fit:cover;
}

.solar-content h2{
    font-family:"Montserrat";
    font-size:44px;
    margin:15px 0;
}

.solar-content p{
    color:var(--gris-texto);
    line-height:1.9;
    margin-bottom:25px;
}

.check{
    display:flex;
    gap:12px;
    margin:15px 0;
    align-items:center;
}

.check span{
    width:27px;
    height:27px;
    border-radius:50%;
    background:#e5f3ef;
    color:var(--verde-opalo);
    display:grid;
    place-items:center;
}

/* =========================================================
   STATS
========================================================= */

.stats{
    background:linear-gradient(110deg,var(--verde-opalo),var(--azul-agua));
    color:white;
}

.stats-grid{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    text-align:center;
}

.stat{
    padding:20px;
    border-right:1px solid rgba(255,255,255,.18);
}

.stat:last-child{
    border:none;
}

.stat-number{
    font-family:"Montserrat";
    font-size:44px;
    font-weight:800;
}

.stat p{
    opacity:.8;
    margin-top:5px;
}

/* =========================================================
   PROJECTS
========================================================= */

.filters{
    display:flex;
    justify-content:center;
    gap:10px;
    flex-wrap:wrap;
    margin-bottom:35px;
}

.filter{
    border:1px solid #d7e5e1;
    background:white;
    padding:10px 18px;
    border-radius:30px;
    cursor:pointer;
    color:var(--gris-texto);
    transition:.3s;
}

.filter.active,
.filter:hover{
    background:var(--verde-opalo);
    color:white;
}

.project-grid{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    gap:15px;
}

.project{
    height:260px;
    border-radius:20px;
    overflow:hidden;
    position:relative;
    cursor:pointer;
}

.project img{
    width:100%;
    height:100%;
    object-fit:cover;
    transition:.5s;
}

.project:hover img{
    transform:scale(1.1);
}

.project-overlay{
    position:absolute;
    inset:0;
    background:linear-gradient(transparent,rgba(0,0,0,.75));
    display:flex;
    align-items:flex-end;
    padding:20px;
    color:white;
    opacity:0;
    transition:.3s;
}

.project:hover .project-overlay{
    opacity:1;
}

/* =========================================================
   QUOTE
========================================================= */

.quote{
    background:#f4f8f7;
}

.quote-box{
    background:white;
    border-radius:30px;
    padding:50px;
    box-shadow:var(--sombra);
}

.form-grid{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:18px;
}

.form-group{
    display:flex;
    flex-direction:column;
    gap:8px;
}

.form-group.full{
    grid-column:1/-1;
}

.form-group label{
    font-weight:600;
    font-size:14px;
}

.form-group input,
.form-group select,
.form-group textarea{
    border:1px solid #dce8e5;
    padding:15px;
    border-radius:12px;
    outline:none;
    transition:.3s;
}

.form-group textarea{
    min-height:130px;
    resize:vertical;
}

.form-group input:focus,
.form-group select:focus,
.form-group textarea:focus{
    border-color:var(--verde-opalo);
    box-shadow:0 0 0 4px rgba(1,93,82,.08);
}

/* =========================================================
   FOOTER
========================================================= */

footer{
    background:#073f39;
    color:white;
    padding:70px 0 25px;
}

.footer-grid{
    display:grid;
    grid-template-columns:2fr 1fr 1fr 1.5fr;
    gap:50px;
}

.footer-brand p{
    color:#c4dad5;
    line-height:1.8;
    margin:20px 0;
}

.footer h4{
    margin-bottom:20px;
}

.footer-links{
    display:flex;
    flex-direction:column;
    gap:12px;
    color:#c4dad5;
    font-size:14px;
}

.footer-links a:hover{
    color:white;
}

.socials{
    display:flex;
    gap:10px;
}

.social{
    width:40px;
    height:40px;
    border:1px solid rgba(255,255,255,.2);
    border-radius:50%;
    display:grid;
    place-items:center;
    transition:.3s;
}

.social:hover{
    background:white;
    color:var(--verde-opalo);
}

.footer-bottom{
    border-top:1px solid rgba(255,255,255,.12);
    margin-top:50px;
    padding-top:20px;
    display:flex;
    justify-content:space-between;
    color:#aac8c2;
    font-size:12px;
}

/* =========================================================
   WHATSAPP
========================================================= */

.whatsapp{
    position:fixed;
    right:25px;
    bottom:25px;
    width:58px;
    height:58px;
    border-radius:50%;
    background:#25d366;
    color:white;
    display:grid;
    place-items:center;
    font-size:27px;
    z-index:900;
    box-shadow:0 10px 30px rgba(0,0,0,.2);
    transition:.3s;
}

.whatsapp:hover{
    transform:scale(1.1);
}

/* =========================================================
   AI ASSISTANT
========================================================= */

.ai-button{
    position:fixed;
    right:25px;
    bottom:95px;
    width:58px;
    height:58px;
    border-radius:50%;
    background:var(--verde-opalo);
    color:white;
    border:none;
    cursor:pointer;
    font-size:24px;
    z-index:900;
    box-shadow:0 10px 30px rgba(0,0,0,.2);
}

.ai-window{
    position:fixed;
    right:25px;
    bottom:165px;
    width:340px;
    max-width:calc(100% - 30px);
    background:white;
    border-radius:22px;
    box-shadow:0 20px 60px rgba(0,0,0,.2);
    overflow:hidden;
    z-index:901;
    display:none;
}

.ai-window.active{
    display:block;
    animation:pop .3s ease;
}

.ai-header{
    background:var(--verde-opalo);
    color:white;
    padding:18px;
    display:flex;
    justify-content:space-between;
    align-items:center;
}

.ai-body{
    height:320px;
    padding:15px;
    overflow-y:auto;
}

.ai-message{
    background:#eef6f4;
    padding:12px;
    border-radius:14px;
    font-size:13px;
    margin-bottom:10px;
}

.ai-user{
    background:var(--verde-opalo);
    color:white;
    margin-left:30px;
}

.ai-options{
    display:flex;
    flex-direction:column;
    gap:7px;
}

.ai-options button{
    background:white;
    border:1px solid #d5e3df;
    padding:9px;
    border-radius:10px;
    cursor:pointer;
    text-align:left;
}

.ai-input{
    border-top:1px solid #eee;
    padding:10px;
    display:flex;
    gap:7px;
}

.ai-input input{
    flex:1;
    border:1px solid #ddd;
    padding:10px;
    border-radius:10px;
}

/* =========================================================
   MODAL
========================================================= */

.modal{
    position:fixed;
    inset:0;
    background:rgba(0,0,0,.6);
    z-index:2000;
    display:none;
    align-items:center;
    justify-content:center;
    padding:20px;
}

.modal.active{
    display:flex;
}

.modal-box{
    background:white;
    width:600px;
    max-width:100%;
    padding:40px;
    border-radius:25px;
    position:relative;
    animation:pop .3s;
}

.modal-close{
    position:absolute;
    right:20px;
    top:20px;
    border:none;
    background:#eef5f3;
    width:35px;
    height:35px;
    border-radius:50%;
    cursor:pointer;
    font-size:18px;
}

/* =========================================================
   BACK TO TOP
========================================================= */

.top{
    position:fixed;
    bottom:25px;
    left:25px;
    width:45px;
    height:45px;
    border:none;
    border-radius:50%;
    background:white;
    color:var(--verde-opalo);
    box-shadow:var(--sombra);
    cursor:pointer;
    opacity:0;
    pointer-events:none;
    transition:.3s;
    z-index:800;
}

.top.show{
    opacity:1;
    pointer-events:auto;
}

/* =========================================================
   ANIMATIONS
========================================================= */

.reveal{
    opacity:0;
    transform:translateY(30px);
    transition:opacity .7s, transform .7s;
}

.reveal.visible{
    opacity:1;
    transform:translateY(0);
}

@keyframes fadeUp{
    from{
        opacity:0;
        transform:translateY(30px);
    }
    to{
        opacity:1;
        transform:translateY(0);
    }
}

@keyframes pop{
    from{
        opacity:0;
        transform:scale(.9);
    }
    to{
        opacity:1;
        transform:scale(1);
    }
}

/* =========================================================
   RESPONSIVE
========================================================= */

@media(max-width:950px){

    .nav-links,
    .nav-actions{
        display:none;
    }

    .mobile-menu{
        display:block;
    }

    .nav-links.mobile-active{
        position:absolute;
        display:flex;
        flex-direction:column;
        background:white;
        width:92%;
        top:75px;
        left:4%;
        padding:25px;
        border-radius:18px;
        box-shadow:var(--sombra);
    }

    .hero-grid,
    .mission-grid,
    .solar-grid{
        grid-template-columns:1fr;
    }

    .hero{
        padding-top:110px;
    }

    .hero-content{
        padding-right:0;
        margin-bottom:40px;
    }

    .hero-image{
        height:430px;
        border-radius:30px;
    }

    .service-grid{
        grid-template-columns:repeat(2,1fr);
    }

    .project-grid{
        grid-template-columns:repeat(2,1fr);
    }

    .stats-grid{
        grid-template-columns:repeat(2,1fr);
    }

    .stat{
        border-bottom:1px solid rgba(255,255,255,.15);
    }

    .footer-grid{
        grid-template-columns:1fr 1fr;
    }

}

@media(max-width:600px){

    section{
        padding:70px 0;
    }

    .quick-box{
        flex-direction:column;
        align-items:flex-start;
    }

    .mission{
        padding:35px 25px;
    }

    .values{
        grid-template-columns:1fr;
    }

    .service-grid,
    .project-grid,
    .stats-grid,
    .footer-grid,
    .form-grid{
        grid-template-columns:1fr;
    }

    .hero h1{
        font-size:43px;
    }

    .hero-image{
        height:350px;
    }

    .solar-content h2{
        font-size:34px;
    }

    .quote-box{
        padding:25px;
    }

    .footer-bottom{
        flex-direction:column;
        gap:10px;
    }

}

</style>
</head>

<body>

<!-- =====================================================
     HEADER
===================================================== -->

<header id="header">

<div class="container navbar">

<a href="#inicio" class="logo">

<div class="logo-symbol"></div>

<div class="logo-text">
<strong>SOLUCIONES</strong>
<strong>INTEGRALES</strong>
<span>SOSTENIBLES</span>
</div>

</a>

<nav class="nav-links" id="navLinks">
<a href="#inicio">Inicio</a>
<a href="#servicios">Servicios</a>
<a href="#nosotros">Nosotros</a>
<a href="#proyectos">Proyectos</a>
<a href="#presupuesto">Contacto</a>
<a href="#footer">Blog</a>
</nav>

<div class="nav-actions">

<a class="btn btn-outline"
href="https://wa.me/34634000534"
target="_blank">
WhatsApp
</a>

<a class="btn btn-primary"
href="#presupuesto">
Solicitar presupuesto
</a>

</div>

<div class="mobile-menu" id="mobileMenu">
☰
</div>

</div>

</header>


<!-- =====================================================
     HERO
===================================================== -->

<main>

<section class="hero" id="inicio">

<div class="container hero-grid">

<div class="hero-content">

<div class="eyebrow">
Soluciones profesionales y sostenibles
</div>

<h1>
Soluciones que construyen un
<span>futuro sostenible.</span>
</h1>

<p>
Proporcionamos soluciones integrales de mantenimiento,
limpieza especializada y asesoramiento profesional que
contribuyen a la seguridad, eficiencia y sostenibilidad
de empresas, comunidades y particulares.
</p>

<div class="hero-buttons">

<a href="#servicios" class="btn btn-primary">
Ver nuestros servicios →
</a>

<a href="#presupuesto" class="btn btn-outline">
Solicitar presupuesto
</a>

</div>

</div>


<div class="hero-image">

<img
src="https://images.unsplash.com/photo-1509391366360-2e959784a276?auto=format&fit=crop&w=1200&q=85"
alt="Paneles solares y energía sostenible"
>

<div class="hero-card">

<div class="hero-card-item">
<div class="hero-card-icon">🌱</div>
<div>
Compromiso<br>
<small>con el medio ambiente</small>
</div>
</div>

<div class="hero-card-item">
<div class="hero-card-icon">⚙️</div>
<div>
Tecnología<br>
<small>e innovación</small>
</div>
</div>

<div class="hero-card-item">
<div class="hero-card-icon">✓</div>
<div>
Resultados<br>
<small>profesionales</small>
</div>
</div>

</div>

</div>

</div>

</section>


<!-- =====================================================
     CONTACTO RAPIDO
===================================================== -->

<div class="quick-contact">

<div class="container quick-box">

<a href="tel:+34634000534" class="contact-item">
☎️ +34 634 00 05 34
</a>

<a href="mailto:sissostenible@gmail.com" class="contact-item">
✉️ sissostenible@gmail.com
</a>

<a href="https://instagram.com/sissostenible"
target="_blank"
class="contact-item">
Instagram
</a>

<a href="https://www.tiktok.com/@sissostenible"
target="_blank"
class="contact-item">
TikTok
</a>

</div>

</div>


<!-- =====================================================
     MISION
===================================================== -->

<section id="nosotros">

<div class="mission reveal">

<div class="mission-grid">

<div>

<small>🌱 NUESTRA MISIÓN</small>

<h2>
Profesionalidad con visión sostenible.
</h2>

<p>
Proporcionamos soluciones integrales de mantenimiento,
limpieza especializada y asesoramiento profesional que
contribuyan a la seguridad, eficiencia y sostenibilidad
de las instalaciones de empresas, comunidades y particulares.
</p>

</div>


<div>

<h3>Nuestros valores</h3>

<div class="values">

<div class="value">✓ Profesionalidad</div>
<div class="value">✓ Compromiso</div>
<div class="value">✓ Transparencia</div>
<div class="value">✓ Innovación</div>
<div class="value">✓ Seguridad</div>
<div class="value">✓ Responsabilidad</div>
<div class="value">✓ Sostenibilidad</div>

</div>

</div>

</div>

</div>

</section>


<!-- =====================================================
     SERVICIOS
===================================================== -->

<section class="services" id="servicios">

<div class="container">

<div class="section-title center reveal">

<small>Qué hacemos</small>

<h2>
Servicios de limpieza profesional
</h2>

<p>
Ofrecemos soluciones de limpieza adaptadas a diferentes
tipos de instalaciones y superficies.
</p>

</div>


<div class="service-grid">


<!-- SERVICE 1 -->

<article class="service-card reveal">

<div class="service-image">

<img
src="https://images.unsplash.com/photo-1581578731548-c64695cc6952?auto=format&fit=crop&w=800&q=85"
alt="Limpieza profesional"
>

</div>

<div class="service-content">

<div class="service-icon">🧹</div>

<h3>Limpieza técnica especializada</h3>

<p>
Soluciones profesionales para instalaciones
que requieren un cuidado específico.
</p>

<span class="more"
onclick="openService('Limpieza técnica especializada')">
Más información →
</span>

</div>

</article>


<!-- SERVICE 2 -->

<article class="service-card reveal">

<div class="service-image">

<img
src="https://images.unsplash.com/photo-1497435334941-8c899ee9e8e9?auto=format&fit=crop&w=800&q=85"
alt="Mantenimiento industrial"
>

</div>

<div class="service-content">

<div class="service-icon">🏭</div>

<h3>Limpieza de cubiertas industriales</h3>

<p>
Limpieza profesional y mantenimiento de
cubiertas y superficies industriales.
</p>

<span class="more"
onclick="openService('Limpieza de cubiertas industriales')">
Más información →
</span>

</div>

</article>


<!-- SERVICE 3 -->

<article class="service-card reveal">

<div class="service-image">

<img
src="https://images.unsplash.com/photo-1509391366360-2e959784a276?auto=format&fit=crop&w=800&q=85"
alt="Limpieza de placas fotovoltaicas"
>

</div>

<div class="service-content">

<div class="service-icon">☀️</div>

<h3>Limpieza de placas fotovoltaicas</h3>

<p>
Mantenimiento y limpieza profesional para
instalaciones solares.
</p>

<span class="more"
onclick="openService('Limpieza de placas fotovoltaicas')">
Más información →
</span>

</div>

</article>


<!-- SERVICE 4 -->

<article class="service-card reveal">

<div class="service-image">

<img
src="https://images.unsplash.com/photo-1497366811353-6870744d04b2?auto=format&fit=crop&w=800&q=85"
alt="Limpieza de oficinas"
>

</div>

<div class="service-content">

<div class="service-icon">🏢</div>

<h3>Limpieza de oficinas</h3>

<p>
Espacios de trabajo limpios, cuidados y preparados
para el día a día.
</p>

<span class="more"
onclick="openService('Limpieza de oficinas')">
Más información →
</span>

</div>

</article>


<!-- SERVICE 5 -->

<article class="service-card reveal">

<div class="service-image">

<img
src="https://images.unsplash.com/photo-1600607687920-4e2a09cf159d?auto=format&fit=crop&w=800&q=85"
alt="Limpieza de comunidades"
>

</div>

<div class="service-content">

<div class="service-icon">🏘️</div>

<h3>Limpieza de comunidades</h3>

<p>
Mantenimiento de zonas comunes para comunidades
de propietarios.
</p>

<span class="more"
onclick="openService('Limpieza de comunidades')">
Más información →
</span>

</div>

</article>


<!-- SERVICE 6 -->

<article class="service-card reveal">

<div class="service-image">

<img
src="https://images.unsplash.com/photo-1556761175-b413da4baf72?auto=format&fit=crop&w=800&q=85"
alt="Limpieza de locales"
>

</div>

<div class="service-content">

<div class="service-icon">🏪</div>

<h3>Locales comerciales</h3>

<p>
Limpieza profesional para negocios y espacios
comerciales.
</p>

<span class="more"
onclick="openService('Limpieza de locales comerciales')">
Más información →
</span>

</div>

</article>

</div>

</div>

</section>


<!-- =====================================================
     SOLAR
===================================================== -->

<section class="solar">

<div class="container solar-grid">

<div class="solar-image reveal">

<img
src="https://images.unsplash.com/photo-1508514177221-188b1cf16e9d?auto=format&fit=crop&w=1000&q=85"
alt="Paneles fotovoltaicos"
>

</div>

<div class="solar-content reveal">

<small class="eyebrow">
ENERGÍA SOLAR
</small>

<h2>
Limpieza profesional de placas fotovoltaicas
</h2>

<p>
Cuidamos tus instalaciones solares mediante soluciones
profesionales de limpieza y mantenimiento, ayudando a
conservar las superficies en condiciones adecuadas.
</p>

<div class="check">
<span>✓</span>
Limpieza especializada
</div>

<div class="check">
<span>✓</span>
Profesionales cualificados
</div>

<div class="check">
<span>✓</span>
Tratamiento cuidadoso de superficies
</div>

<div class="check">
<span>✓</span>
Presupuesto personalizado
</div>

<a href="#presupuesto" class="btn btn-primary">
Solicitar presupuesto
</a>

</div>

</div>

</section>


<!-- =====================================================
     ESTADISTICAS
===================================================== -->

<section class="stats">

<div class="container stats-grid">

<div class="stat">
<div class="stat-number counter" data-target="120">0</div>
<p>Proyectos realizados</p>
</div>

<div class="stat">
<div class="stat-number counter" data-target="85">0</div>
<p>Clientes satisfechos</p>
</div>

<div class="stat">
<div class="stat-number counter" data-target="15">0</div>
<p>Años de experiencia</p>
</div>

<div class="stat">
<div class="stat-number">100%</div>
<p>Compromiso sostenible</p>
</div>

</div>

</section>


<!-- =====================================================
     PROYECTOS
===================================================== -->

<section id="proyectos">

<div class="container">

<div class="section-title center reveal">

<small>Nuestro trabajo</small>

<h2>Proyectos destacados</h2>

<p>
Algunos ejemplos de nuestros trabajos y soluciones.
</p>

</div>


<div class="filters">

<button class="filter active" data-filter="all">
Todos
</button>

<button class="filter" data-filter="solar">
Fotovoltaica
</button>

<button class="filter" data-filter="clean">
Limpieza
</button>

<button class="filter" data-filter="industrial">
Industrial
</button>

</div>


<div class="project-grid">


<div class="project" data-category="solar">

<img src="https://images.unsplash.com/photo-1509391366360-2e959784a276?auto=format&fit=crop&w=800&q=80">

<div class="project-overlay">
Proyecto fotovoltaico
</div>

</div>


<div class="project" data-category="clean">

<img src="https://images.unsplash.com/photo-1581578731548-c64695cc6952?auto=format&fit=crop&w=800&q=80">

<div class="project-overlay">
Limpieza profesional
</div>

</div>


<div class="project" data-category="industrial">

<img src="https://images.unsplash.com/photo-1581092160562-40aa08e78837?auto=format&fit=crop&w=800&q=80">

<div class="project-overlay">
Mantenimiento industrial
</div>

</div>


<div class="project" data-category="solar">

<img src="https://images.unsplash.com/photo-1497435334941-8c899ee9e8e9?auto=format&fit=crop&w=800&q=80">

<div class="project-overlay">
Instalación solar
</div>

</div>


<div class="project" data-category="clean">

<img src="https://images.unsplash.com/photo-1497366754035-f200968a6e72?auto=format&fit=crop&w=800&q=80">

<div class="project-overlay">
Limpieza de oficinas
</div>

</div>


<div class="project" data-category="industrial">

<img src="https://images.unsplash.com/photo-1586864387967-d02ef85d93e8?auto=format&fit=crop&w=800&q=80">

<div class="project-overlay">
Limpieza industrial
</div>

</div>

</div>

</div>

</section>


<!-- =====================================================
     PRESUPUESTO
===================================================== -->

<section class="quote" id="presupuesto">

<div class="container">

<div class="quote-box reveal">

<div class="section-title">

<small>Contacto</small>

<h2>Solicita tu presupuesto</h2>

<p>
Cuéntanos qué necesitas y estudiaremos una solución
adaptada a tu instalación.
</p>

</div>


<form id="quoteForm">

<div class="form-grid">

<div class="form-group">

<label>Nombre</label>

<input
type="text"
id="name"
placeholder="Tu nombre"
required
>

</div>


<div class="form-group">

<label>Teléfono</label>

<input
type="tel"
id="phone"
placeholder="+34..."
required
>

</div>


<div class="form-group">

<label>Email</label>

<input
type="email"
id="email"
placeholder="tu@email.com"
required
>

</div>


<div class="form-group">

<label>Servicio</label>

<select id="service">

<option>Limpieza técnica especializada</option>
<option>Limpieza de cubiertas industriales</option>
<option>Limpieza de placas fotovoltaicas</option>
<option>Limpieza de oficinas</option>
<option>Limpieza de comunidades</option>
<option>Limpieza de locales comerciales</option>
<option>Otro servicio</option>

</select>

</div>


<div class="form-group full">

<label>Mensaje</label>

<textarea
id="message"
placeholder="Cuéntanos qué necesitas..."
></textarea>

</div>

<div class="form-group full">

<button class="btn btn-primary" type="submit">
Enviar solicitud →
</button>

</div>

</div>

</form>

</div>

</div>

</section>

</main>


<!-- =====================================================
     FOOTER
===================================================== -->

<footer id="footer">

<div class="container">

<div class="footer-grid">

<div class="footer-brand">

<div class="logo">

<div class="logo-symbol"></div>

<div class="logo-text">
<strong style="color:white">SOLUCIONES</strong>
<strong style="color:white">INTEGRALES</strong>
<span>SOSTENIBLES</span>
</div>

</div>

<p>
Soluciones profesionales para construir
un futuro más seguro, eficiente y sostenible.
</p>

<div class="socials">

<a class="social"
href="https://www.instagram.com/sissostenible/"
target="_blank">
IG
</a>

<a class="social"
href="https://www.tiktok.com/@sissostenible"
target="_blank">
TK
</a>

<a class="social"
href="https://wa.me/34634000534"
target="_blank">
WA
</a>

</div>

</div>


<div>

<h4>Enlaces</h4>

<div class="footer-links">

<a href="#inicio">Inicio</a>
<a href="#servicios">Servicios</a>
<a href="#nosotros">Nosotros</a>
<a href="#proyectos">Proyectos</a>
<a href="#presupuesto">Contacto</a>

</div>

</div>


<div>

<h4>Servicios</h4>

<div class="footer-links">

<a href="#servicios">Limpieza técnica</a>
<a href="#servicios">Cubiertas industriales</a>
<a href="#servicios">Placas fotovoltaicas</a>
<a href="#servicios">Oficinas</a>
<a href="#servicios">Comunidades</a>

</div>

</div>


<div>

<h4>Contacto</h4>

<div class="footer-links">

<a href="tel:+34634000534">
+34 634 00 05 34
</a>

<a href="mailto:sissostenible@gmail.com">
sissostenible@gmail.com
</a>

<a href="https://www.instagram.com/sissostenible/"
target="_blank">
Instagram
</a>

<a href="https://www.tiktok.com/@sissostenible"
target="_blank">
TikTok
</a>

</div>

</div>

</div>


<div class="footer-bottom">

<span>
© 2026 Soluciones Integrales Sostenibles.
Todos los derechos reservados.
</span>

<span>
Aviso legal · Privacidad · Cookies
</span>

</div>

</div>

</footer>


<!-- =====================================================
     WHATSAPP
===================================================== -->

<a
class="whatsapp"
href="https://wa.me/34634000534?text=Hola,%20me%20gustaría%20solicitar%20información."
target="_blank"
aria-label="WhatsApp">
☎
</a>


<!-- =====================================================
     AI ASSISTANT
===================================================== -->

<button class="ai-button" id="aiButton">
✦
</button>

<div class="ai-window" id="aiWindow">

<div class="ai-header">

<strong>Asistente SISS</strong>

<button
onclick="toggleAI()"
style="background:none;border:0;color:white;cursor:pointer;font-size:20px">
×
</button>

</div>


<div class="ai-body" id="aiBody">

<div class="ai-message">

👋 ¡Hola! Soy el asistente virtual de
<strong>Soluciones Integrales Sostenibles</strong>.

¿En qué puedo ayudarte?

</div>


<div class="ai-options">

<button onclick="aiQuestion('servicios')">
¿Qué servicios ofrecéis?
</button>

<button onclick="aiQuestion('solar')">
¿Limpiáis placas solares?
</button>

<button onclick="aiQuestion('presupuesto')">
Quiero solicitar un presupuesto
</button>

<button onclick="aiQuestion('contacto')">
¿Cómo puedo contactar?
</button>

</div>

</div>


<div class="ai-input">

<input
id="aiInput"
placeholder="Escribe tu pregunta..."
>

<button
class="btn btn-primary"
onclick="sendAI()">
➤
</button>

</div>

</div>


<!-- =====================================================
     MODAL SERVICIO
===================================================== -->

<div class="modal" id="serviceModal">

<div class="modal-box">

<button
class="modal-close"
onclick="closeModal()">
×
</button>

<h2 id="modalTitle"></h2>

<p id="modalText" style="margin:20px 0;line-height:1.8;color:#5d6b69"></p>

<a
href="#presupuesto"
onclick="closeModal()"
class="btn btn-primary">
Solicitar presupuesto
</a>

</div>

</div>


<!-- =====================================================
     BACK TO TOP
===================================================== -->

<button class="top" id="top">
↑
</button>


<script>

/* =========================================================
   HEADER SCROLL
========================================================= */

const header = document.getElementById("header");

window.addEventListener("scroll",()=>{

if(window.scrollY > 50){
    header.classList.add("scrolled");
}else{
    header.classList.remove("scrolled");
}

});


/* =========================================================
   MOBILE MENU
========================================================= */

const mobileMenu = document.getElementById("mobileMenu");
const navLinks = document.getElementById("navLinks");

mobileMenu.addEventListener("click",()=>{

navLinks.classList.toggle("mobile-active");

});


document.querySelectorAll(".nav-links a").forEach(link=>{

link.addEventListener("click",()=>{

navLinks.classList.remove("mobile-active");

});

});


/* =========================================================
   SCROLL REVEAL
========================================================= */

const reveals = document.querySelectorAll(".reveal");

const observer = new IntersectionObserver(entries=>{

entries.forEach(entry=>{

if(entry.isIntersecting){

entry.target.classList.add("visible");

}

});

},{threshold:.15});

reveals.forEach(el=>observer.observe(el));


/* =========================================================
   CONTADORES
========================================================= */

let countersStarted = false;

const statsSection = document.querySelector(".stats");

const statsObserver = new IntersectionObserver(entries=>{

if(entries[0].isIntersecting && !countersStarted){

countersStarted = true;

document.querySelectorAll(".counter").forEach(counter=>{

const target = +counter.dataset.target;

let current = 0;

const increment = target / 60;

function update(){

current += increment;

if(current < target){

counter.textContent = Math.ceil(current) + "+";

requestAnimationFrame(update);

}else{

counter.textContent = target + "+";

}

}

update();

});

}

});

statsObserver.observe(statsSection);


/* =========================================================
   PROJECT FILTER
========================================================= */

const filters = document.querySelectorAll(".filter");
const projects = document.querySelectorAll(".project");

filters.forEach(button=>{

button.addEventListener("click",()=>{

filters.forEach(b=>b.classList.remove("active"));

button.classList.add("active");

const filter = button.dataset.filter;

projects.forEach(project=>{

if(filter === "all" || project.dataset.category === filter){

project.style.display = "block";

}else{

project.style.display = "none";

}

});

});

});


/* =========================================================
   SERVICE MODAL
========================================================= */

function openService(service){

const modal = document.getElementById("serviceModal");

const title = document.getElementById("modalTitle");

const text = document.getElementById("modalText");

title.textContent = service;

const descriptions = {

"Limpieza técnica especializada":
"Realizamos servicios de limpieza profesional adaptados a instalaciones y superficies que requieren procedimientos específicos.",

"Limpieza de cubiertas industriales":
"Ofrecemos soluciones de limpieza y mantenimiento para cubiertas industriales, ayudando a conservar las instalaciones en condiciones adecuadas.",

"Limpieza de placas fotovoltaicas":
"Realizamos limpieza profesional de placas fotovoltaicas para ayudar a mantener la superficie de los paneles limpia y correctamente conservada.",

"Limpieza de oficinas":
"Mantenemos espacios de trabajo limpios, higiénicos y preparados para empleados, clientes y visitantes.",

"Limpieza de comunidades":
"Servicios adaptados a comunidades de propietarios, zonas comunes y diferentes espacios compartidos.",

"Limpieza de locales comerciales":
"Soluciones de limpieza profesional para comercios y establecimientos abiertos al público."

};

text.textContent =
descriptions[service] ||
"Contacta con nosotros para conocer todos los detalles de este servicio.";

modal.classList.add("active");

}


function closeModal(){

document
.getElementById("serviceModal")
.classList.remove("active");

}


window.addEventListener("click",e=>{

if(e.target.id === "serviceModal"){

closeModal();

}

});


/* =========================================================
   FORMULARIO
========================================================= */

document
.getElementById("quoteForm")
.addEventListener("submit",function(e){

e.preventDefault();

const name = document.getElementById("name").value;
const phone = document.getElementById("phone").value;
const service = document.getElementById("service").value;
const message = document.getElementById("message").value;

const whatsappMessage =
`Hola, soy ${name}.
Me gustaría solicitar un presupuesto.

Servicio: ${service}

Teléfono: ${phone}

Mensaje:
${message}`;

const url =
"https://wa.me/34634000534?text=" +
encodeURIComponent(whatsappMessage);

window.open(url,"_blank");

});


/* =========================================================
   AI
========================================================= */

const aiWindow = document.getElementById("aiWindow");
const aiBody = document.getElementById("aiBody");

document
.getElementById("aiButton")
.addEventListener("click",toggleAI);


function toggleAI(){

aiWindow.classList.toggle("active");

}


function aiQuestion(type){

let question = "";
let answer = "";

if(type === "servicios"){

question = "¿Qué servicios ofrecéis?";

answer =
"Ofrecemos limpieza técnica especializada, limpieza de cubiertas industriales, limpieza de placas fotovoltaicas, oficinas, comunidades, locales comerciales y otras soluciones de mantenimiento.";

}

if(type === "solar"){

question = "¿Limpiáis placas solares?";

answer =
"Sí. Realizamos limpieza profesional de placas fotovoltaicas. Puedes solicitar un presupuesto personalizado desde la sección de contacto.";

}

if(type === "presupuesto"){

question = "Quiero solicitar un presupuesto";

answer =
"Perfecto. Puedes rellenar nuestro formulario de presupuesto o contactar directamente por WhatsApp en el +34 634 00 05 34.";

}

if(type === "contacto"){

question = "¿Cómo puedo contactar?";

answer =
"Puedes llamarnos o escribirnos por WhatsApp al +34 634 00 05 34 o enviarnos un correo a sissostenible@gmail.com.";

}

addAIMessage(question,true);

setTimeout(()=>{

addAIMessage(answer,false);

},400);

}


function addAIMessage(text,user){

const div = document.createElement("div");

div.className =
"user" === "user"
? "ai-message ai-user"
: "ai-message";

if(user){
div.classList.add("ai-user");
}

div.textContent = text;

aiBody.appendChild(div);

aiBody.scrollTop = aiBody.scrollHeight;

}


function sendAI(){

const input = document.getElementById("aiInput");

const text = input.value.trim();

if(!text)return;

addAIMessage(text,true);

input.value = "";

setTimeout(()=>{

let answer =
"Gracias por tu consulta. Para recibir información personalizada puedes contactar con nosotros por WhatsApp en el +34 634 00 05 34 o solicitar un presupuesto.";

const lower = text.toLowerCase();

if(lower.includes("solar") ||
lower.includes("placa") ||
lower.includes("fotovolta")){
answer =
"Sí, ofrecemos limpieza profesional de placas fotovoltaicas. Puedes solicitar un presupuesto personalizado.";
}

else if(lower.includes("precio") ||
lower.includes("presupuesto")){
answer =
"Podemos preparar un presupuesto personalizado según el tipo de instalación y servicio. Escríbenos por WhatsApp al +34 634 00 05 34.";
}

else if(lower.includes("correo") ||
lower.includes("email")){
answer =
"Nuestro correo es sissostenible@gmail.com.";
}

else if(lower.includes("telefono") ||
lower.includes("teléfono") ||
lower.includes("whatsapp")){
answer =
"Puedes contactar con nosotros en el +34 634 00 05 34.";
}

addAIMessage(answer,false);

},500);

}


/* =========================================================
   BACK TO TOP
========================================================= */

const topButton = document.getElementById("top");

window.addEventListener("scroll",()=>{

if(window.scrollY > 500){

topButton.classList.add("show");

}else{

topButton.classList.remove("show");

}

});


topButton.addEventListener("click",()=>{

window.scrollTo({
top:0,
behavior:"smooth"
});

});

</script>

</body>
</html>
