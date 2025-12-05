<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<title>Galería de Arte Interactiva</title>

<style>
    body {
        font-family: Arial, sans-serif;
        background: #f3f4f7;
        margin: 0;
        padding: 20px;
    }

    h1 {
        text-align: center;
        margin-bottom: 40px;
    }

    /* CONTENEDOR DE GALERÍAS */
    .section {
        margin-bottom: 60px;
    }

    h2 {
        margin-bottom: 15px;
        border-left: 5px solid #4a86e8;
        padding-left: 10px;
    }

    /* SLIDER */
    .gallery-container {
        position: relative;
        width: 100%;
        max-width: 720px;
        margin: 0 auto;
        overflow: hidden;
        border-radius: 12px;
        box-shadow: 0 0 15px rgba(0,0,0,0.15);
        background: white;
    }

    .slides {
        display: flex;
        transition: transform 0.5s ease-in-out;
    }

    .slide {
        min-width: 100%;
        box-sizing: border-box;
        padding: 20px;
        text-align: center;
    }

    .slide img {
        width: 90%;
        max-height: 400px;
        border-radius: 10px;
        object-fit: cover;
    }

    .info-box {
        background: #eef3f7;
        padding: 15px;
        margin-top: 15px;
        border-radius: 8px;
        text-align: left;
    }

    /* BOTONES SLIDER */
    .btn {
        position: absolute;
        top: 50%;
        transform: translateY(-50%);
        background: rgba(0,0,0,0.5);
        color: white;
        border: none;
        padding: 15px;
        cursor: pointer;
        border-radius: 50%;
        font-size: 18px;
    }
    .btn:hover {
        background: rgba(0,0,0,0.7);
    }

    .prev { left: 10px; }
    .next { right: 10px; }

</style>
</head>

<body>

<h1>Galería Interactiva de Arte</h1>

<!-- =======================================================
                   VAN GOGH — GALERÍA
======================================================= -->
<div class="section">
    <h2>Vincent van Gogh</h2>

    <div class="gallery-container" id="vangogh-gallery">
        <button class="btn prev" onclick="prevSlide('vangogh')">❮</button>
        <button class="btn next" onclick="nextSlide('vangogh')">❯</button>

        <div class="slides" id="vangogh-slides">

            <!-- LA NOCHE ESTRELLADA -->
            <div class="slide">
                <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/ef/The_Starry_Night.jpg/640px-The_Starry_Night.jpg">
                <div class="info-box">
                    <h3>La noche estrellada (1889)</h3>
                    <p><strong>Autor:</strong> Vincent van Gogh</p>
                    <p><strong>Técnica:</strong> Óleo sobre lienzo</p>
                    <p><strong>Lugar actual:</strong> Museo de Arte Moderno (MoMA), Nueva York</p>
                    <p>Considerada una de las pinturas más influyentes del arte occidental, representa un cielo turbulento y lleno de energía que refleja el estado emocional del artista mientras estaba internado en Saint-Rémy-de-Provence.</p>
                </div>
            </div>

            <!-- LOS GIRASOLES -->
            <div class="slide">
                <img src="https://upload.wikimedia.org/wikipedia/commons/4/47/Vincent_Willem_van_Gogh_128.jpg">
                <div class="info-box">
                    <h3>Los girasoles (1888)</h3>
                    <p><strong>Técnica:</strong> Óleo sobre lienzo</p>
                    <p><strong>Lugar actual:</strong> National Gallery, Londres</p>
                    <p>Esta serie muestra la fascinación de Van Gogh por los colores vibrantes y la luz del sur de Francia. Es una de las colecciones más reconocidas del posimpresionismo.</p>
                </div>
            </div>

            <!-- NOCHE ESTRELLADA SOBRE EL RÓDANO -->
            <div class="slide">
                <img src="https://upload.wikimedia.org/wikipedia/commons/7/76/Starry_Night_Over_the_Rhone.jpg">
                <div class="info-box">
                    <h3>Noche estrellada sobre el Ródano (1888)</h3>
                    <p><strong>Técnica:</strong> Óleo sobre lienzo</p>
                    <p><strong>Lugar actual:</strong> Museo de Orsay, París</p>
                    <p>Una de las primeras exploraciones del cielo nocturno por parte de Van Gogh, con reflejos luminosos sobre el río Ródano.</p>
                </div>
            </div>

        </div>
    </div>
</div>

<!-- =======================================================
                   MAGRITTE — GALERÍA
======================================================= -->
<div class="section">
    <h2>René Magritte</h2>

    <div class="gallery-container" id="magritte-gallery">
        <button class="btn prev" onclick="prevSlide('magritte')">❮</button>
        <button class="btn next" onclick="nextSlide('magritte')">❯</button>

        <div class="slides" id="magritte-slides">

            <!-- EL HIJO DEL HOMBRE -->
            <div class="slide">
                <img src="https://upload.wikimedia.org/wikipedia/en/0/0c/Magritte_TheSonOfMan.jpg">
                <div class="info-box">
                    <h3>El hijo del hombre (1964)</h3>
                    <p><strong>Autor:</strong> René Magritte</p>
                    <p><strong>Técnica:</strong> Óleo sobre lienzo</p>
                    <p><strong>Lugar actual:</strong> Colección privada</p>
                    <p>Un retrato icónico del surrealismo, donde el rostro del hombre es ocultado por una manzana verde, explorando el misterio de lo visible y lo oculto.</p>
                </div>
            </div>

            <!-- LA TRAICIÓN DE LAS IMÁGENES -->
            <div class="slide">
                <img src="https://upload.wikimedia.org/wikipedia/en/b/b9/MagrittePipe.jpg">
                <div class="info-box">
                    <h3>La traición de las imágenes (1929)</h3>
                    <p><strong>Técnica:</strong> Óleo sobre lienzo</p>
                    <p><strong>Lugar actual:</strong> Museo de Arte del Condado de Los Ángeles</p>
                    <p>Famoso por la frase “Esto no es una pipa”, desafía la relación entre objetos y representaciones.</p>
                </div>
            </div>

            <!-- LOS AMANTES -->
            <div class="slide">
                <img src="https://upload.wikimedia.org/wikipedia/en/0/0a/The_Lovers_(Magritte).jpg">
                <div class="info-box">
                    <h3>Los amantes (1928)</h3>
                    <p><strong>Técnica:</strong> Óleo sobre lienzo</p>
                    <p><strong>Lugar actual:</strong> MoMA, Nueva York</p>
                    <p>Dos figuras besándose con telas que cubren sus rostros; un símbolo de la incomunicación y la imposibilidad de conocer totalmente a otra persona.</p>
                </div>
            </div>

        </div>
    </div>
</div>

<script>
const indexes = { vangogh: 0, magritte: 0 };

function updateSlide(artist) {
    const slideContainer = document.getElementById(artist + "-slides");
    const slides = slideContainer.children.length;
    slideContainer.style.transform = "translateX(" + (-indexes[artist] * 100) + "%)";
}

function nextSlide(artist) {
    const slideContainer = document.getElementById(artist + "-slides");
    const slides = slideContainer.children.length;
    indexes[artist] = (indexes[artist] + 1) % slides;
    updateSlide(artist);
}

function prevSlide(artist) {
    const slideContainer = document.getElementById(artist + "-slides");
    const slides = slideContainer.children.length;
    indexes[artist] = (indexes[artist] - 1 + slides) % slides;
    updateSlide(artist);
}
</script>

</body>
</html>
