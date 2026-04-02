<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Saleha Haider Turk - AI & Automation Specialist | Portfolio">
    <title>Saleha Haider Turk | AI & Automation Specialist</title>
    
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Font Awesome -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.6.0/css/all.min.css">
    
    <!-- Google Fonts: Poppins (Headings) + Inter (Body) -->
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@500;600;700&amp;family=Inter:wght@400;500&amp;display=swap" rel="stylesheet">
    
    <style>
        :root {
            --primary: #0B192E;
            --accent: #14B8A6;
            --light-blue: #3B82F6;
        }
        
        * {
            font-family: 'Inter', system-ui, sans-serif;
        }
        
        h1, h2, h3, h4 {
            font-family: 'Poppins', sans-serif;
        }
        
        body {
            background-color: #0B192E;
            color: #f1f5f9;
        }
        
        /* Navbar */
        nav {
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
        }
        
        nav.scrolled {
            background-color: #14B8A6 !important;
            box-shadow: 0 10px 15px -3px rgb(20 184 166);
        }
        
        /* Hero Neural Network Canvas */
        #neural-canvas {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: 1;
            opacity: 0.15;
        }
        
        /* 3D Tech Cards */
        .tech-card {
            transition: all 0.4s cubic-bezier(0.34, 1.56, 0.64, 1);
        }
        
        .tech-card:hover {
            transform: perspective(1200px) rotateX(8deg) rotateY(12deg) scale(1.05);
            box-shadow: 0 25px 50px -12px rgb(20 184 166);
        }
        
        /* Project Card Hover Reveal */
        .project-card {
            transition: all 0.3s ease;
        }
        
        .project-card:hover .project-overlay {
            opacity: 1;
            transform: translateY(0);
        }
        
        /* Glassmorphism Contact Form */
        .glass {
            background: rgba(255, 255, 255, 0.08);
            backdrop-filter: blur(16px);
            border: 1px solid rgba(20, 184, 166, 0.2);
        }
        
        /* Smooth scroll */
        html {
            scroll-behavior: smooth;
        }
    </style>
</head>
<body class="min-h-screen">

    <!-- NAVIGATION & HEADER -->
    <nav id="navbar" class="sticky top-0 z-50 bg-transparent py-5 px-8 flex items-center justify-between">
        <!-- Logo -->
        <div class="flex items-center gap-3">
            <div class="w-9 h-9 bg-[#14B8A6] rounded-2xl flex items-center justify-center text-[#0B192E] font-bold text-2xl shadow-inner">
                S
            </div>
            <div>
                <h1 class="text-2xl font-semibold tracking-tight text-white">Saleha Haider Turk</h1>
                <p class="text-xs tracking-[2px] text-[#14B8A6] -mt-1">AI &amp; AUTOMATION</p>
            </div>
        </div>

        <!-- Menu -->
        <div class="hidden md:flex items-center gap-x-8 text-sm font-medium">
            <a href="#hero" class="hover:text-[#14B8A6] transition-colors">Home</a>
            <a href="#about" class="hover:text-[#14B8A6] transition-colors">About</a>
            <a href="#expertise" class="hover:text-[#14B8A6] transition-colors">Expertise</a>
            <a href="#projects" class="hover:text-[#14B8A6] transition-colors">Projects</a>
            <a href="#insights" class="hover:text-[#14B8A6] transition-colors">Insights</a>
            <a href="#contact" class="hover:text-[#14B8A6] transition-colors">Contact</a>
        </div>

        <!-- Mobile Menu Button -->
        <button id="mobile-menu-btn" class="md:hidden text-2xl text-white">
            <i class="fa-solid fa-bars"></i>
        </button>

        <!-- Mobile Menu -->
        <div id="mobile-menu" class="hidden md:hidden fixed top-20 left-0 right-0 bg-[#0B192E] shadow-2xl py-6 px-8 flex flex-col gap-4 text-lg z-50">
            <a href="#hero" class="hover:text-[#14B8A6]">Home</a>
            <a href="#about" class="hover:text-[#14B8A6]">About</a>
            <a href="#expertise" class="hover:text-[#14B8A6]">Expertise</a>
            <a href="#projects" class="hover:text-[#14B8A6]">Projects</a>
            <a href="#insights" class="hover:text-[#14B8A6]">Insights</a>
            <a href="#contact" class="hover:text-[#14B8A6]">Contact</a>
        </div>
    </nav>

    <!-- HERO SECTION -->
    <section id="hero" class="relative min-h-screen flex items-center overflow-hidden">
        <!-- Neural Network Background -->
        <canvas id="neural-canvas"></canvas>
        
        <div class="relative z-10 max-w-7xl mx-auto px-8 grid md:grid-cols-2 gap-12 items-center">
            
            <!-- Left Content -->
            <div class="space-y-8">
                <div class="inline-flex items-center gap-2 px-4 py-2 bg-white/10 rounded-3xl text-sm backdrop-blur-md border border-white/10">
                    <div class="w-2 h-2 bg-[#14B8A6] rounded-full animate-pulse"></div>
                    AI &amp; Automation Specialist
                </div>
                
                <h1 class="text-6xl md:text-7xl font-bold leading-none tracking-tighter">
                    Building the<br>future with<br><span class="text-[#14B8A6]">intelligence</span>
                </h1>
                
                <p class="text-xl text-slate-300 max-w-md">
                    AI student &amp; technical intern turning complex problems into intelligent automated solutions.
                </p>
                
                <div class="flex items-center gap-4">
                    <a href="#contact" 
                       class="px-8 py-4 bg-[#14B8A6] hover:bg-[#0F9A8A] text-[#0B192E] font-semibold rounded-2xl flex items-center gap-3 transition-all active:scale-95">
                        Let's Connect
                        <i class="fa-solid fa-arrow-right"></i>
                    </a>
                    
                    <a href="#projects" 
                       class="px-8 py-4 border border-white/30 hover:border-[#14B8A6] rounded-2xl font-medium flex items-center gap-3 transition-all">
                        View Projects
                    </a>
                </div>
                
                <div class="flex items-center gap-8 text-sm">
                    <div>
                        <span class="block text-[#14B8A6] text-3xl font-semibold">12+</span>
                        <span class="text-slate-400">Projects Delivered</span>
                    </div>
                    <div>
                        <span class="block text-[#14B8A6] text-3xl font-semibold">4</span>
                        <span class="text-slate-400">Expertise Areas</span>
                    </div>
                    <div class="flex -space-x-4">
                        <i class="fa-brands fa-linkedin text-3xl text-[#14B8A6]"></i>
                        <i class="fa-brands fa-github text-3xl text-[#3B82F6]"></i>
                    </div>
                </div>
            </div>
            
            <!-- Right Visual -->
            <div class="relative flex justify-center">
                <div class="w-80 h-80 md:w-96 md:h-96 bg-gradient-to-br from-[#1E3A8A] to-[#14B8A6] rounded-3xl rotate-6 shadow-2xl flex items-center justify-center relative overflow-hidden">
                    <!-- Tech Illustration -->
                    <div class="text-8xl text-white/90 z-10">
                        <i class="fa-solid fa-brain"></i>
                    </div>
                    <!-- Floating icons -->
                    <div class="absolute -top-6 -left-6 text-4xl bg-white/10 backdrop-blur-xl p-4 rounded-2xl rotate-12 shadow-inner">
                        <i class="fa-solid fa-robot"></i>
                    </div>
                    <div class="absolute -bottom-6 -right-6 text-4xl bg-white/10 backdrop-blur-xl p-4 rounded-2xl -rotate-12 shadow-inner">
                        <i class="fa-solid fa-diagram-project"></i>
                    </div>
                    <div class="absolute top-1/2 -left-10 text-3xl bg-white/10 backdrop-blur-xl p-3 rounded-2xl">
                        <i class="fa-solid fa-chart-line"></i>
                    </div>
                    
                    <!-- Personal photo placeholder -->
                    <div class="absolute bottom-8 right-8 w-28 h-28 bg-white/90 rounded-2xl shadow-2xl overflow-hidden border-4 border-[#14B8A6]">
                        <div class="w-full h-full bg-[#0B192E] flex items-center justify-center text-[#14B8A6] text-xs font-medium text-center leading-tight">
                            YOUR PHOTO<br>HERE
                        </div>
                    </div>
                </div>
            </div>
        </div>
        
        <!-- Scroll indicator -->
        <div class="absolute bottom-12 left-1/2 hidden md:flex flex-col items-center gap-2 text-xs tracking-widest">
            <span>SCROLL TO EXPLORE</span>
            <i class="fa-solid fa-chevron-down animate-bounce text-[#14B8A6]"></i>
        </div>
    </section>

    <!-- ABOUT ME -->
    <section id="about" class="py-24 px-8 max-w-7xl mx-auto">
        <div class="grid md:grid-cols-2 gap-16 items-center">
            <!-- Left Image -->
            <div class="relative">
                <div class="bg-gradient-to-br from-[#1E3A8A] to-[#14B8A6] rounded-3xl p-3 shadow-2xl">
                    <div class="bg-[#0B192E] rounded-3xl overflow-hidden aspect-square flex items-center justify-center">
                        <div class="text-center">
                            <div class="w-40 h-40 mx-auto bg-white/10 backdrop-blur-md rounded-2xl flex items-center justify-center mb-6">
                                <i class="fa-solid fa-user-tie text-8xl text-[#14B8A6]"></i>
                            </div>
                            <p class="text-slate-400 text-sm">Saleha Haider Turk</p>
                            <p class="font-medium">AI Student &amp; Technical Intern</p>
                            <!-- Replace the div above with your actual photo -->
                            <p class="text-[10px] text-slate-500 mt-8">Replace this placeholder with your professional photo</p>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- Right Bio -->
            <div class="space-y-8">
                <div class="flex items-center gap-3">
                    <div class="h-px w-12 bg-[#14B8A6]"></div>
                    <span class="uppercase tracking-[2px] text-[#14B8A6] text-sm font-medium">My Story</span>
                </div>
                
                <h2 class="text-5xl font-semibold leading-tight">Turning curiosity into intelligent systems</h2>
                
                <div class="prose prose-invert text-slate-300 text-lg">
                    <p>As an AI &amp; Automation specialist, I combine deep technical knowledge with creative problem-solving. Currently pursuing advanced studies in Artificial Intelligence, I bring real-world experience from technical internships where I designed and deployed intelligent workflows.</p>
                    <p>My passion lies at the intersection of AI, automation, and human-centered design — creating solutions that are not only powerful but also intuitive and scalable.</p>
                </div>
                
                <div class="grid grid-cols-3 gap-6 text-center">
                    <div class="bg-white/5 rounded-3xl p-6">
                        <i class="fa-solid fa-graduation-cap text-3xl text-[#14B8A6] mb-3"></i>
                        <p class="font-semibold">AI Student</p>
                    </div>
                    <div class="bg-white/5 rounded-3xl p-6">
                        <i class="fa-solid fa-laptop-code text-3xl text-[#14B8A6] mb-3"></i>
                        <p class="font-semibold">Technical Intern</p>
                    </div>
                    <div class="bg-white/5 rounded-3xl p-6">
                        <i class="fa-solid fa-lightbulb text-3xl text-[#14B8A6] mb-3"></i>
                        <p class="font-semibold">Innovator</p>
                    </div>
                </div>
                
                <a href="#contact" class="inline-flex items-center gap-3 text-[#14B8A6] font-medium group">
                    Get to know me better 
                    <span class="transition-transform group-hover:translate-x-2">→</span>
                </a>
            </div>
        </div>
    </section>

    <!-- MY TECH STACK (EXPERTISE) -->
    <section id="expertise" class="py-24 bg-[#0B192E] px-8 max-w-7xl mx-auto">
        <div class="text-center mb-16">
            <span class="px-5 py-2 bg-[#14B8A6]/10 text-[#14B8A6] text-sm font-medium rounded-3xl">Expertise</span>
            <h2 class="text-5xl font-semibold mt-4">My Tech Stack</h2>
            <p class="text-slate-400 mt-3 max-w-md mx-auto">Tools and technologies I master to build intelligent, automated solutions</p>
        </div>
        
        <div class="grid md:grid-cols-4 gap-8">
            <!-- Card 1 -->
            <div class="tech-card bg-white/5 rounded-3xl p-8 border border-white/10 text-center">
                <div class="w-16 h-16 mx-auto mb-6 bg-[#14B8A6]/10 text-[#14B8A6] rounded-2xl flex items-center justify-center text-4xl">
                    <i class="fa-solid fa-brain"></i>
                </div>
                <h3 class="text-2xl font-semibold mb-3">Artificial Intelligence</h3>
                <p class="text-slate-400">Neural Networks • Machine Learning • Generative AI • Computer Vision</p>
                <div class="mt-8 flex flex-wrap justify-center gap-2">
                    <span class="text-xs px-4 py-1 bg-white/10 rounded-full">PyTorch</span>
                    <span class="text-xs px-4 py-1 bg-white/10 rounded-full">TensorFlow</span>
                    <span class="text-xs px-4 py-1 bg-white/10 rounded-full">LLMs</span>
                </div>
            </div>
            
            <!-- Card 2 -->
            <div class="tech-card bg-white/5 rounded-3xl p-8 border border-white/10 text-center">
                <div class="w-16 h-16 mx-auto mb-6 bg-[#3B82F6]/10 text-[#3B82F6] rounded-2xl flex items-center justify-center text-4xl">
                    <i class="fa-solid fa-gears"></i>
                </div>
                <h3 class="text-2xl font-semibold mb-3">Workflow Automation</h3>
                <p class="text-slate-400">RPA • Python Scripting • Zapier • AI Agents • API Integration</p>
                <div class="mt-8 flex flex-wrap justify-center gap-2">
                    <span class="text-xs px-4 py-1 bg-white/10 rounded-full">Make.com</span>
                    <span class="text-xs px-4 py-1 bg-white/10 rounded-full">n8n</span>
                    <span class="text-xs px-4 py-1 bg-white/10 rounded-full">Selenium</span>
                </div>
            </div>
            
            <!-- Card 3 -->
            <div class="tech-card bg-white/5 rounded-3xl p-8 border border-white/10 text-center">
                <div class="w-16 h-16 mx-auto mb-6 bg-[#14B8A6]/10 text-[#14B8A6] rounded-2xl flex items-center justify-center text-4xl">
                    <i class="fa-solid fa-palette"></i>
                </div>
                <h3 class="text-2xl font-semibold mb-3">Graphic Design</h3>
                <p class="text-slate-400">UI/UX • Branding • Data Visualization • Motion Graphics</p>
                <div class="mt-8 flex flex-wrap justify-center gap-2">
                    <span class="text-xs px-4 py-1 bg-white/10 rounded-full">Figma</span>
                    <span class="text-xs px-4 py-1 bg-white/10 rounded-full">Adobe Suite</span>
                    <span class="text-xs px-4 py-1 bg-white/10 rounded-full">Canva Pro</span>
                </div>
            </div>
            
            <!-- Card 4 -->
            <div class="tech-card bg-white/5 rounded-3xl p-8 border border-white/10 text-center">
                <div class="w-16 h-16 mx-auto mb-6 bg-[#3B82F6]/10 text-[#3B82F6] rounded-2xl flex items-center justify-center text-4xl">
                    <i class="fa-solid fa-code"></i>
                </div>
                <h3 class="text-2xl font-semibold mb-3">Web Development</h3>
                <p class="text-slate-400">Next.js • Tailwind • React • FastAPI • Full-Stack Solutions</p>
                <div class="mt-8 flex flex-wrap justify-center gap-2">
                    <span class="text-xs px-4 py-1 bg-white/10 rounded-full">HTML/CSS/JS</span>
                    <span class="text-xs px-4 py-1 bg-white/10 rounded-full">Node.js</span>
                    <span class="text-xs px-4 py-1 bg-white/10 rounded-full">PostgreSQL</span>
                </div>
            </div>
        </div>
    </section>

    <!-- FEATURED PROJECTS -->
    <section id="projects" class="py-24 px-8 bg-[#0B192E] max-w-7xl mx-auto">
        <div class="flex justify-between items-end mb-12">
            <div>
                <span class="uppercase text-[#14B8A6] text-sm font-medium">Featured Work</span>
                <h2 class="text-5xl font-semibold">Recent Projects</h2>
            </div>
            <a href="#" class="text-sm flex items-center gap-2 hover:text-[#14B8A6]">
                View all projects <i class="fa-solid fa-arrow-right"></i>
            </a>
        </div>
        
        <div class="grid md:grid-cols-2 gap-8">
            
            <!-- Project 1: Neural Grid -->
            <div class="project-card group relative bg-white/5 rounded-3xl overflow-hidden border border-white/10">
                <div class="h-80 bg-gradient-to-br from-[#1E3A8A] to-[#0B192E] flex items-center justify-center relative">
                    <div class="text-[120px] text-white/20 group-hover:text-white/30 transition-all">
                        <i class="fa-solid fa-network-wired"></i>
                    </div>
                    <div class="absolute inset-0 flex items-center justify-center">
                        <span class="px-6 py-3 bg-black/60 text-white text-sm font-medium rounded-3xl backdrop-blur">NEURAL GRID</span>
                    </div>
                </div>
                <div class="p-8">
                    <h3 class="text-2xl font-semibold">Neural Grid</h3>
                    <p class="text-slate-400 mt-2">Interactive 3D visualization platform for exploring deep neural network architectures in real-time.</p>
                    <div class="project-overlay opacity-0 translate-y-6 group-hover:opacity-100 group-hover:translate-y-0 transition-all mt-6 pt-6 border-t border-white/10 flex justify-between text-sm">
                        <div class="flex gap-2">
                            <span class="px-4 py-1 bg-[#14B8A6]/20 text-[#14B8A6] rounded-3xl text-xs">PyTorch</span>
                            <span class="px-4 py-1 bg-[#14B8A6]/20 text-[#14B8A6] rounded-3xl text-xs">Three.js</span>
                        </div>
                        <a href="#" class="font-medium flex items-center">View Live Demo →</a>
                    </div>
                </div>
            </div>
            
            <!-- Project 2: RSS News Automation -->
            <div class="project-card group relative bg-white/5 rounded-3xl overflow-hidden border border-white/10">
                <div class="h-80 bg-gradient-to-br from-[#14B8A6] to-[#1E3A8A] flex items-center justify-center relative">
                    <div class="text-[120px] text-white/20 group-hover:text-white/30 transition-all">
                        <i class="fa-solid fa-rss"></i>
                    </div>
                    <div class="absolute inset-0 flex items-center justify-center">
                        <span class="px-6 py-3 bg-black/60 text-white text-sm font-medium rounded-3xl backdrop-blur">RSS AUTOMATION</span>
                    </div>
                </div>
                <div class="p-8">
                    <h3 class="text-2xl font-semibold">RSS News Automation</h3>
                    <p class="text-slate-400 mt-2">End-to-end AI-powered pipeline that scrapes, summarizes, and distributes personalized news feeds automatically.</p>
                    <div class="project-overlay opacity-0 translate-y-6 group-hover:opacity-100 group-hover:translate-y-0 transition-all mt-6 pt-6 border-t border-white/10 flex justify-between text-sm">
                        <div class="flex gap-2">
                            <span class="px-4 py-1 bg-[#14B8A6]/20 text-[#14B8A6] rounded-3xl text-xs">Python</span>
                            <span class="px-4 py-1 bg-[#14B8A6]/20 text-[#14B8A6] rounded-3xl text-xs">LangChain</span>
                            <span class="px-4 py-1 bg-[#14B8A6]/20 text-[#14B8A6] rounded-3xl text-xs">Telegram Bot</span>
                        </div>
                        <a href="#" class="font-medium flex items-center">View GitHub →</a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- RESEARCH & INSIGHTS (Blog Preview) -->
    <section id="insights" class="py-24 px-8 max-w-7xl mx-auto">
        <div class="text-center mb-12">
            <span class="px-5 py-2 bg-[#3B82F6]/10 text-[#3B82F6] text-sm font-medium rounded-3xl">Research &amp; Insights</span>
            <h2 class="text-5xl font-semibold mt-4">Latest Thoughts</h2>
        </div>
        
        <div class="grid md:grid-cols-2 gap-8">
            <!-- Blog Card 1 -->
            <div class="glass rounded-3xl p-8 flex gap-6 hover:border-[#14B8A6] transition-all">
                <div class="text-6xl text-[#14B8A6]"><i class="fa-solid fa-youtube"></i></div>
                <div class="flex-1">
                    <h3 class="text-2xl font-semibold">YouTube Blueprint 2026</h3>
                    <p class="text-slate-300 mt-3">Complete step-by-step framework to build fully automated YouTube channels using AI agents and no-code tools.</p>
                    <div class="mt-8 flex justify-between items-center text-sm">
                        <span class="text-slate-400">March 2026 • 8 min read</span>
                        <a href="#" class="text-[#14B8A6] flex items-center">Read full post <i class="fa-solid fa-arrow-right ml-2"></i></a>
                    </div>
                </div>
            </div>
            
            <!-- Blog Card 2 -->
            <div class="glass rounded-3xl p-8 flex gap-6 hover:border-[#14B8A6] transition-all">
                <div class="text-6xl text-[#3B82F6]"><i class="fa-solid fa-user-secret"></i></div>
                <div class="flex-1">
                    <h3 class="text-2xl font-semibold">Dark Psychology in AI Marketing</h3>
                    <p class="text-slate-300 mt-3">How behavioral science meets artificial intelligence to create persuasive, ethical automation strategies.</p>
                    <div class="mt-8 flex justify-between items-center text-sm">
                        <span class="text-slate-400">February 2026 • 12 min read</span>
                        <a href="#" class="text-[#14B8A6] flex items-center">Read full post <i class="fa-solid fa-arrow-right ml-2"></i></a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- CONTACT SECTION -->
    <section id="contact" class="py-24 px-8 max-w-7xl mx-auto">
        <div class="glass rounded-3xl p-12 md:p-16 max-w-2xl mx-auto">
            <div class="text-center mb-12">
                <h2 class="text-5xl font-semibold">Let's build something intelligent together</h2>
                <p class="text-slate-400 mt-4">Open to collaborations, internships, or just a friendly chat about AI.</p>
            </div>
            
            <form id="contact-form" class="space-y-8">
                <div class="grid md:grid-cols-2 gap-6">
                    <div>
                        <label class="block text-xs font-medium mb-2 text-slate-400">YOUR NAME</label>
                        <input type="text" id="name" required 
                               class="w-full bg-transparent border border-white/20 focus:border-[#14B8A6] rounded-2xl px-6 py-5 outline-none text-white placeholder:text-slate-400">
                    </div>
                    <div>
                        <label class="block text-xs font-medium mb-2 text-slate-400">EMAIL ADDRESS</label>
                        <input type="email" id="email" required 
                               class="w-full bg-transparent border border-white/20 focus:border-[#14B8A6] rounded-2xl px-6 py-5 outline-none text-white placeholder:text-slate-400">
                    </div>
                </div>
                
                <div>
                    <label class="block text-xs font-medium mb-2 text-slate-400">MESSAGE</label>
                    <textarea id="message" rows="6" required
                              class="w-full bg-transparent border border-white/20 focus:border-[#14B8A6] rounded-3xl px-6 py-5 outline-none text-white placeholder:text-slate-400"></textarea>
                </div>
                
                <button type="submit"
                        class="w-full py-6 bg-[#14B8A6] hover:bg-[#0F9A8A] text-[#0B192E] font-semibold text-lg rounded-3xl flex items-center justify-center gap-3 transition-all">
                    SEND MESSAGE
                    <i class="fa-solid fa-paper-plane"></i>
                </button>
            </form>
            
            <!-- Social Links -->
            <div class="flex justify-center gap-8 mt-12 text-3xl">
                <a href="https://linkedin.com/in/saleha-haider-turk" target="_blank" class="hover:text-[#14B8A6] transition-colors"><i class="fa-brands fa-linkedin"></i></a>
                <a href="https://github.com/saleha-haider-turk" target="_blank" class="hover:text-[#14B8A6] transition-colors"><i class="fa-brands fa-github"></i></a>
                <a href="#" target="_blank" class="hover:text-[#14B8A6] transition-colors"><i class="fa-solid fa-envelope"></i></a>
            </div>
        </div>
    </section>

    <!-- FOOTER -->
    <footer class="bg-[#0B192E] border-t border-white/10 py-12 px-8 text-center text-sm text-slate-400">
        <p>© 2026 Saleha Haider Turk. Built with intelligence and ❤️ in Wah Cantt, Pakistan.</p>
        <p class="text-xs mt-3">Designed as a premium, modern portfolio following your exact specifications</p>
    </footer>

    <script>
        // Tailwind script already loaded via CDN
        
        // Navbar scroll effect (transparent → Teal)
        const navbar = document.getElementById('navbar');
        window.addEventListener('scroll', () => {
            if (window.scrollY > 80) {
                navbar.classList.add('scrolled');
            } else {
                navbar.classList.remove('scrolled');
            }
        });
        
        // Mobile menu toggle
        const mobileBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');
        mobileBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
            if (mobileMenu.classList.contains('hidden')) {
                mobileBtn.innerHTML = `<i class="fa-solid fa-bars"></i>`;
            } else {
                mobileBtn.innerHTML = `<i class="fa-solid fa-xmark"></i>`;
            }
        });
        
        // Neural Network Canvas Animation
        function createNeuralCanvas() {
            const canvas = document.getElementById('neural-canvas');
            const ctx = canvas.getContext('2d');
            
            function resizeCanvas() {
                canvas.width = window.innerWidth;
                canvas.height = window.innerHeight;
            }
            window.addEventListener('resize', resizeCanvas);
            resizeCanvas();
            
            let particles = [];
            const particleCount = 120;
            
            class Particle {
                constructor() {
                    this.x = Math.random() * canvas.width;
                    this.y = Math.random() * canvas.height;
                    this.vx = (Math.random() - 0.5) * 1.2;
                    this.vy = (Math.random() - 0.5) * 1.2;
                    this.radius = Math.random() * 3 + 1;
                }
                update() {
                    this.x += this.vx;
                    this.y += this.vy;
                    
                    if (this.x < 0 || this.x > canvas.width) this.vx *= -1;
                    if (this.y < 0 || this.y > canvas.height) this.vy *= -1;
                }
            }
            
            for (let i = 0; i < particleCount; i++) {
                particles.push(new Particle());
            }
            
            function animate() {
                ctx.clearRect(0, 0, canvas.width, canvas.height);
                
                // Draw particles
                for (let i = 0; i < particles.length; i++) {
                    const p = particles[i];
                    p.update();
                    
                    ctx.fillStyle = '#14B8A6';
                    ctx.beginPath();
                    ctx.arc(p.x, p.y, p.radius, 0, Math.PI * 2);
                    ctx.fill();
                }
                
                // Draw connecting lines
                ctx.strokeStyle = '#3B82F6';
                ctx.lineWidth = 0.6;
                for (let i = 0; i < particles.length; i++) {
                    for (let j = i + 1; j < particles.length; j++) {
                        const dx = particles[i].x - particles[j].x;
                        const dy = particles[i].y - particles[j].y;
                        const distance = Math.sqrt(dx * dx + dy * dy);
                        
                        if (distance < 160) {
                            ctx.globalAlpha = 1 - (distance / 160);
                            ctx.beginPath();
                            ctx.moveTo(particles[i].x, particles[i].y);
                            ctx.lineTo(particles[j].x, particles[j].y);
                            ctx.stroke();
                        }
                    }
                }
                ctx.globalAlpha = 1;
                
                requestAnimationFrame(animate);
            }
            
            animate();
        }
        
        // Contact form submission (demo)
        const form = document.getElementById('contact-form');
        form.addEventListener('submit', function(e) {
            e.preventDefault();
            
            const btn = this.querySelector('button');
            const originalText = btn.innerHTML;
            
            btn.innerHTML = `SENDING <i class="fa-solid fa-spinner fa-spin"></i>`;
            btn.disabled = true;
            
            // Simulate API call
            setTimeout(() => {
                btn.innerHTML = `MESSAGE SENT <i class="fa-solid fa-check"></i>`;
                btn.classList.add('!bg-emerald-400');
                
                setTimeout(() => {
                    alert("✅ Thank you! Your message has been sent to Saleha Haider Turk.");
                    form.reset();
                    btn.innerHTML = originalText;
                    btn.classList.remove('!bg-emerald-400');
                    btn.disabled = false;
                }, 2000);
            }, 1800);
        });
        
        // Initialize everything
        window.onload = function() {
            createNeuralCanvas();
            console.log('%c✅ Premium Portfolio for Saleha Haider Turk ready!', 'color:#14B8A6; font-family:Poppins; font-size:13px');
        };
    </script>
</body>
</html>
