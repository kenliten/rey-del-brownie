<!DOCTYPE html>
<html lang="es">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rey del Brownie - El Brownie Perfecto para Cada Momento</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Font Inter from Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
    <!-- Font Awesome for social media icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.1.1/css/all.min.css">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #fcf8f6;
            /* Soft off-white background */
        }

        .text-shadow-dark {
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
        }

        .card-hover {
            transition: transform 0.3s ease-in-out, box-shadow 0.3s ease-in-out;
        }

        .card-hover:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
        }

        /* Custom styles for social icons */
        .social-icon {
            transition: color 0.3s ease-in-out;
        }

        .social-icon:hover {
            color: #d2b48c;
            /* Lighter stone/beige on hover */
        }
    </style>
</head>

<body class="text-gray-800">

    <!-- Header Section -->
    <header class="bg-white/70 backdrop-blur-md sticky top-0 z-50 shadow-sm">
        <div class="container mx-auto px-6 py-4 flex justify-between items-center">
            <a href="#" class="flex items-center space-x-2">
                <!-- Placeholder for the Rey del Brownie Logo -->
                <img src="./logo.jpg" alt="Rey del Brownie Logo"
                    class="h-10">
            </a>
            <nav class="hidden md:block">
                <ul class="flex space-x-8 text-lg font-semibold">
                    <li><a href="#flavors"
                            class="text-gray-700 hover:text-stone-600 transition-colors duration-300">Sabores</a></li>
                    <li><a href="#stats"
                            class="text-gray-700 hover:text-stone-600 transition-colors duration-300">Nuestros
                            Números</a></li>
                    <li><a href="#testimonials"
                            class="text-gray-700 hover:text-stone-600 transition-colors duration-300">Testimonios</a>
                    </li>
                    <li><a href="#contact-cta"
                            class="bg-stone-600 text-white py-2 px-4 rounded-full hover:bg-stone-700 transition-colors duration-300">Comprar
                            Ahora</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <main>
        <!-- Hero Section -->
        <section class="relative bg-gradient-to-br from-amber-100 to-rose-100 py-24 md:py-40 overflow-hidden">
            <div class="relative container mx-auto px-6 flex flex-col md:flex-row items-center gap-16">
                <div class="md:w-1/2 text-center md:text-left">
                    <h2 class="text-5xl md:text-7xl font-extrabold leading-tight mb-6 text-stone-800 text-shadow-dark">
                        La Felicidad tiene Sabor a Chocolate
                    </h2>
                    <p class="text-xl md:text-2xl font-light mb-10 text-gray-700">
                        Descubre nuestros brownies artesanales, hechos con pasión y los mejores ingredientes para
                        brindarte un momento de pura indulgencia.
                    </p>
                    <a href="#flavors"
                        class="inline-block bg-stone-600 text-white font-bold py-4 px-10 rounded-full shadow-lg hover:bg-stone-700 transform hover:scale-105 transition-all duration-300">
                        Explorar Nuestros Sabores
                    </a>
                </div>
                <div class="md:w-1/2 mt-12 md:mt-0 flex justify-center">
                    <img src="./pexels-jeshoots-3666.jpg"
                        alt="Un brownie con chocolate derretido y una cuchara"
                        class="rounded-3xl shadow-2xl transform rotate-3 hover:rotate-0 transition-transform duration-500 max-w-full h-auto">
                </div>
            </div>
        </section>

        <!-- Our Story Section -->
        <section id="about-us" class="py-24 bg-white">
            <div class="container mx-auto px-6 text-center md:text-left">
                <div class="md:grid md:grid-cols-2 md:gap-16 items-center">
                    <div class="order-2">
                        <img src="./ingredients.jpg"
                            alt="Ingredientes de brownie como cacao, chocolate y nueces"
                            class="rounded-3xl shadow-xl max-w-full h-auto">
                    </div>
                    <div class="mt-12 md:mt-0 order-1">
                        <h3 class="text-4xl md:text-5xl font-bold mb-6 text-stone-800">Nuestra Historia</h3>
                        <p class="text-lg md:text-xl max-w-xl text-gray-600">
                            En Rey del Brownie, creemos que un buen brownie es más que un postre; es una experiencia.
                            Comenzamos con una simple idea: crear el brownie perfecto. Cada lote es horneado con los
                            ingredientes más finos, desde cacao de origen hasta mantequilla real, para asegurar un sabor
                            y una textura inigualables.
                        </p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Flavors Section -->
        <section id="flavors" class="bg-fcf8f6 py-24">
            <div class="container mx-auto px-6">
                <h3 class="text-4xl md:text-5xl font-bold text-center mb-16 text-stone-800">Descubre Nuestros
                    Irresistibles Sabores</h3>
                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-12">
                    <!-- Flavor Card 1 -->
                    <div class="bg-white card-hover p-8 rounded-3xl border-l-4 border-stone-500">
                        <img src="./pexels-pixabay-45202.jpg" alt="Brownie Clásico"
                            class="rounded-2xl mb-6 w-full h-auto">
                        <h4 class="text-2xl font-semibold mb-2 text-center text-stone-800">El Clásico de Chocolate</h4>
                        <p class="text-center text-gray-600">El brownie original, con un sabor a chocolate intenso y una
                            textura suave y húmeda.</p>
                    </div>
                    <!-- Flavor Card 2 -->
                    <div class="bg-white card-hover p-8 rounded-3xl border-l-4 border-stone-500">
                        <img src="./pexels-karolina-grabowska-5386684.jpg"
                            alt="Brownie con Nueces" class="rounded-2xl mb-6 w-full h-auto">
                        <h4 class="text-2xl font-semibold mb-2 text-center text-stone-800">Con Nuez de la India</h4>
                        <p class="text-center text-gray-600">Nuestro clásico elevado, con el toque crujiente de nueces
                            recién tostadas.</p>
                    </div>
                    <!-- Flavor Card 3 -->
                    <div class="bg-white card-hover p-8 rounded-3xl border-l-4 border-stone-500">
                        <img src="./colored.jpg"
                            alt="Brownie de Chocolate Blanco" class="rounded-2xl mb-6 w-full h-auto">
                        <h4 class="text-2xl font-semibold mb-2 text-center text-stone-800">Tentación de Chocolate Blanco
                        </h4>
                        <p class="text-center text-gray-600">Una variante dulce y cremosa, perfecta para los amantes del
                            chocolate blanco.</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Stats Section -->
        <section id="stats" class="bg-white py-24">
            <div class="container mx-auto px-6 text-center">
                <h3 class="text-4xl md:text-5xl font-bold mb-16 text-stone-800">Nuestros Números Hablan por Sí Mismos
                </h3>
                <div class="grid grid-cols-1 md:grid-cols-3 gap-12">
                    <div class="flex flex-col items-center">
                        <span class="text-5xl md:text-6xl font-bold mb-2 text-stone-600">10,000+</span>
                        <p class="text-xl font-light text-gray-600">Brownies Vendidos al Mes</p>
                    </div>
                    <div class="flex flex-col items-center">
                        <span class="text-5xl md:text-6xl font-bold mb-2 text-stone-600">5+</span>
                        <p class="text-xl font-light text-gray-600">Provincias de Cobertura</p>
                    </div>
                    <div class="flex flex-col items-center">
                        <span class="text-5xl md:text-6xl font-bold mb-2 text-stone-600">99%</span>
                        <p class="text-xl font-light text-gray-600">Satisfacción del Cliente</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Testimonials Section -->
        <section id="testimonials" class="bg-stone-700 text-white py-24">
            <div class="container mx-auto px-6 text-center">
                <h3 class="text-4xl md:text-5xl font-bold mb-16">Lo que Nuestros Clientes Dicen</h3>
                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-12">
                    <!-- Testimonial 1 -->
                    <div class="bg-stone-800/70 p-8 rounded-2xl">
                        <p class="text-lg italic mb-4">"Simplemente los mejores brownies que he probado. La textura es
                            perfecta y el sabor es increíblemente intenso."</p>
                        <p class="font-semibold">- Ana G.</p>
                    </div>
                    <!-- Testimonial 2 -->
                    <div class="bg-stone-800/70 p-8 rounded-2xl">
                        <p class="text-lg italic mb-4">"Cada bocado es una delicia. Siempre pido para mis eventos y mis
                            invitados los aman."</p>
                        <p class="font-semibold">- Carlos P.</p>
                    </div>
                    <!-- Testimonial 3 -->
                    <div class="bg-stone-800/70 p-8 rounded-2xl">
                        <p class="text-lg italic mb-4">"Increíble calidad y un servicio excelente. Son mi nueva obsesión
                            de postre."</p>
                        <p class="font-semibold">- Sofía R.</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Final Call to Action Section -->
        <section id="contact-cta" class="bg-fcf8f6 py-24">
            <div class="container mx-auto px-6 text-center">
                <h3 class="text-4xl md:text-5xl font-bold mb-6 text-stone-800">¿Listo para un Momento Inolvidable?</h3>
                <p class="text-lg md:text-xl mb-8 text-gray-600">
                    Pide tus brownies ahora y déjanos endulzar tu día.
                </p>
                <a href="#"
                    class="inline-block bg-pink-500 text-white font-bold py-4 px-10 rounded-full shadow-lg hover:bg-pink-600 transform hover:scale-105 transition-all duration-300">
                    Comprar Ahora
                </a>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer class="bg-stone-800 text-gray-300 py-12">
        <div class="container mx-auto px-6">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8">
                <!-- Search Column -->
                <div class="col-span-1">
                    <h5 class="text-2xl font-bold mb-4 text-white">Búsqueda</h5>
                    <form action="#" method="get">
                        <div class="relative">
                            <input type="search" placeholder="Buscar..."
                                class="w-full bg-stone-700 text-white px-4 py-2 rounded-lg border border-stone-600 focus:outline-none focus:ring focus:ring-stone-500">
                            <button type="submit"
                                class="absolute right-0 top-0 mt-2 mr-4 text-gray-400 hover:text-white">
                                <i class="fas fa-search"></i>
                            </button>
                        </div>
                    </form>
                </div>

                <!-- Contact Column -->
                <div class="col-span-1">
                    <h5 class="text-2xl font-bold mb-4 text-white">Contacto</h5>
                    <address class="not-italic text-gray-400 space-y-2">
                        <p><i class="fas fa-map-marker-alt mr-2"></i> Calle Principal 123, Ciudad, País</p>
                        <p><i class="fas fa-phone mr-2"></i> (809) 305-9027</p>
                        <p><i class="fas fa-envelope mr-2"></i> contacto@reydelbrownie.com</p>
                    </address>
                </div>

                <!-- Useful Links Column -->
                <div class="col-span-1">
                    <h5 class="text-2xl font-bold mb-4 text-white">Enlaces Útiles</h5>
                    <ul class="text-gray-400 space-y-2">
                        <li><a href="#" class="hover:text-white transition-colors duration-300">Acerca de Nosotros</a>
                        </li>
                        <li><a href="#" class="hover:text-white transition-colors duration-300">Preguntas Frecuentes</a>
                        </li>
                        <li><a href="#" class="hover:text-white transition-colors duration-300">Términos y
                                Condiciones</a></li>
                        <li><a href="#" class="hover:text-white transition-colors duration-300">Política de
                                Privacidad</a></li>
                    </ul>
                </div>

                <!-- Social Media Column -->
                <div class="col-span-1">
                    <h5 class="text-2xl font-bold mb-4 text-white">Síguenos</h5>
                    <div class="flex space-x-6 text-2xl">
                        <a href="#" target="_blank" class="text-gray-400 social-icon"><i
                                class="fab fa-facebook-f"></i></a>
                        <a href="#" target="_blank" class="text-gray-400 social-icon"><i
                                class="fab fa-instagram"></i></a>
                        <a href="#" target="_blank" class="text-gray-400 social-icon"><i class="fab fa-twitter"></i></a>
                    </div>
                </div>
            </div>
            <div class="mt-12 text-center text-gray-500 border-t border-stone-700 pt-8">
                <p>&copy; 2024 Rey del Brownie. Todos los derechos reservados.</p>
            </div>
        </div>
    </footer>
</body>

</html>