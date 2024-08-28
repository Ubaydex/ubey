<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ubaydillah</title>
   <link href="./output.css" rel="stylesheet">
    <style>
        html {
            scroll-behavior: smooth;
        }
        .hover-tilt:hover {
            transform: scale(1.05);
            transition: transform 0.3s ease;
        }
        #about {
            scroll-margin-top: 64px; /* Sesuaikan dengan tinggi navbar */
        }
        /* Tambahkan CSS untuk hamburger menu */
        .mobile-menu {
            display: none;
        }
        @media (max-width: 768px) {
            .desktop-menu {
                display: none;
            }
            .mobile-menu {
                display: block;
            }
            #mobile-menu {
                display: none;
            }
            #mobile-menu.open {
                display: block;
            }
        }
    </style>
</head>
<body class="bg-blue-700">

    <!-- Navbar -->
    <nav class="bg-red-500 py-4 fixed w-full z-10">
        <div class="container mx-auto flex justify-between items-center px-6">
            <div class="text-2xl font-bold">Ubaydillah</div>
            <!-- Desktop Menu -->
            <ul class="desktop-menu flex space-x-6">
                <li><a href="#about" class="hover:text-indigo-200 transition">About</a></li>
                <li><a href="#portfolio" class="hover:text-indigo-200 transition">Portfolio</a></li>
                <li><a href="#contact" class="hover:text-indigo-200 transition">Contact</a></li>
            </ul>
            <!-- Hamburger Button -->
            <button id="hamburger-button" class="mobile-menu text-2xl focus:outline-none">
                <span class="sr-only">Open menu</span>
                &#9776;
            </button>
            <!-- Mobile Menu -->
            <div id="mobile-menu" class="mobile-menu absolute top-16 right-0 bg-gray-800 w-full text-center">
                <ul class="flex flex-col space-y-4 py-4">
                    <li><a href="#about" class="hover:text-indigo-200 transition">About</a></li>
                    <li><a href="#portfolio" class="hover:text-indigo-200 transition">Portfolio</a></li>
                    <li><a href="#contact" class="hover:text-indigo-200 transition">Contact</a></li>
                </ul>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="relative bg-gradient-to-r from-red-400 to-blue-500 text-center h-screen flex flex-col justify-center items-center">
        <img src="foto ku.jpeg" alt="Profile Photo" class="w-32 h-32 rounded-full object-cover mb-6 border-4 border-white mt-6">
        <h1 class="text-6xl font-extrabold">I student in Politeknik IDN</h1>
        <p class="mt-4 text-2xl">Junior Programin</p>
        <a href="#portfolio" class="mt-10 inline-block px-10 py-4 bg-indigo-600 text-white font-semibold rounded-lg shadow-md hover:bg-indigo-700 transition duration-300">Explore my litte Project</a>
        <div class="absolute inset-0 bg-gradient-to-b from-transparent to-gray-900 opacity-80 pointer-events-none"></div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-20 px-4 sm:px-6 lg:px-8 bg-green-700">
        <div class="max-w-4xl mx-auto text-center">
            <h2 class="text-4xl font-extrabold">About Me</h2>
            <p class="mt-6 text-lg text-gray-400">I'm Junior web Develotmen</p>
            <div class="mt-10 flex justify-center space-x-8">
                <img src="profil.jpg" alt="Skill 1" class="w-16 h-16">
                <img src="profil.jpg" alt="Skill 2" class="w-16 h-16">
                <img src="profil.jpg" alt="Skill 3" class="w-16 h-16">
                <img src="profil.jpg" alt="Skill 4" class="w-16 h-16">
            </div>
        </div>
    </section>

    <!-- Portfolio Section -->
    <section id="portfolio" class="py-20 bg-gray-900">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <h2 class="text-4xl font-extrabold text-center">My Portfolio</h2>
            <div class="mt-12 grid gap-10 grid-cols-1 sm:grid-cols-2 lg:grid-cols-3">
                <div class="bg-gray-800 rounded-lg shadow-lg overflow-hidden hover-tilt">
                    <img src="coffe projec.jpg" alt="Project 1" class="w-full h-56 object-cover">
                    <div class="p-6">
                        <h3 class="text-xl font-semibold">Project One</h3>
                        <p class="mt-4 text-gray-400">A project in the codecamp Training 2</p>
                    </div>
                </div>
                <div class="bg-gray-800 rounded-lg shadow-lg overflow-hidden hover-tilt">
                    <img src="projectkucing.jpg" alt="Project 2" class="w-full h-56 object-cover">
                    <div class="p-6">
                        <h3 class="text-xl font-semibold">Project Two</h3>
                        <p class="mt-4 text-gray-400">A Portofolio use the html and css</p>
                    </div>
                </div>
                <div class="bg-gray-800 rounded-lg shadow-lg overflow-hidden hover-tilt">
                    <img src="https://picsum.photos/200/302" alt="Project 3" class="w-full h-56 object-cover">
                    <div class="p-6">
                        <h3 class="text-xl font-semibold">Project Three</h3>
                        <p class="mt-4 text-gray-400">A Menu Coffe</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-20 bg-gray-800">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <h2 class="text-4xl font-extrabold">Contact Me</h2>
            <p class="mt-4 text-lg text-gray-400">I invite all of you to take a look at my simple portfolio but it has deep meaning in each project</p>
            <form action="#" method="POST" class="mt-8">
                <div class="grid gap-6 sm:grid-cols-2">
                    <input type="text" placeholder="Your Name" class="w-full px-4 py-3 bg-gray-700 border border-gray-600 rounded-lg focus:outline-none focus:border-indigo-500 
text-white">
                    <input type="email" placeholder="Your Email" class="w-full px-4 py-3 bg-gray-700 border border-gray-600 rounded-lg focus:outline-none focus:border-indigo-500 
text-white">
                </div>
                <textarea placeholder="Your Message" class="w-full mt-6 px-4 py-3 bg-gray-700 border border-gray-600 rounded-lg focus:outline-none focus:border-indigo-500 
text-white"></textarea>
                <button type="submit" class="mt-6 px-8 py-3 bg-indigo-600 text-white font-semibold rounded-lg shadow-md hover:bg-indigo-700 transition duration-300">Send 
Message</button>
            </form>
        </div>
    </section>

    <!-- Footer -->
    <footer class="py-10 bg-gray-900 text-center text-gray-400">
        <p>&copy; 2024 Ubaydillah.</p>
        <div class="mt-4 space-x-6">
            <a href="https://www.linkedin.com/in/ubaydillah-devnet-839171316?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app" class="hover:text-white">LinkedIn</a>
            <a href="https://github.com/Ubaydex" class="hover:text-white">GitHub</a>
            <a href="#" class="hover:text-white">Instagram</a>
        </div>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const hamburgerButton = document.getElementById('hamburger-button');
            const mobileMenu = document.getElementById('mobile-menu');
            
            hamburgerButton.addEventListener('click', () => {
                mobileMenu.classList.toggle('open');
            });

            // Smooth scroll for anchor links
            document.querySelectorAll('a[href^="#"]').forEach(anchor => {
                anchor.addEventListener('click', function(e) {
                    e.preventDefault();
                    document.querySelector(this.getAttribute('href')).scrollIntoView({
                        behavior: 'smooth'
                    });
                    // Close menu when an item is clicked (optional)
                    if (mobileMenu.classList.contains('open')) {
                        mobileMenu.classList.remove('open');
                    }
                });
            });
        });
    </script>

</body>
</html>
