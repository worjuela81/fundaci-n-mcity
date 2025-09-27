<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <!-- Título completo de la fundación -->
    <title>Fundación M City S.S por Colombia</title>
    <!-- Carga de Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@100..900&display=swap" rel="stylesheet">
    <style>
        /* Definición de la fuente y colores base */
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f7f7f7; /* Fondo ligero */
        }
        
        /* ESTILO APLICADO A LA IMAGEN DE FONDO DEL HERO SECTION */
        .hero-section {
            /* Usamos la imagen subida IMG-20250917-WA0006.jpg como fondo */
            background: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.5)), url('IMG-20250917-WA0006.jpg');
            background-size: cover;
            background-position: center;
            background-attachment: fixed; /* Efecto Parallax ligero para el Hero */
        }
        
        /* Estilo para el botón principal de donación (sombra azul) */
        .donate-button {
            transition: all 0.3s ease;
        }
        .donate-button:hover {
            transform: translateY(-2px);
            /* Sombra del color principal (azul) */
            box-shadow: 0 10px 20px rgba(37, 99, 235, 0.4);
        }

        /* Estilo para dar más realce al texto sobre la imagen */
        .shadow-text {
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.6);
        }

        /* Estilos para los botones flotantes de Contacto Rápido */
        .floating-btn-container {
            position: fixed;
            bottom: 20px;
            right: 20px;
            z-index: 1000;
            display: flex;
            flex-direction: column;
            gap: 15px; /* Espacio entre los botones */
        }
        .floating-btn {
            width: 60px;
            height: 60px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .floating-btn:hover {
            transform: scale(1.05);
            box-shadow: 0 6px 15px rgba(0, 0, 0, 0.3);
        }

        .whatsapp-btn {
            background-color: #25d366; /* Verde WhatsApp */
        }
        .facebook-btn {
            background-color: #1877f2; /* Azul Facebook */
        }
        
        /* Estilo para el botón de Instagram con gradiente */
        .instagram-btn {
            background: radial-gradient(circle at 30% 107%, #fdf497 0%, #fdf497 5%, #fd5949 45%, #d6249f 60%, #285AEB 90%);
        }
    </style>
</head>
<body>

    <!-- Encabezado y Navegación -->
    <header class="sticky top-0 z-50 bg-white shadow-md">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center py-4 md:justify-start md:space-x-10">
                <!-- Logo de la Fundación (Nombre completo) -->
                <div class="flex justify-start lg:w-0 lg:flex-1">
                    <a href="#" class="text-xl font-bold text-blue-700 tracking-wider rounded-lg p-2 hover:bg-blue-50">
                        <span class="text-3xl font-extrabold text-blue-500">F</span>undación M City S.S por Colombia
                    </a>
                </div>
                <!-- Menú de Navegación -->
                <nav class="hidden md:flex space-x-10">
                    <a href="#inicio" class="text-base font-medium text-gray-500 hover:text-blue-600 rounded-md p-2 transition duration-150 ease-in-out">Inicio</a>
                    <a href="#quienes-somos" class="text-base font-medium text-gray-500 hover:text-blue-600 rounded-md p-2 transition duration-150 ease-in-out">Quiénes Somos</a>
                    <a href="#programas" class="text-base font-medium text-gray-500 hover:text-blue-600 rounded-md p-2 transition duration-150 ease-in-out">Programas</a>
                    <a href="#galeria" class="text-base font-medium text-gray-500 hover:text-blue-600 rounded-md p-2 transition duration-150 ease-in-out">Galería</a>
                    <a href="#contacto" class="text-base font-medium text-gray-500 hover:text-blue-600 rounded-md p-2 transition duration-150 ease-in-out">Contacto</a>
                </nav>
                <!-- Botón de Donación (Call to Action principal) - Color azul -->
                <div class="hidden md:flex items-center justify-end md:flex-1 lg:w-0">
                    <a href="#donar" class="ml-8 whitespace-nowrap inline-flex items-center justify-center px-4 py-2 border border-transparent rounded-full shadow-lg text-base font-medium text-white bg-blue-600 hover:bg-blue-700 donate-button">
                        Donar Ahora
                    </a>
                </div>
            </div>
        </div>
    </header>

    <main>
        <!-- Sección Principal (Hero) -->
        <section id="inicio" class="hero-section min-h-[80vh] flex items-center justify-center text-center py-20">
            <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
                <h1 class="text-5xl md:text-6xl font-extrabold tracking-tight text-white mb-4 shadow-text">
                    Transformamos vidas, creamos futuro.
                </h1>
                <p class="text-xl md:text-2xl text-gray-200 mb-8 font-light max-w-2xl mx-auto shadow-text">
                    Nuestra misión es empoderar a las comunidades más vulnerables a través de la educación y el desarrollo sostenible.
                </p>
                <!-- Botón principal en rojo vibrante -->
                <a href="#donar" class="inline-flex items-center justify-center px-8 py-4 border border-transparent text-lg font-bold rounded-full shadow-xl text-white bg-red-600 hover:bg-red-700 donate-button">
                    ¡Sé parte del cambio!
                </a>
            </div>
        </section>

        <!-- Sección Quiénes Somos / Nuestra Misión -->
        <section id="quienes-somos" class="py-16 md:py-24 bg-white">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="lg:grid lg:grid-cols-2 lg:gap-12 items-center">
                    <!-- Contenido de texto -->
                    <div class="mb-10 lg:mb-0">
                        <!-- Título azul -->
                        <h2 class="text-sm font-semibold text-blue-600 uppercase tracking-wide">
                            NUESTRA HISTORIA Y VALORES
                        </h2>
                        <p class="mt-2 text-3xl md:text-4xl font-extrabold text-gray-900 tracking-tight sm:text-4xl">
                            Comprometidos con el impacto positivo en la región.
                        </p>
                        <p class="mt-4 text-lg text-gray-600">
                            Desde el inicio, hemos trabajado incansablemente para cerrar las brechas de desigualdad en Colombia. Creemos en la **transparencia**, la **colaboración comunitaria** y la **sostenibilidad** como pilares para lograr un impacto duradero. Cada donación se traduce directamente en oportunidades reales.
                        </p>
                        <!-- Tags en azul -->
                        <div class="mt-6 flex flex-wrap gap-4">
                            <span class="inline-flex items-center px-3 py-1 rounded-full text-sm font-medium bg-blue-100 text-blue-800">
                                Transparencia
                            </span>
                            <span class="inline-flex items-center px-3 py-1 rounded-full text-sm font-medium bg-blue-100 text-blue-800">
                                Sostenibilidad
                            </span>
                            <span class="inline-flex items-center px-3 py-1 rounded-full text-sm font-medium bg-blue-100 text-blue-800">
                                Comunidad
                            </span>
                        </div>
                    </div>
                    <!-- Imagen de impacto real (IMG-20250917-WA0014.jpg) -->
                    <div class="relative">
                        <img class="w-full h-80 object-cover rounded-xl shadow-2xl" 
                             src="IMG-20250917-WA0014.jpg" 
                             alt="Miembro de la fundación entregando útiles escolares a niños sonrientes en Colombia."
                             onerror="this.onerror=null; this.src='https://placehold.co/600x400/10b981/ffffff?text=Comunidad+Beneficiada'">
                        <!-- Overlay azul -->
                        <div class="absolute inset-0 bg-blue-600 opacity-20 rounded-xl"></div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Sección Nuestros Programas -->
        <section id="programas" class="py-16 md:py-24 bg-gray-50">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
                <!-- Subtítulo azul -->
                <h2 class="text-sm font-semibold text-blue-600 uppercase tracking-wide">
                    ÁREAS DE ENFOQUE
                </h2>
                <p class="mt-2 text-3xl md:text-4xl font-extrabold text-gray-900">
                    Conoce nuestros pilares de acción
                </p>
                <p class="mt-4 text-xl text-gray-600 max-w-3xl mx-auto mb-12">
                    Nuestros programas están diseñados para generar un cambio sistémico y medible en la vida de las personas.
                </p>

                <!-- Tarjetas de Programas -->
                <div class="mt-10 grid grid-cols-1 gap-10 md:grid-cols-3">

                    <!-- Programa 1: Educación (Acento Rojo) -->
                    <div class="bg-white rounded-xl shadow-xl overflow-hidden p-6 hover:shadow-2xl transition duration-300">
                        <div class="flex items-center justify-center w-12 h-12 rounded-full bg-red-100 text-red-600 mb-4 mx-auto">
                            <!-- Icono de Libro -->
                            <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 6.253v13m0-13C10.832 5.477 9.246 5 7.5 5S4.168 5.477 3 6.253v13C4.168 18.477 5.754 18 7.5 18s3.332.477 4.5 1.253m0-13C13.168 5.477 14.754 5 16.5 5s3.332.477 4.5 1.253v13C19.832 18.477 18.246 18 16.5 18s-3.332.477-4.5 1.253"></path></svg>
                        </div>
                        <h3 class="text-xl font-bold text-gray-900 mb-3">Educación de Calidad</h3>
                        <p class="text-gray-600">
                            Provisión de útiles, construcción de escuelas, becas para estudiantes y capacitación docente en zonas rurales.
                        </p>
                    </div>

                    <!-- Programa 2: Salud (Acento Rojo) -->
                    <div class="bg-white rounded-xl shadow-xl overflow-hidden p-6 hover:shadow-2xl transition duration-300">
                        <div class="flex items-center justify-center w-12 h-12 rounded-full bg-red-100 text-red-600 mb-4 mx-auto">
                            <!-- Icono de Corazón -->
                            <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4.318 6.318a4.5 4.5 0 000 6.364L12 20.364l7.682-7.682a4.5 4.5 0 00-6.364-6.364L12 7.636l-1.318-1.318a4.5 4.5 0 00-6.364 0z"></path></svg>
                        </div>
                        <h3 class="text-xl font-bold text-gray-900 mb-3">Acceso a la Salud</h3>
                        <p class="text-gray-600">
                            Jornadas médicas gratuitas, suministro de medicamentos esenciales y campañas de prevención.
                        </p>
                    </div>

                    <!-- Programa 3: Sostenibilidad (Acento Azul) -->
                    <div class="bg-white rounded-xl shadow-xl overflow-hidden p-6 hover:shadow-2xl transition duration-300">
                        <div class="flex items-center justify-center w-12 h-12 rounded-full bg-blue-100 text-blue-600 mb-4 mx-auto">
                            <!-- Icono de Planta -->
                            <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z"></path></svg>
                        </div>
                        <h3 class="text-xl font-bold text-gray-900 mb-3">Desarrollo Sostenible</h3>
                        <p class="text-gray-600">
                            Proyectos de agricultura ecológica, promoción de energías renovables y emprendimiento local.
                        </p>
                    </div>

                </div>
            </div>
        </section>
        
        <!-- Sección de Galería de Impacto -->
        <section id="galeria" class="py-16 md:py-24 bg-white">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
                <h2 class="text-sm font-semibold text-red-600 uppercase tracking-wide">
                    NUESTRO TRABAJO EN ACCIÓN
                </h2>
                <p class="mt-2 text-3xl md:text-4xl font-extrabold text-gray-900">
                    Momentos que Transforman
                </p>
                <p class="mt-4 text-xl text-gray-600 max-w-3xl mx-auto mb-12">
                    Una mirada a la alegría y el impacto que generamos en las comunidades de Colombia.
                </p>

                <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6">
                    <!-- Fila 1 -->
                    <div class="relative overflow-hidden rounded-xl shadow-xl">
                        <img class="w-full h-64 object-cover transition duration-500 ease-in-out transform hover:scale-105" 
                             src="IMG-20250917-WA0037.jpg" 
                             alt="Miembro de la fundación repartiendo alimentos a una gran multitud de niños en un asentamiento">
                        <div class="absolute inset-0 bg-blue-900 bg-opacity-30 flex items-end p-4"><p class="text-white font-semibold text-lg">Jornadas Comunitarias</p></div>
                    </div>
                    <div class="relative overflow-hidden rounded-xl shadow-xl">
                        <img class="w-full h-64 object-cover transition duration-500 ease-in-out transform hover:scale-105" 
                             src="IMG-20250917-WA0041.jpg" 
                             alt="Vista panorámica de una gran cantidad de niños y familias en un evento comunitario al aire libre">
                        <div class="absolute inset-0 bg-blue-900 bg-opacity-30 flex items-end p-4"><p class="text-white font-semibold text-lg">Fortalecimiento Comunitario</p></div>
                    </div>
                    <div class="relative overflow-hidden rounded-xl shadow-xl">
                        <img class="w-full h-64 object-cover transition duration-500 ease-in-out transform hover:scale-105" 
                             src="IMG-20250917-WA0015.jpg" 
                             alt="Entrega cercana de kits escolares a niñas con uniformes en un patio de escuela">
                        <div class="absolute inset-0 bg-blue-900 bg-opacity-30 flex items-end p-4"><p class="text-white font-semibold text-lg">Regreso a Clases</p></div>
                    </div>

                    <!-- Fila 2 -->
                    <div class="relative overflow-hidden rounded-xl shadow-xl">
                        <img class="w-full h-64 object-cover transition duration-500 ease-in-out transform hover:scale-105" 
                             src="IMG-20250917-WA0008.jpg" 
                             alt="Entrega de útiles escolares a un grupo de niños en fila">
                        <div class="absolute inset-0 bg-blue-900 bg-opacity-30 flex items-end p-4"><p class="text-white font-semibold text-lg">Apoyo a la Educación</p></div>
                    </div>
                    <div class="relative overflow-hidden rounded-xl shadow-xl">
                        <img class="w-full h-64 object-cover transition duration-500 ease-in-out transform hover:scale-105" 
                             src="IMG-20250917-WA0009.jpg" 
                             alt="Niños sonrientes posando con sus kits escolares en un entorno rural">
                        <div class="absolute inset-0 bg-blue-900 bg-opacity-30 flex items-end p-4"><p class="text-white font-semibold text-lg">Futuro Brillante</p></div>
                    </div>
                    <div class="relative overflow-hidden rounded-xl shadow-xl">
                        <img class="w-full h-64 object-cover transition duration-500 ease-in-out transform hover:scale-105" 
                             src="IMG-20250917-WA0010.jpg" 
                             alt="Niños recibiendo paquetes de ayuda con alegría">
                        <div class="absolute inset-0 bg-blue-900 bg-opacity-30 flex items-end p-4"><p class="text-white font-semibold text-lg">Entrega de Alegría</p></div>
                    </div>

                    <!-- Fila 3 -->
                    <div class="relative overflow-hidden rounded-xl shadow-xl">
                        <img class="w-full h-64 object-cover transition duration-500 ease-in-out transform hover:scale-105" 
                             src="IMG-20250917-WA0011.jpg" 
                             alt="Un grupo de niños posando en un aula con útiles nuevos">
                        <div class="absolute inset-0 bg-blue-900 bg-opacity-30 flex items-end p-4"><p class="text-white font-semibold text-lg">Materiales Escolares</p></div>
                    </div>
                    <div class="relative overflow-hidden rounded-xl shadow-xl">
                        <img class="w-full h-64 object-cover transition duration-500 ease-in-out transform hover:scale-105" 
                             src="IMG-20250917-WA0012.jpg" 
                             alt="Niños sosteniendo sus útiles y sonriendo">
                        <div class="absolute inset-0 bg-blue-900 bg-opacity-30 flex items-end p-4"><p class="text-white font-semibold text-lg">El Poder de la Sonrisa</p></div>
                    </div>
                    <div class="relative overflow-hidden rounded-xl shadow-xl">
                        <!-- Reutilizamos la imagen de la hero section aquí para completar la cuadrícula, mostrando el rostro de la misión. -->
                        <img class="w-full h-64 object-cover transition duration-500 ease-in-out transform hover:scale-105" 
                             src="IMG-20250917-WA0006.jpg" 
                             alt="Representante de la fundación con niños en un aula">
                        <div class="absolute inset-0 bg-blue-900 bg-opacity-30 flex items-end p-4"><p class="text-white font-semibold text-lg">Nuestra Misión</p></div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Sección de Llamada a la Acción (Donar/Colaborar) -->
        <!-- Fondo azul oscuro -->
        <section id="donar" class="bg-blue-700 py-16 md:py-20">
            <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
                <h2 class="text-3xl md:text-5xl font-extrabold text-white tracking-tight mb-4">
                    Tu apoyo transforma vidas.
                </h2>
                <!-- Texto complementario azul claro -->
                <p class="text-xl text-blue-200 mb-8 max-w-2xl mx-auto">
                    Cada aporte nos permite llevar esperanza y herramientas a quienes más lo necesitan. ¡Únete a nuestra causa hoy!
                </p>
                <div class="flex flex-col sm:flex-row justify-center space-y-4 sm:space-y-0 sm:space-x-6">
                    <!-- Botón de Donación (Rojo Fuerte) -->
                    <a href="#" class="w-full sm:w-auto inline-flex items-center justify-center px-10 py-4 border border-transparent text-xl font-bold rounded-full shadow-2xl text-white bg-red-600 hover:bg-red-700 donate-button">
                        Donar con Tarjeta
                    </a>
                    <!-- Botón de Voluntariado (Borde blanco, hover azul) -->
                    <a href="#" class="w-full sm:w-auto inline-flex items-center justify-center px-10 py-4 border-2 border-white text-xl font-bold rounded-full text-white hover:bg-white hover:text-blue-700 transition duration-300">
                        Ser Voluntario
                    </a>
                </div>
            </div>
        </section>

        <!-- Sección de Contacto -->
        <section id="contacto" class="py-16 md:py-24 bg-gray-50">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                <!-- Subtítulos azules -->
                <h2 class="text-sm font-semibold text-blue-600 uppercase tracking-wide text-center">
                    MANTENTE EN CONTACTO
                </h2>
                <p class="mt-2 text-3xl md:text-4xl font-extrabold text-gray-900 text-center mb-12">
                    Conversemos sobre cómo colaborar
                </p>

                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                    <!-- Información de Contacto -->
                    <div class="bg-white p-6 rounded-xl shadow-lg">
                        <!-- Título azul -->
                        <h3 class="text-xl font-bold text-blue-700 mb-3">Oficina Principal</h3>
                        <p class="text-gray-600">
                            Dirección: Cr4 número 20h04 barrio Las palmas valledupar Colombia
                        </p>
                        <!-- Número del CEO Neftali Silva -->
                        <p class="text-gray-600 font-semibold">
                            CEO Neftali Silva: <a href="tel:+573045912252" class="text-red-600 hover:text-red-800 transition duration-150">+57 304 591 2252</a>
                        </p>
                        <p class="text-gray-600">
                            <!-- Correo Electrónico ACTUALIZADO -->
                            Email: <a href="mailto:mcityss222@gmail.com" class="text-blue-600 hover:text-blue-800">mcityss222@gmail.com</a>
                        </p>
                    </div>

                    <!-- Horarios -->
                    <div class="bg-white p-6 rounded-xl shadow-lg">
                        <!-- Título azul -->
                        <h3 class="text-xl font-bold text-blue-700 mb-3">Horario de Atención</h3>
                        <p class="text-gray-600">
                            Lunes a Viernes: 9:00 AM - 5:00 PM
                        </p>
                        <p class="text-gray-600">
                            Sábados: 10:00 AM - 1:00 PM
                        </p>
                        <p class="text-gray-600">
                            Domingos: Cerrado
                        </p>
                    </div>

                    <!-- Redes Sociales -->
                    <div class="bg-white p-6 rounded-xl shadow-lg">
                        <!-- Título azul -->
                        <h3 class="text-xl font-bold text-blue-700 mb-3">Síguenos</h3>
                        <div class="flex space-x-4 mt-3">
                            <!-- Facebook (Placeholder) -->
                            <a href="#" class="text-blue-600 hover:text-blue-800 transition duration-150" aria-label="Facebook">
                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="currentColor"><path d="M14 11h-2v-3h2v3zm0 4h-2v-2h2v2zm7 0h-2v-2h2v2zm0 4h-2v-2h2v2zm-4 0h-2v-2h2v2zm-4 0h-2v-2h2v2zm-4 0h-2v-2h2v2zm-4 0h-2v-2h2v2zm0-4h-2v-2h2v2zm0-4h-2v-2h2v2zm0-4h-2v-2h2v2zm4 8h-2v-2h2v2zM5 19v-2h2v2H5zm0-4h2v2H5zm0-4h2v2H5zm0-4h2v2H5zm4-4h2v2H9zM7 3h10a4 4 0 014 4v10a4 4 0 01-4 4H7a4 4 0 01-4-4V7a4 4 0 014-4z"/></svg>
                            </a>
                            <!-- X (Twitter - Placeholder) -->
                            <a href="#" class="text-blue-600 hover:text-blue-800 transition duration-150" aria-label="Twitter/X">
                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="currentColor"><path d="M18.84 6.185c.98-.67 1.83-1.5 2.5-2.45-.88.52-1.85.9-2.88 1.09.8-.48 1.4-1.2 1.69-2.07-.8.47-1.68.81-2.6 1.01-.8-.85-1.95-1.38-3.23-1.38-2.43 0-4.4 1.96-4.4 4.38 0 .34.04.67.11 1-.36-.02-.73-.07-1.09-.12-3.65-.2-6.88-1.94-9.1-4.6-.37.64-.58 1.4-.58 2.2 0 1.5.76 2.84 1.94 3.63-.67-.02-1.3-.2-1.86-.5v.06c0 2.1 1.5 3.86 3.5 4.26-.37.1-.75.15-1.15.15-.28 0-.55-.03-.8-.08.57 1.73 2.17 3 4.07 3.03-1.5 1.18-3.4 1.87-5.46 1.87-.36 0-.7-.02-1.04-.07 1.94 1.25 4.25 1.97 6.7 1.97 8.04 0 12.44-6.68 12.44-12.44 0-.19-.01-.38-.01-.58.85-.62 1.57-1.38 2.15-2.28z"/></svg>
                            </a>
                            <!-- Instagram (Enlace real) -->
                            <a href="https://www.instagram.com/fundacionmcitys.s/" target="_blank" rel="noopener noreferrer" class="text-blue-600 hover:text-blue-800 transition duration-150" aria-label="Instagram">
                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="currentColor"><path d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.204-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.069-4.849.069-3.204 0-3.584-.012-4.849-.069-3.251-.148-4.771-1.691-4.919-4.919-.058-1.265-.068-1.644-.068-4.849 0-3.204.012-3.584.069-4.849.149-3.225 1.664-4.771 4.919-4.919 1.266-.057 1.645-.068 4.849-.068zm0 5.838a6.162 6.162 0 100 12.324 6.162 6.162 0 000-12.324zm0 10.324a4.162 4.162 0 110-8.324 4.162 4.162 0 010 8.324zm6.27-8.374c-.655 0-1.188.533-1.188 1.188s.533 1.188 1.188 1.188 1.188-.533 1.188-1.188-.533-1.188-1.188-1.188z"/></svg>
                            </a>
                        </div>
                    </div>
                </div>
            </div>
        </section>

    </main>

    <!-- Pie de Página (Footer) -->
    <footer class="bg-gray-800">
        <div class="max-w-7xl mx-auto py-8 px-4 sm:px-6 lg:px-8">
            <div class="md:flex md:justify-between md:items-center">
                <div class="text-center md:text-left">
                    <p class="text-sm text-gray-400">&copy; 2024 Fundación M City S.S por Colombia. Todos los derechos reservados.</p>
                </div>
                <div class="mt-4 md:mt-0 flex justify-center space-x-6">
                    <!-- Enlaces del footer azules -->
                    <a href="#inicio" class="text-sm text-gray-400 hover:text-blue-400">Política de Privacidad</a>
                    <a href="#inicio" class="text-sm text-gray-400 hover:text-blue-400">Términos de Uso</a>
                </div>
            </div>
        </div>
    </footer>

    <!-- Botones Flotantes de Contacto Rápido (Instagram, WhatsApp, Facebook) -->
    <div class="floating-btn-container">
        
        <!-- Instagram Button -->
        <a href="https://www.instagram.com/fundacionmcitys.s/" 
           target="_blank" 
           rel="noopener noreferrer" 
           aria-label="Seguir en Instagram"
           class="floating-btn instagram-btn">
           <!-- Icono de Instagram (SVG simple) -->
           <svg xmlns="http://www.w3.org/2000/svg" class="w-8 h-8 text-white" viewBox="0 0 24 24" fill="currentColor"><path d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.204-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.069-4.849.069-3.204 0-3.584-.012-4.849-.069-3.251-.148-4.771-1.691-4.919-4.919-.058-1.265-.068-1.644-.068-4.849 0-3.204.012-3.584.069-4.849.149-3.225 1.664-4.771 4.919-4.919 1.266-.057 1.645-.068 4.849-.068zm0 1.838c-3.15 0-3.541.012-4.717.067-2.735.124-3.957 1.402-4.081 4.081-.055 1.176-.067 1.566-.067 4.717s.012 3.541.067 4.717c.124 2.679 1.346 3.957 4.081 4.081 1.176.055 1.566.067 4.717.067s3.541-.012 4.717-.067c2.679-.124 3.957-1.346 4.081-4.081.055-1.176.067-1.566.067-4.717s-.012-3.541-.067-4.717c-.124-2.679-1.346-3.957-4.081-4.081-1.176-.055-1.566-.067-4.717-0.067zm0 5.838c-2.485 0-4.5 2.015-4.5 4.5s2.015 4.5 4.5 4.5 4.5-2.015 4.5-4.5-2.015-4.5-4.5-4.5zm0 7c-1.38 0-2.5-1.12-2.5-2.5s1.12-2.5 2.5-2.5 2.5 1.12 2.5 2.5-1.12 2.5-2.5 2.5zm6.5-10.5c0-.552.447-1 1-1s1 .448 1 1v.008c0 .552-.447 1-1 1s-1-.448-1-1v-.008z"/></svg>
        </a>

        <!-- WhatsApp Button (Con el número de Neftali Silva) -->
        <a href="https://wa.me/+573045912252?text=Hola%2C%20estoy%20interesado%20en%20conocer%20m%C3%A1s%20sobre%20la%20Fundaci%C3%B3n%20M%20City%20S.S." 
           target="_blank" 
           rel="noopener noreferrer" 
           aria-label="Contactar por WhatsApp"
           class="floating-btn whatsapp-btn">
           <!-- Icono de WhatsApp (SVG simple) -->
           <svg xmlns="http://www.w3.org/2000/svg" class="w-8 h-8 text-white" viewBox="0 0 24 24" fill="currentColor"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zM9.5 16.5c-.3 0-.54-.12-.75-.36l-1.92-2.14c-.19-.21-.29-.46-.29-.75s.1-.54.29-.75l1.92-2.14c.21-.24.45-.36.75-.36s.54.12.75.36l1.92 2.14c.19.21.29.46.29.75s-.1.54-.29.75l-1.92 2.14c-.21.24-.45.36-.75.36zm4.5-3.5h-2v-1h2v1z"/></svg>
        </a>

        <!-- Facebook Messenger Button (Placeholder) -->
        <a href="https://m.me/NombreDeTuPaginaDeFacebook" 
           target="_blank" 
           rel="noopener noreferrer" 
           aria-label="Contactar por Facebook Messenger"
           class="floating-btn facebook-btn">
            <!-- Icono de Facebook Messenger (SVG simple) -->
            <svg xmlns="http://www.w3.org/2000/svg" class="w-8 h-8 text-white" viewBox="0 0 24 24" fill="currentColor"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm1 14h-2v-2h2v2zm0-4h-2V7h2v5z"/></svg>
        </a>
    </div>

</body>
</html>
