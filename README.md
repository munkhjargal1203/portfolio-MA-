# portfolio-MA-
A.Munkhjargal Portfolio
[index.html](https://github.com/user-attachments/files/26144128/index.html)
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Munkhjargal Amgalanbaatar - Portfolio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Syne:wght@400;600;700&family=DM+Mono:wght@300;400;500&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        'syne': ['Syne', 'sans-serif'],
                        'mono': ['DM Mono', 'monospace']
                    },
                    animation: {
                        'glow': 'glow 2s ease-in-out infinite alternate',
                        'float': 'float 6s ease-in-out infinite',
                        'slide-up': 'slideUp 0.6s ease-out',
                        'fade-in': 'fadeIn 0.8s ease-out'
                    }
                }
            }
        }
    </script>
    <style>
        @keyframes glow {
            from { box-shadow: 0 0 20px rgba(56, 189, 248, 0.3); }
            to { box-shadow: 0 0 30px rgba(56, 189, 248, 0.6), 0 0 40px rgba(56, 189, 248, 0.3); }
        }
        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
        }
        @keyframes slideUp {
            from { opacity: 0; transform: translateY(30px); }
            to { opacity: 1; transform: translateY(0); }
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        .custom-cursor { cursor: none; }
        .cursor { position: fixed; width: 20px; height: 20px; border: 2px solid #38bdf8; border-radius: 50%; pointer-events: none; z-index: 9999; transition: all 0.1s ease; }
        .cursor-dot { position: fixed; width: 4px; height: 4px; background: #38bdf8; border-radius: 50%; pointer-events: none; z-index: 10000; }
        .reveal { opacity: 0; transform: translateY(30px); transition: all 0.6s ease; }
        .reveal.active { opacity: 1; transform: translateY(0); }
        
        .dark { background: linear-gradient(135deg, #0f172a 0%, #1e293b 50%, #334155 100%); }
        .light { background: linear-gradient(135deg, #f8fafc 0%, #e2e8f0 50%, #cbd5e1 100%); }
    </style>
</head>
<body class="font-syne transition-all duration-500 min-h-screen custom-cursor" id="body">
    <!-- Custom Cursor -->
    <div class="cursor hidden lg:block"></div>
    <div class="cursor-dot hidden lg:block"></div>
    
    <!-- Theme Toggle -->
    <button id="themeToggle" class="fixed top-6 right-6 z-50 p-3 rounded-full bg-slate-800/20 dark:bg-slate-200/20 backdrop-blur-md border border-slate-700/30 dark:border-slate-300/30 hover:bg-slate-700/30 dark:hover:bg-slate-100/30 transition-all duration-300 group">
        <i class="fas fa-moon text-slate-200 dark:text-slate-800 group-hover:scale-110 transition-transform"></i>
    </button>

    <div class="min-h-screen text-slate-100 dark:text-slate-800">
        <!-- Hero Section -->
        <section class="min-h-screen flex items-center justify-center relative overflow-hidden">
            <div class="absolute inset-0 bg-gradient-to-br from-slate-900 via-indigo-950 to-slate-900 dark:from-slate-100 dark:via-blue-50 dark:to-slate-200"></div>
            
            <!-- Animated Background Elements -->
            <div class="absolute top-20 left-20 w-64 h-64 bg-sky-500/10 rounded-full blur-3xl animate-float"></div>
            <div class="absolute bottom-20 right-20 w-96 h-96 bg-indigo-500/10 rounded-full blur-3xl animate-float" style="animation-delay: -3s;"></div>
            
            <div class="relative z-10 text-center px-6 max-w-4xl mx-auto reveal">
                <div class="mb-8">
                    <h1 class="text-6xl md:text-8xl font-bold mb-6 bg-gradient-to-r from-sky-400 via-blue-400 to-indigo-400 bg-clip-text text-transparent animate-glow">
                        Munkhjargal
                    </h1>
                    <h2 class="text-4xl md:text-6xl font-bold mb-6 text-slate-300 dark:text-slate-600">
                        Amgalanbaatar
                    </h2>
                    <div class="w-32 h-1 bg-gradient-to-r from-sky-400 to-indigo-400 mx-auto mb-8 animate-glow"></div>
                </div>
                
                <p class="text-xl md:text-2xl font-mono text-slate-400 dark:text-slate-500 mb-8 leading-relaxed">
                    17-Year-Old Entrepreneur & Future Business Leader
                </p>
                
                <div class="flex flex-col sm:flex-row gap-4 justify-center items-center">
                    <div class="flex items-center gap-2 text-slate-300 dark:text-slate-600">
                        <i class="fas fa-graduation-cap text-sky-400"></i>
                        <span class="font-mono">Starting GMU Honors 2026</span>
                    </div>
                    <div class="hidden sm:block w-1 h-6 bg-slate-600 dark:bg-slate-400"></div>
                    <div class="flex items-center gap-2 text-slate-300 dark:text-slate-600">
                        <i class="fas fa-briefcase text-sky-400"></i>
                        <span class="font-mono">Brand Leader 2025</span>
                    </div>
                </div>
            </div>
            
            <!-- Scroll Indicator -->
            <div class="absolute bottom-8 left-1/2 transform -translate-x-1/2 animate-bounce">
                <div class="w-6 h-10 border-2 border-sky-400 rounded-full flex justify-center">
                    <div class="w-1 h-3 bg-sky-400 rounded-full mt-2 animate-pulse"></div>
                </div>
            </div>
        </section>

        <!-- About Section -->
        <section class="py-20 px-6 bg-slate-800/30 dark:bg-slate-200/30 backdrop-blur-sm">
            <div class="max-w-6xl mx-auto">
                <h2 class="text-5xl font-bold mb-16 text-center bg-gradient-to-r from-sky-400 to-indigo-400 bg-clip-text text-transparent reveal">
                    About Me
                </h2>
                
                <div class="grid md:grid-cols-2 gap-12 items-center">
                    <div class="reveal">
                        <div class="bg-slate-800/50 dark:bg-slate-100/50 backdrop-blur-md rounded-2xl p-8 border border-slate-700/30 dark:border-slate-400/30 hover:border-sky-400/50 transition-all duration-300">
                            <h3 class="text-2xl font-bold mb-6 text-sky-400">My Story</h3>
                            <p class="text-slate-300 dark:text-slate-600 leading-relaxed mb-4">
                                At 17 years old and turning 18 this year, I'm a high school student at Ulaanbaatar Elite International School (UIES), graduating and heading to George Mason University's Honors Program for Business Administration and Marketing in 2026.
                            </p>
                            <p class="text-slate-300 dark:text-slate-600 leading-relaxed mb-4">
                                I'm passionate about creating opportunities for others, whether through business leadership or education. As the youngest in a family of 4 brothers, I've learned the value of standing out and making my mark.
                            </p>
                            <p class="text-slate-300 dark:text-slate-600 leading-relaxed">
                                Beyond academics and business, I stay active through basketball, football, volleyball, and running. When I'm not on the field, you'll find me strategizing in CS:GO2.
                            </p>
                        </div>
                    </div>
                    
                    <div class="grid grid-cols-2 gap-6 reveal" style="animation-delay: 0.2s;">
                        <div class="bg-slate-800/50 dark:bg-slate-100/50 backdrop-blur-md rounded-xl p-6 border border-slate-700/30 dark:border-slate-400/30 hover:border-sky-400/50 transition-all duration-300 text-center">
                            <i class="fas fa-basketball-ball text-3xl text-sky-400 mb-3"></i>
                            <h4 class="font-bold text-slate-200 dark:text-slate-700">Sports</h4>
                            <p class="text-sm text-slate-400 dark:text-slate-500 font-mono">Multi-Sport Athlete</p>
                        </div>
                        
                        <div class="bg-slate-800/50 dark:bg-slate-100/50 backdrop-blur-md rounded-xl p-6 border border-slate-700/30 dark:border-slate-400/30 hover:border-sky-400/50 transition-all duration-300 text-center">
                            <i class="fas fa-gamepad text-3xl text-sky-400 mb-3"></i>
                            <h4 class="font-bold text-slate-200 dark:text-slate-700">Gaming</h4>
                            <p class="text-sm text-slate-400 dark:text-slate-500 font-mono">CS:GO2 Strategist</p>
                        </div>
                        
                        <div class="bg-slate-800/50 dark:bg-slate-100/50 backdrop-blur-md rounded-xl p-6 border border-slate-700/30 dark:border-slate-400/30 hover:border-sky-400/50 transition-all duration-300 text-center">
                            <i class="fas fa-users text-3xl text-sky-400 mb-3"></i>
                            <h4 class="font-bold text-slate-200 dark:text-slate-700">Family</h4>
                            <p class="text-sm text-slate-400 dark:text-slate-500 font-mono">Brother of 4</p>
                        </div>
                        
                        <div class="bg-slate-800/50 dark:bg-slate-100/50 backdrop-blur-md rounded-xl p-6 border border-slate-700/30 dark:border-slate-400/30 hover:border-sky-400/50 transition-all duration-300 text-center">
                            <i class="fas fa-running text-3xl text-sky-400 mb-3"></i>
                            <h4 class="font-bold text-slate-200 dark:text-slate-700">Running</h4>
                            <p class="text-sm text-slate-400 dark:text-slate-500 font-mono">Endurance Focus</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Experience Section -->
        <section class="py-20 px-6">
            <div class="max-w-6xl mx-auto">
                <h2 class="text-5xl font-bold mb-16 text-center bg-gradient-to-r from-sky-400 to-indigo-400 bg-clip-text text-transparent reveal">
                    Experience
                </h2>
                
                <div class="space-y-8">
                    <!-- Brand Director -->
                    <div class="bg-slate-800/50 dark:bg-slate-100/50 backdrop-blur-md rounded-2xl p-8 border border-slate-700/30 dark:border-slate-400/30 hover:border-sky-400/50 transition-all duration-300 reveal">
                        <div class="flex flex-col md:flex-row md:items-center md:justify-between mb-6">
                            <div>
                                <h3 class="text-2xl font-bold text-sky-400 mb-2">Brand Director</h3>
                                <p class="text-slate-300 dark:text-slate-600 font-mono">Clothing Brand</p>
                            </div>
                            <div class="text-slate-400 dark:text-slate-500 font-mono mt-2 md:mt-0">
                                <i class="fas fa-calendar-alt mr-2"></i>2025
                            </div>
                        </div>
                        
                        <div class="space-y-4">
                            <div class="flex items-start gap-3">
                                <i class="fas fa-share-alt text-sky-400 mt-1"></i>
                                <p class="text-slate-300 dark:text-slate-600">Led comprehensive social media marketing strategy, building brand presence across multiple platforms</p>
                            </div>
                            <div class="flex items-start gap-3">
                                <i class="fas fa-globe text-sky-400 mt-1"></i>
                                <p class="text-slate-300 dark:text-slate-600">Designed and developed company website from concept to launch, ensuring optimal user experience</p>
                            </div>
                            <div class="flex items-start gap-3">
                                <i class="fas fa-chart-line text-sky-400 mt-1"></i>
                                <p class="text-slate-300 dark:text-slate-600">Managed all digital marketing initiatives, driving customer engagement and brand growth</p>
                            </div>
                        </div>
                        
                        <div class="flex flex-wrap gap-2 mt-6">
                            <span class="px-3 py-1 bg-sky-400/20 text-sky-400 rounded-full text-sm font-mono">Leadership</span>
                            <span class="px-3 py-1 bg-sky-400/20 text-sky-400 rounded-full text-sm font-mono">Marketing</span>
                            <span class="px-3 py-1 bg-sky-400/20 text-sky-400 rounded-full text-sm font-mono">Web Development</span>
                            <span class="px-3 py-1 bg-sky-400/20 text-sky-400 rounded-full text-sm font-mono">Social Media</span>
                        </div>
                    </div>

                    <!-- SPARK Volunteer -->
                    <div class="bg-slate-800/50 dark:bg-slate-100/50 backdrop-blur-md rounded-2xl p-8 border border-slate-700/30 dark:border-slate-400/30 hover:border-sky-400/50 transition-all duration-300 reveal">
                        <div class="flex flex-col md:flex-row md:items-center md:justify-between mb-6">
                            <div>
                                <h3 class="text-2xl font-bold text-sky-400 mb-2">Volunteer English Teacher</h3>
                                <p class="text-slate-300 dark:text-slate-600 font-mono">SPARK Program</p>
                            </div>
                            <div class="text-slate-400 dark:text-slate-500 font-mono mt-2 md:mt-0">
                                <i class="fas fa-calendar-alt mr-2"></i>Ongoing
                            </div>
                        </div>
                        
                        <div class="space-y-4">
                            <div class="flex items-start gap-3">
                                <i class="fas fa-graduation-cap text-sky-400 mt-1"></i>
                                <p class="text-slate-300 dark:text-slate-600">Teaching English to countryside children, expanding their educational opportunities and global perspective</p>
                            </div>
                            <div class="flex items-start gap-3">
                                <i class="fas fa-heart text-sky-400 mt-1"></i>
                                <p class="text-slate-300 dark:text-slate-600">Volunteering time to bridge educational gaps and inspire young minds in rural communities</p>
                            </div>
                            <div class="flex items-start gap-3">
                                <i class="fas fa-lightbulb text-sky-400 mt-1"></i>
                                <p class="text-slate-300 dark:text-slate-600">Creating engaging lesson plans to make learning English accessible and enjoyable for students</p>
                            </div>
                        </div>
                        
                        <div class="flex flex-wrap gap-2 mt-6">
                            <span class="px-3 py-1 bg-sky-400/20 text-sky-400 rounded-full text-sm font-mono">Teaching</span>
                            <span class="px-3 py-1 bg-sky-400/20 text-sky-400 rounded-full text-sm font-mono">Community Impact</span>
                            <span class="px-3 py-1 bg-sky-400/20 text-sky-400 rounded-full text-sm font-mono">Mentoring</span>
                            <span class="px-3 py-1 bg-sky-400/20 text-sky-400 rounded-full text-sm font-mono">Social Responsibility</span>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Contact Section -->
        <section class="py-20 px-6 bg-slate-800/30 dark:bg-slate-200/30 backdrop-blur-sm">
            <div class="max-w-4xl mx-auto text-center">
                <h2 class="text-5xl font-bold mb-16 bg-gradient-to-r from-sky-400 to-indigo-400 bg-clip-text text-transparent reveal">
                    Let's Connect
                </h2>
                
                <div class="grid md:grid-cols-2 gap-8 mb-12">
                    <a href="mailto:amunkhjargal1203@gmail.com" class="group reveal">
                        <div class="bg-slate-800/50 dark:bg-slate-100/50 backdrop-blur-md rounded-2xl p-8 border border-slate-700/30 dark:border-slate-400/30 hover:border-sky-400/50 transition-all duration-300 hover:scale-105">
                            <i class="fas fa-envelope text-4xl text-sky-400 mb-4 group-hover:animate-bounce"></i>
                            <h3 class="text-xl font-bold mb-2 text-slate-200 dark:text-slate-700">Email</h3>
                            <p class="text-sky-400 font-mono break-all">amunkhjargal1203@gmail.com</p>
                        </div>
                    </a>
                    
                    <a href="tel:+97694133366" class="group reveal">
                        <div class="bg-slate-800/50 dark:bg-slate-100/50 backdrop-blur-md rounded-2xl p-8 border border-slate-700/30 dark:border-slate-400/30 hover:border-sky-400/50 transition-all duration-300 hover:scale-105">
                            <i class="fas fa-phone text-4xl text-sky-400 mb-4 group-hover:animate-bounce"></i>
                            <h3 class="text-xl font-bold mb-2 text-slate-200 dark:text-slate-700">Phone</h3>
                            <p class="text-sky-400 font-mono">+976 94133366</p>
                        </div>
                    </a>
                </div>
                
                <div class="reveal">
                    <p class="text-slate-400 dark:text-slate-500 text-lg mb-8">
                        Ready to discuss opportunities, collaborations, or just connect? I'd love to hear from you.
                    </p>
                    <div class="w-32 h-1 bg-gradient-to-r from-sky-400 to-indigo-400 mx-auto animate-glow"></div>
                </div>
            </div>
        </section>

        <!-- Footer -->
        <footer class="py-8 px-6 border-t border-slate-700/30 dark:border-slate-400/30">
            <div class="max-w-6xl mx-auto text-center">
                <p class="text-slate-400 dark:text-slate-500 font-mono">
                    © 2026 Munkhjargal Amgalanbaatar. Future Business Leader.
                </p>
            </div>
        </footer>
    </div>

    <script>
        // Theme Toggle
        const themeToggle = document.getElementById('themeToggle');
        const body = document.getElementById('body');
        
        // Load saved theme
        const savedTheme = localStorage.getItem('theme') || 'dark';
        if (savedTheme === 'light') {
            body.classList.add('dark');
        }
        
        themeToggle.addEventListener('click', () => {
            body.classList.toggle('dark');
            const isDark = !body.classList.contains('dark');
            localStorage.setItem('theme', isDark ? 'dark' : 'light');
        });

        // Custom Cursor
        const cursor = document.querySelector('.cursor');
        const cursorDot = document.querySelector('.cursor-dot');
        
        document.addEventListener('mousemove', (e) => {
            cursor.style.left = e.clientX - 10 + 'px';
            cursor.style.top = e.clientY - 10 + 'px';
            cursorDot.style.left = e.clientX - 2 + 'px';
            cursorDot.style.top = e.clientY - 2 + 'px';
        });

        // Scroll Reveal Animation
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('active');
                }
            });
        }, observerOptions);

        document.querySelectorAll('.reveal').forEach(el => {
            observer.observe(el);
        });

        // Smooth Scrolling
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });
    </script>
</body>
</html>
