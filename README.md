<html lang="id">
<head>
    <meta charset="UTF-8">
    <link rel="shortcut icon" type="image/x-icon" href="file:///D:/WEB%20LATIHAN/codev.jpg">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CodeV</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        primary: '#1e293b',
                        secondary: '#3b82f6',
                        dark: '#0f172a',
                        light: '#f8fafc'
                    },
                    fontFamily: {
                        poppins: ['Poppins', 'sans-serif']
                    }
                }
            }
        }
    </script>
    <style>
        .gradient-bg {
            background: linear-gradient(135deg, #0f172a 0%, #1e293b 100%);
        }
        .skill-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(59, 130, 246, 0.3);
        }
        .project-card:hover {
            transform: scale(1.02);
        }
        .animate-float {
            animation: float 6s ease-in-out infinite;
        }
        @keyframes float {
            0%, 100% { transform: translateY(0px) }
            50% { transform: translateY(-20px) }
        }
        .social-icon {
            transition: all 0.3s ease;
        }
        .social-icon:hover {
            transform: translateY(-3px);
            filter: drop-shadow(0px 5px 10px rgba(59, 130, 246, 0.4));
        }
    </style>
</head>
<body class="font-poppins bg-gradient-to-br from-dark to-primary text-light min-h-screen">
    <!-- Header & Navigation -->
    <header class="py-6 px-4 md:px-12 fixed w-full z-50 backdrop-blur-sm">
        <div class="container mx-auto flex justify-between items-center">
            <div class="text-2xl font-bold text-secondary">CodeV</div>
            <nav class="hidden md:block">
                <ul class="flex space-x-10">
                    <li><a href="#home" class="hover:text-secondary transition">Home</a></li>
                    <li><a href="#about" class="hover:text-secondary transition">About</a></li>
                    <li><a href="#skills" class="hover:text-secondary transition">Skills</a></li>
                    <li><a href="#projects" class="hover:text-secondary transition">Projects</a></li>
                    <li><a href="#contact" class="hover:text-secondary transition">Contact</a></li>
                </ul>
            </nav>
            <div class="md:hidden">
                <button id="menu-toggle" class="text-white">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
                    </svg>
                </button>
            </div>
        </div>
        <!-- Mobile Menu -->
        <div id="mobile-menu" class="hidden md:hidden bg-dark/95 py-4 px-8 rounded-lg mt-2 absolute w-5/6 left-2/4 -translate-x-1/2">
            <ul class="space-y-3">
                <li><a href="#home" class="block hover:text-secondary transition">Home</a></li>
                <li><a href="#about" class="block hover:text-secondary transition">About</a></li>
                <li><a href="#skills" class="block hover:text-secondary transition">Skills</a></li>
                <li><a href="#projects" class="block hover:text-secondary transition">Projects</a></li>
                <li><a href="#contact" class="block hover:text-secondary transition">Contact</a></li>
            </ul>
        </div>
    </header>

    <!-- Hero Section -->
    <section id="home" class="min-h-screen flex items-center pt-20 pb-28 px-4 md:px-12">
        <div class="container mx-auto grid md:grid-cols-2 gap-12 items-center">
            <div>
                <h1 class="text-4xl md:text-6xl font-bold mb-4">Hi, I am <span class="text-secondary">Fatkhur Rokhman Abdillah</span></h1>
                <h2 class="text-xl md:text-3xl font-semibold text-gray-300 mb-6">Web Developer & UI/UX Designer</h2>
                <p class="text-lg mb-8 max-w-xl">I create beautiful and functional digital solutions with a focus on user experience and cutting-edge technology.</p>
                <div class="flex flex-wrap gap-4">
                    <a href="#projects" class="bg-secondary hover:bg-blue-500 py-3 px-8 rounded-lg font-medium transition shadow-xl shadow-blue-500/20">The Project</a>
                    <a href="#contact" class="border border-secondary hover:bg-secondary/20 py-3 px-8 rounded-lg font-medium transition">Contact me</a>
                </div>
            </div>
            <div class="flex justify-center">
                <div class="relative">
                    <div class="absolute w-80 h-80 bg-secondary/20 rounded-full -top-8 -left-8 -z-10 animate-pulse"></div>
                    <div class="absolute w-80 h-80 bg-secondary/10 rounded-full -bottom-8 -right-8 -z-10 animate-pulse"></div>
                    <img 
                        src="img/IMG_9307.JPG"
                        alt="Professional portrait of a web developer working in a modern office with laptop" 
                        class="relative w-64 h-80 md:w-80 md:h-96 object-cover rounded-xl shadow-xl animate-float"
                    >
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-20 px-4 md:px-12">
        <div class="container mx-auto">
            <h2 class="text-4xl font-bold mb-4 text-center">About Me</h2>
            <div class="w-24 h-1 bg-secondary mx-auto mb-12 rounded-full"></div>
            
            <div class="grid md:grid-cols-2 gap-12 items-center">
                <div class="space-y-6 text-lg">
                    <p>I am a talented professional in web development and graphic design with 3 years of experience.
                    <p>My expertise includes both frontend and backend development with a focus on innovation and quality.
                    <p>With experience in various large projects, I am capable of designing solutions that are technically robust while also visually stunning. In my work, I always prioritize code quality and user experience.Outside of work, I enjoy exploring the latest technology trends and contributing to open source projects.
                    <div class="pt-4">
                        <a href="#" class="inline-flex items-center text-secondary group">
                            Unduh CV
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 ml-2 group-hover:translate-x-1 transition" viewBox="0 0 20 20" fill="currentColor">
                                <path fill-rule="evenodd" d="M10.293 5.293a1 1 0 011.414 0l4 4a1 1 0 010 1.414l-4 4a1 1 0 01-1.414-1.414L12.586 11H5a1 1 0 110-2h7.586l-2.293-2.293a1 1 0 010-1.414z" clip-rule="evenodd" />
                            </svg>
                        </a>
                    </div>
                </div>
                <div>
                    <div class="bg-white/5 p-8 rounded-xl grid grid-cols-2 gap-8">
                        <div class="text-center">
                            <div class="text-5xl font-bold text-secondary mb-2">3+</div>
                            <div>years of experience</div>
                        </div>
                        <div class="text-center">
                            <div class="text-5xl font-bold text-secondary mb-2">20+</div>
                            <div>Project Completed</div>
                        </div>
                        <div class="text-center">
                            <div class="text-5xl font-bold text-secondary mb-2">15+</div>
                            <div>Satisfied Client</div>
                        </div>
                        <div class="text-center">
                            <div class="text-5xl font-bold text-secondary mb-2">3+</div>
                            <div>Awards</div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="py-20 px-4 md:px-12">
        <div class="container mx-auto">
            <h2 class="text-4xl font-bold mb-4 text-center">Skill</h2>
            <div class="w-24 h-1 bg-secondary mx-auto mb-16 rounded-full"></div>
            
            <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-5 gap-8">
                <!-- Skill 1 -->
                <div class="skill-card bg-white/5 rounded-xl p-6 flex flex-col items-center transition duration-300 border border-white/10">
                    <div class="bg-white/10 p-4 rounded-full mb-4">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/4f5b05ba-cac0-41c7-95fa-b0ee7ff297b6.png" alt="HTML5 logo with stylized 3D effect" class="w-16 h-16 object-contain">
                    </div>
                    <h3 class="text-xl font-semibold mb-2">HTML</h3>
                    <div class="w-full bg-gray-700 rounded-full h-2.5">
                        <div class="bg-secondary h-2.5 rounded-full" style="width: 95%"></div>
                    </div>
                </div>
                
                <!-- Skill 2 -->
                <div class="skill-card bg-white/5 rounded-xl p-6 flex flex-col items-center transition duration-300 border border-white/10">
                    <div class="bg-white/10 p-4 rounded-full mb-4">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/6d389beb-0193-45de-9c76-c4f0ff906994.png" alt="CSS3 logo with dynamic gradient effect" class="w-16 h-16 object-contain">
                    </div>
                    <h3 class="text-xl font-semibold mb-2">CSS</h3>
                    <div class="w-full bg-gray-700 rounded-full h-2.5">
                        <div class="bg-secondary h-2.5 rounded-full" style="width: 90%"></div>
                    </div>
                </div>
                
                <!-- Skill 3 -->
                <div class="skill-card bg-white/5 rounded-xl p-6 flex flex-col items-center transition duration-300 border border-white/10">
                    <div class="bg-white/10 p-4 rounded-full mb-4">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/75cce08b-b436-4518-a1f2-77589e7410aa.png" alt="JavaScript logo with code particles animation" class="w-16 h-16 object-contain">
                    </div>
                    <h3 class="text-xl font-semibold mb-2">JavaScript</h3>
                    <div class="w-full bg-gray-700 rounded-full h-2.5">
                        <div class="bg-secondary h-2.5 rounded-full" style="width: 85%"></div>
                    </div>
                </div>
                
                <!-- Skill 4 -->
                <div class="skill-card bg-white/5 rounded-xl p-6 flex flex-col items-center transition duration-300 border border-white/10">
                    <div class="bg-white/10 p-4 rounded-full mb-4">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/4c26e9b6-8797-488d-b8f3-05ec15132ca2.png" alt="React logo with atom particle effect" class="w-16 h-16 object-contain">
                    </div>
                    <h3 class="text-xl font-semibold mb-2">React</h3>
                    <div class="w-full bg-gray-700 rounded-full h-2.5">
                        <div class="bg-secondary h-2.5 rounded-full" style="width: 88%"></div>
                    </div>
                </div>
                
                <!-- Skill 5 -->
                <div class="skill-card bg-white/5 rounded-xl p-6 flex flex-col items-center transition duration-300 border border-white/10">
                    <div class="bg-white/10 p-4 rounded-full mb-4">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/f1e86818-67d2-408d-a3d1-5ecead22c429.png" alt="Node.js logo with interconnected network nodes" class="w-16 h-16 object-contain">
                    </div>
                    <h3 class="text-xl font-semibold mb-2">Node.js</h3>
                    <div class="w-full bg-gray-700 rounded-full h-2.5">
                        <div class="bg-secondary h-2.5 rounded-full" style="width: 82%"></div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="py-20 px-4 md:px-12 bg-dark">
        <div class="container mx-auto">
            <h2 class="text-4xl font-bold mb-4 text-center">New Project</h2>
            <div class="w-24 h-1 bg-secondary mx-auto mb-16 rounded-full"></div>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Project 1 -->
                <div class="project-card bg-white/5 rounded-xl overflow-hidden transition duration-300 hover:shadow-lg hover:shadow-secondary/20">
                    <div class="h-56 overflow-hidden">
                        <img 
                            src="img/ss e-comarch.jpeg" 
                            alt="Dashboard interface of e-commerce platform showing analytics charts"
                            class="w-full h-full object-cover"
                        >
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-2">E-Commerce Dashboard</h3>
                        <p class="text-gray-400 mb-4">Complete dashboard to monitor sales, visitor statistics, and product management.</p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="bg-secondary/10 text-secondary px-3 py-1 rounded-full text-sm">React</span>
                            <span class="bg-secondary/10 text-secondary px-3 py-1 rounded-full text-sm">Node.js</span>
                            <span class="bg-secondary/10 text-secondary px-3 py-1 rounded-full text-sm">MongoDB</span>
                        </div>
                        <a href="file:///D:/CodeV/redirect/e-commerch.html" class="text-secondary hover:text-blue-400 transition flex items-center">
                            Detail Proyek
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 ml-1" viewBox="0 0 20 20" fill="currentColor">
                                <path fill-rule="evenodd" d="M10.293 5.293a1 1 0 011.414 0l4 4a1 1 0 010 1.414l-4 4a1 1 0 01-1.414-1.414L12.586 11H5a1 1 0 110-2h7.586l-2.293-2.293a1 1 0 010-1.414z" clip-rule="evenodd" />
                            </svg>
                        </a>
                    </div>
                </div>
                
                <!-- Project 2 -->
                <div class="project-card bg-white/5 rounded-xl overflow-hidden transition duration-300 hover:shadow-lg hover:shadow-secondary/20">
                    <div class="h-56 overflow-hidden">
                        <img 
                            src="img/ss fitnes.jpeg" 
                            alt="Mobile fitness tracking application showing workout statistics"
                            class="w-full h-full object-cover"
                        >
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-2">Aplikasi Fitness</h3>
                        <p class="text-gray-400 mb-4">Mobile solutions to track fitness activities with personalized workout recommendations.</p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="bg-secondary/10 text-secondary px-3 py-1 rounded-full text-sm">React Native</span>
                            <span class="bg-secondary/10 text-secondary px-3 py-1 rounded-full text-sm">Firebase</span>
                            <span class="bg-secondary/10 text-secondary px-3 py-1 rounded-full text-sm">Redux</span>
                        </div>
                        <a href="file:///D:/CodeV/redirect/Fitnes.html" class="text-secondary hover:text-blue-400 transition flex items-center">
                            Detail Proyek
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 ml-1" viewBox="0 0 20 20" fill="currentColor">
                                <path fill-rule="evenodd" d="M10.293 5.293a1 1 0 011.414 0l4 4a1 1 0 010 1.414l-4 4a1 1 0 01-1.414-1.414L12.586 11H5a1 1 0 110-2h7.586l-2.293-2.293a1 1 0 010-1.414z" clip-rule="evenodd" />
                            </svg>
                        </a>
                    </div>
                </div>
                
                <!-- Project 3 -->
                <div class="project-card bg-white/5 rounded-xl overflow-hidden transition duration-300 hover:shadow-lg hover:shadow-secondary/20">
                    <div class="h-56 overflow-hidden">
                        <img 
                            src="img/ss menejemen keuangan.jpeg" 
                            alt="Financial management website with portfolio tracking dashboard"
                            class="w-full h-full object-cover"
                        >
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-2">Manajemen Keuangan</h3>
                        <p class="text-gray-400 mb-4">Homepage and service page for a technology company with modern animations.</p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="bg-secondary/10 text-secondary px-3 py-1 rounded-full text-sm">Vue.js</span>
                            <span class="bg-secondary/10 text-secondary px-3 py-1 rounded-full text-sm">Express</span>
                            <span class="bg-secondary/10 text-secondary px-3 py-1 rounded-full text-sm">PostgreSQL</span>
                        </div>
                        <a href="file:///D:/CodeV/redirect/Menejemen%20keuangan.html" class="text-secondary hover:text-blue-400 transition flex items-center">
                            Detail Proyek
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 ml-1" viewBox="0 0 20 20" fill="currentColor">
                                <path fill-rule="evenodd" d="M10.293 5.293a1 1 0 011.414 0l4 4a1 1 0 010 1.414l-4 4a1 1 0 01-1.414-1.414L12.586 11H5a1 1 0 110-2h7.586l-2.293-2.293a1 1 0 010-1.414z" clip-rule="evenodd" />
                            </svg>
                        </a>
                    </div>
                </div>
            </div>
            
            <div class="text-center mt-12">
                <a href="file:///D:/CodeV/redirect/CodeV%20Project.html" class="inline-block border border-secondary text-secondary py-2 px-6 rounded-lg hover:bg-secondary hover:text-white transition duration-300">
                    View All Project
                </a>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-20 px-4 md:px-12">
        <div class="container mx-auto">
            <h2 class="text-4xl font-bold mb-4 text-center">Contect me</h2>
            <div class="w-24 h-1 bg-secondary mx-auto mb-16 rounded-full"></div>
            
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-12">
                <div>
                    <p class="text-xl mb-8 max-w-2xl text-center lg:text-left">
                        Interested in working together? Please contact me through this form or through the direct contacts below.
                    </p>
                    
                    <div class="bg-white/5 rounded-xl p-8 space-y-6">
                        <div class="flex items-center">
                            <div class="bg-secondary/10 p-3 rounded-full mr-4">
                                <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-secondary" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z" />
                                </svg>
                            </div>
                            <div>
                                <h3 class="font-semibold">Number Phone</h3>
                                <p>+62 895-4177-79066</p>
                            </div>
                        </div>
                        
                        <div class="flex items-center">
                            <div class="bg-secondary/10 p-3 rounded-full mr-4">
                                <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-secondary" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
                                </svg>
                            </div>
                            <div>
                                <h3 class="font-semibold">Email</h3>
                                <p>codevisual001@gmail.com</p>
                            </div>
                        </div>
                        
                        <div class="flex items-center">
                            <div class="bg-secondary/10 p-3 rounded-full mr-4">
                                <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-secondary" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z" />
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 11a3 3 0 11-6 0 3 3 0 016 0z" />
                                </svg>
                            </div>
                            <div>
                                <h3 class="font-semibold">location</h3>
                                <p>Purbalingga, Indonesia</p>
                            </div>
                        </div>
                        
                        <div class="pt-4">
                            <h3 class="font-semibold mb-4">Media Sosial</h3>
                            <div class="flex space-x-4">
                                <a href="https://web.facebook.com/profile.php?id=100066138840680" class="social-icon block bg-white/10 rounded-full w-10 h-10 flex items-center justify-center hover:bg-secondary">
                                    <svg xmlns="http://www.w3.org/2000/svg" height="20" width="12.5" viewBox="0 0 320 512"><!--!Font Awesome Free v7.0.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free Copyright 2025 Fonticons, Inc.--><path fill="#ffffff" d="M80 299.3l0 212.7 116 0 0-212.7 86.5 0 18-97.8-104.5 0 0-34.6c0-51.7 20.3-71.5 72.7-71.5 16.3 0 29.4 .4 37 1.2l0-88.7C291.4 4 256.4 0 236.2 0 129.3 0 80 50.5 80 159.4l0 42.1-66 0 0 97.8 66 0z"/></svg>
                                    <path d="M22.675 0h-21.35c-.732 0-1.325.593-1.325 1.325v21.351c0 .731.593 1.324 1.325 1.324h11.495v-9.294h-3.128v-3.622h3.128v-2.671c0-3.1 1.893-4.788 4.659-4.788 1.325 0 2.463.099 2.795.143v3.24l-1.918.001c-1.504 0-1.795.715-1.795 1.763v2.313h3.587l-.467 3.622h-3.12v9.293h6.116c.73 0 1.323-.593 1.323-1.325v-21.35c0-.732-.593-1.325-1.325-1.325z"/>
                                    </svg>
                                
                                <a href="https://www.instagram.com/urawa.higuchi/" class="social-icon block bg-white/10 rounded-full w-10 h-10 flex items-center justify-center hover:bg-secondary">
                                    <svg xmlns="http://www.w3.org/2000/svg" height="24" width="21" viewBox="0 0 448 512"><!--!Font Awesome Free v7.0.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free Copyright 2025 Fonticons, Inc.--><path fill="#ffffff" d="M224.3 141a115 115 0 1 0 -.6 230 115 115 0 1 0 .6-230zm-.6 40.4a74.6 74.6 0 1 1 .6 149.2 74.6 74.6 0 1 1 -.6-149.2zm93.4-45.1a26.8 26.8 0 1 1 53.6 0 26.8 26.8 0 1 1 -53.6 0zm129.7 27.2c-1.7-35.9-9.9-67.7-36.2-93.9-26.2-26.2-58-34.4-93.9-36.2-37-2.1-147.9-2.1-184.9 0-35.8 1.7-67.6 9.9-93.9 36.1s-34.4 58-36.2 93.9c-2.1 37-2.1 147.9 0 184.9 1.7 35.9 9.9 67.7 36.2 93.9s58 34.4 93.9 36.2c37 2.1 147.9 2.1 184.9 0 35.9-1.7 67.7-9.9 93.9-36.2 26.2-26.2 34.4-58 36.2-93.9 2.1-37 2.1-147.8 0-184.8zM399 388c-7.8 19.6-22.9 34.7-42.6 42.6-29.5 11.7-99.5 9-132.1 9s-102.7 2.6-132.1-9c-19.6-7.8-34.7-22.9-42.6-42.6-11.7-29.5-9-99.5-9-132.1s-2.6-102.7 9-132.1c7.8-19.6 22.9-34.7 42.6-42.6 29.5-11.7 99.5-9 132.1-9s102.7-2.6 132.1 9c19.6 7.8 34.7 22.9 42.6 42.6 11.7 29.5 9 99.5 9 132.1s2.7 102.7-9 132.1z"/></svg>
                                    <path d="M12 0c-6.627 0-12 5.373-12 12s5.373 12 12 12 12-5.373 12-12-5.373-12-12-12zm6.066 9.645c.183 4.04-2.83 8.544-8.164 8.544-1.622 0-3.131-.46-4.402-1.291 1.524.18 3.045-.244 4.252-1.189-1.256-.023-2.317-.854-2.684-1.995.451.086.895.061 1.298-.049-1.381-.277-2.335-1.522-2.304-2.853.388.215.83.344 1.301.359-1.279-.855-1.641-2.544-.889-3
