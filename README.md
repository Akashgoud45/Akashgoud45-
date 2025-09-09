<!DOCTYPE html>  <html lang="en" class="scroll-smooth">  
<head>  
    <meta charset="UTF-8">  
    <meta name="viewport" content="width=device-width, initial-scale=1.0">  
    <title>DAVV Sports Hub - Selections, Tournaments & News</title>  <!-- Tailwind CSS -->  
<script src="https://cdn.tailwindcss.com"></script>  
  
<!-- Google Fonts: Inter -->  
<link rel="preconnect" href="https://fonts.googleapis.com">  
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>  
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">  
  
<!-- Custom Styles -->  
<style>  
    body {  
        font-family: 'Inter', sans-serif;  
        background-color: #f8fafc; /* Tailwind's gray-50 */  
    }  
    .hero-section {  
        background: linear-gradient(rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.6)), url('https://placehold.co/1920x1080/000000/FFFFFF?text=DAVV+Sports+Action') no-repeat center center;  
        background-size: cover;  
    }  
    .section-title {  
        position: relative;  
        padding-bottom: 0.5rem;  
        margin-bottom: 1rem;  
    }  
    .section-title::after {  
        content: '';  
        position: absolute;  
        bottom: 0;  
        left: 50%;  
        transform: translateX(-50%);  
        width: 80px;  
        height: 4px;  
        background-color: #f97316; /* Tailwind's orange-500 */  
        border-radius: 2px;  
    }  
</style>

</head>  
<body class="bg-gray-50 text-gray-800">  <!-- Header & Navigation -->  
<header class="bg-white/80 backdrop-blur-md shadow-md sticky top-0 z-50">  
    <nav class="container mx-auto px-6 py-3">  
        <div class="flex justify-between items-center">  
            <div class="flex items-center space-x-3">  
                <svg class="w-10 h-10 text-orange-500" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">  
                    <path stroke-linecap="round" stroke-linejoin="round" d="M12 6.75a.75.75 0 110-1.5.75.75 0 010 1.5zM12 12.75a.75.75 0 110-1.5.75.75 0 010 1.5zM12 18.75a.75.75 0 110-1.5.75.75 0 010 1.5z" />  
                    <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 6A2.25 2.25 0 016 3.75h2.25A2.25 2.25 0 0110.5 6v2.25a2.25 2.25 0 01-2.25 2.25H6a2.25 2.25 0 01-2.25-2.25V6zM3.75 14.25A2.25 2.25 0 016 12h2.25a2.25 2.25 0 012.25 2.25v2.25a2.25 2.25 0 01-2.25 2.25H6a2.25 2.25 0 01-2.25-2.25v-2.25zM13.5 6A2.25 2.25 0 0115.75 3.75h2.25A2.25 2.25 0 0120.25 6v2.25a2.25 2.25 0 01-2.25 2.25h-2.25a2.25 2.25 0 01-2.25-2.25V6zM13.5 14.25A2.25 2.25 0 0115.75 12h2.25a2.25 2.25 0 012.25 2.25v2.25a2.25 2.25 0 01-2.25 2.25h-2.25a2.25 2.25 0 01-2.25-2.25v-2.25z" />  
                </svg>  
                <a href="#" class="text-2xl font-bold text-gray-800">DAVV Sports Hub</a>  
            </div>  
            <!-- Desktop Menu -->  
            <div class="hidden md:flex items-center space-x-6">  
                <a href="#announcements" class="text-gray-600 hover:text-orange-500 transition-colors duration-300 font-medium">Announcements</a>  
                <a href="#tournaments" class="text-gray-600 hover:text-orange-500 transition-colors duration-300 font-medium">Tournaments</a>  
                <a href="#games" class="text-gray-600 hover:text-orange-500 transition-colors duration-300 font-medium">Games</a>  
                <a href="#trials" class="text-gray-600 hover:text-orange-500 transition-colors duration-300 font-medium">Selection Trials</a>  
            </div>  
            <!-- Mobile Menu Button -->  
            <div class="md:hidden">  
                <button id="mobile-menu-button" class="text-gray-800 focus:outline-none">  
                    <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7"></path></svg>  
                </button>  
            </div>  
        </div>  
        <!-- Mobile Menu -->  
        <div id="mobile-menu" class="hidden md:hidden py-4">  
            <a href="#announcements" class="block py-2 px-4 text-sm text-gray-700 hover:bg-orange-100 rounded">Announcements</a>  
            <a href="#tournaments" class="block py-2 px-4 text-sm text-gray-700 hover:bg-orange-100 rounded">Tournaments</a>  
            <a href="#games" class="block py-2 px-4 text-sm text-gray-700 hover:bg-orange-100 rounded">Games</a>  
            <a href="#trials" class="block py-2 px-4 text-sm text-gray-700 hover:bg-orange-100 rounded">Selection Trials</a>  
        </div>  
    </nav>  
</header>  

<main>  
    <!-- Hero Section -->  
    <section class="hero-section text-white h-[60vh] flex items-center justify-center">  
        <div class="text-center">  
            <h1 class="text-4xl md:text-6xl font-extrabold mb-4 drop-shadow-lg">Unleash Your Potential</h1>  
            <p class="text-lg md:text-2xl mb-8 max-w-2xl mx-auto drop-shadow">Join the legacy of champions at DAVV. Explore upcoming trials, tournaments, and events.</p>  
            <a href="#trials" class="bg-orange-500 hover:bg-orange-600 text-white font-bold py-3 px-8 rounded-full text-lg transition duration-300 ease-in-out transform hover:scale-105">Participate Now</a>  
        </div>  
    </section>  

    <!-- Announcements Section -->  
    <section id="announcements" class="py-16 md:py-24 bg-white">  
        <div class="container mx-auto px-6">  
            <h2 class="text-3xl md:text-4xl font-bold text-center mb-12 section-title">Latest Announcements</h2>  
            <div class="space-y-8 max-w-4xl mx-auto">  
                <!-- Announcement Item 1 -->  
                <div class="bg-gray-50 p-6 rounded-lg shadow-md hover:shadow-xl transition-shadow duration-300 border-l-4 border-orange-500">  
                    <div class="flex justify-between items-start">  
                        <div>  
                            <h3 class="text-xl font-semibold text-gray-900 mb-2">Cricket Team Selection Trials 2025</h3>  
                            <p class="text-gray-600">Open trials for the university men's cricket team will be held at the University Ground. All interested students must register online.</p>  
                        </div>  
                        <span class="bg-red-100 text-red-800 text-xs font-medium ml-4 px-2.5 py-0.5 rounded-full whitespace-nowrap">NEW</span>  
                    </div>  
                    <div class="mt-4 text-sm text-gray-500 flex items-center space-x-4">  
                        <span><strong>Date:</strong> 25th September 2025</span>  
                        <span><strong>Venue:</strong> University Ground, Takshashila Campus</span>  
                    </div>  
                </div>  
                <!-- Announcement Item 2 -->  
                <div class="bg-gray-50 p-6 rounded-lg shadow-md hover:shadow-xl transition-shadow duration-300 border-l-4 border-orange-500">  
                    <h3 class="text-xl font-semibold text-gray-900 mb-2">Inter-College Kabaddi Tournament Schedule Released</h3>  
                    <p class="text-gray-600">The schedule for the upcoming inter-college Kabaddi championship is now available. Captains are requested to attend the pre-tournament meeting.</p>  
                    <div class="mt-4 text-sm text-gray-500 flex items-center space-x-4">  
                        <span><strong>Tournament Starts:</strong> 10th October 2025</span>  
                        <span><strong>Details:</strong> <a href="#" class="text-orange-600 hover:underline">Download PDF</a></span>  
                    </div>  
                </div>  
                <!-- Announcement Item 3 -->  
                <div class="bg-gray-50 p-6 rounded-lg shadow-md hover:shadow-xl transition-shadow duration-300 border-l-4 border-orange-500">  
                    <h3 class="text-xl font-semibold text-gray-900 mb-2">Volleyball (M/F) Nodal Competitions</h3>  
                    <p class="text-gray-600">All affiliated colleges under the Indore Nodal center are invited to send their entries for the Volleyball championship before the deadline.</p>  
                    <div class="mt-4 text-sm text-gray-500 flex items-center space-x-4">  
                       <span><strong>Last Date for Entry:</strong> 5th October 2025</span>  
                       <span><strong>Contact:</strong> Sports Department Office</span>  
                    </div>  
                </div>  
            </div>  
        </div>  
    </section>  

    <!-- Tournaments Section -->  
    <section id="tournaments" class="py-16 md:py-24">  
        <div class="container mx-auto px-6">  
            <h2 class="text-3xl md:text-4xl font-bold text-center mb-12 section-title">Tournaments & Competitions</h2>  
            <div class="grid md:grid-cols-2 gap-12">  
                <!-- Nodal Tournaments -->  
                <div>  
                    <h3 class="text-2xl font-semibold text-center mb-6">Nodal Tournaments</h3>  
                    <div class="space-y-6">  
                        <div class="bg-white p-5 rounded-lg shadow-md hover:scale-105 transition-transform duration-300">  
                            <h4 class="font-bold text-lg">Indore Nodal Center</h4>  
                            <p class="text-gray-600 text-sm mt-1">Hosting Football, Basketball, and Table Tennis this season. Fixtures to be announced soon.</p>  
                        </div>  
                        <div class="bg-white p-5 rounded-lg shadow-md hover:scale-105 transition-transform duration-300">  
                            <h4 class="font-bold text-lg">Ujjain Nodal Center</h4>  
                            <p class="text-gray-600 text-sm mt-1">Get ready for Athletics, Badminton, and Chess competitions. Prepare your teams!</p>  
                        </div>  
                         <div class="bg-white p-5 rounded-lg shadow-md hover:scale-105 transition-transform duration-300">  
                            <h4 class="font-bold text-lg">Khandwa Nodal Center</h4>  
                            <p class="text-gray-600 text-sm mt-1">Focusing on traditional games: Kho-Kho and Kabaddi. A celebration of our sporting roots.</p>  
                        </div>  
                    </div>  
                </div>  
                <!-- Inter-College Competitions -->  
                <div>  
                    <h3 class="text-2xl font-semibold text-center mb-6">Inter-College Competitions</h3>  
                    <div class="space-y-6">  
                        <div class="bg-white p-5 rounded-lg shadow-md hover:scale-105 transition-transform duration-300">  
                            <h4 class="font-bold text-lg">Annual Sports Fest "SPARDHA"</h4>  
                            <p class="text-gray-600 text-sm mt-1">The flagship event featuring over 15 sports. A battle for the ultimate championship trophy.</p>  
                        </div>  
                        <div class="bg-white p-5 rounded-lg shadow-md hover:scale-105 transition-transform duration-300">  
                            <h4 class="font-bold text-lg">Cricket Champions League</h4>  
                            <p class="text-gray-600 text-sm mt-1">The most awaited T20 cricket tournament. College rivalries ignite on the pitch.</p>  
                        </div>  
                        <div class="bg-white p-5 rounded-lg shadow-md hover:scale-105 transition-transform duration-300">  
                            <h4 class="font-bold text-lg">Volleyball Pro League</h4>  
                            <p class="text-gray-600 text-sm mt-1">Showcase your spiking and blocking skills. The best volleyball talent goes head-to-head.</p>  
                        </div>  
                    </div>  
                </div>  
            </div>  
        </div>  
    </section>  

    <!-- Games Section -->  
    <section id="games" class="py-16 md:py-24 bg-white">  
        <div class="container mx-auto px-6">  
            <h2 class="text-3xl md:text-4xl font-bold text-center mb-12 section-title">Our Games</h2>  
            <div class="grid grid-cols-2 sm:grid-cols-3 lg:grid-cols-4 xl:grid-cols-5 gap-8">  
                <!-- Game Card -->  
                <div class="group text-center">  
                    <div class="bg-gray-100 rounded-lg p-6 flex items-center justify-center aspect-square group-hover:bg-orange-500 transition-colors duration-300">  
                        <!-- Icon Placeholder -->  
                        <img src="https://placehold.co/80x80/f97316/FFFFFF?text=🏏" alt="Cricket Icon" class="h-20 w-20 group-hover:hidden transition-all duration-300"/>  
                         <span class="text-white text-lg font-bold hidden group-hover:block">Cricket</span>  
                    </div>  
                    <h3 class="mt-4 font-semibold text-lg">Cricket</h3>  
                </div>  
                 <!-- Game Card -->  
                <div class="group text-center">  
                    <div class="bg-gray-100 rounded-lg p-6 flex items-center justify-center aspect-square group-hover:bg-orange-500 transition-colors duration-300">  
                       <img src="https://placehold.co/80x80/f97316/FFFFFF?text=🏐" alt="Volleyball Icon" class="h-20 w-20 group-hover:hidden transition-all duration-300"/>  
                       <span class="text-white text-lg font-bold hidden group-hover:block">Volleyball</span>  
                    </div>  
                    <h3 class="mt-4 font-semibold text-lg">Volleyball</h3>  
                </div>  
                 <!-- Game Card -->  
                <div class="group text-center">  
                    <div class="bg-gray-100 rounded-lg p-6 flex items-center justify-center aspect-square group-hover:bg-orange-500 transition-colors duration-300">  
                       <img src="https://placehold.co/80x80/f97316/FFFFFF?text=🏃" alt="Kabaddi Icon" class="h-20 w-20 group-hover:hidden transition-all duration-300"/>  
                       <span class="text-white text-lg font-bold hidden group-hover:block">Kabaddi</span>  
                    </div>  
                    <h3 class="mt-4 font-semibold text-lg">Kabaddi</h3>  
                </div>  
                 <!-- Game Card -->  
                <div class="group text-center">  
                    <div class="bg-gray-100 rounded-lg p-6 flex items-center justify-center aspect-square group-hover:bg-orange-500 transition-colors duration-300">  
                        <img src="https://placehold.co/80x80/f97316/FFFFFF?text=👯" alt="Kho-Kho Icon" class="h-20 w-20 group-hover:hidden transition-all duration-300"/>  
                       <span class="text-white text-lg font-bold hidden group-hover:block">Kho-Kho</span>  
                    </div>  
                    <h3 class="mt-4 font-semibold text-lg">Kho-Kho</h3>  
                </div>  
                 <!-- Game Card -->  
                <div class="group text-center">  
                    <div class="bg-gray-100 rounded-lg p-6 flex items-center justify-center aspect-square group-hover:bg-orange-500 transition-colors duration-300">  
                       <img src="https://placehold.co/80x80/f97316/FFFFFF?text=⚽" alt="Football Icon" class="h-20 w-20 group-hover:hidden transition-all duration-300"/>  
                       <span class="text-white text-lg font-bold hidden group-hover:block">Football</span>  
                    </div>  
                    <h3 class="mt-4 font-semibold text-lg">Football</h3>  
                </div>  
                 <!-- Add more games as needed -->  
                 <div class="group text-center">  
                    <div class="bg-gray-100 rounded-lg p-6 flex items-center justify-center aspect-square group-hover:bg-orange-500 transition-colors duration-300">  
                       <img src="https://placehold.co/80x80/f97316/FFFFFF?text=🏀" alt="Basketball Icon" class="h-20 w-20 group-hover:hidden transition-all duration-300"/>  
                       <span class="text-white text-lg font-bold hidden group-hover:block">Basketball</span>  
                    </div>  
                    <h3 class="mt-4 font-semibold text-lg">Basketball</h3>  
                </div>  
                <div class="group text-center">  
                    <div class="bg-gray-100 rounded-lg p-6 flex items-center justify-center aspect-square group-hover:bg-orange-500 transition-colors duration-300">  
                       <img src="https://placehold.co/80x80/f97316/FFFFFF?text=🏸" alt="Badminton Icon" class="h-20 w-20 group-hover:hidden transition-all duration-300"/>  
                       <span class="text-white text-lg font-bold hidden group-hover:block">Badminton</span>  
                    </div>  
                    <h3 class="mt-4 font-semibold text-lg">Badminton</h3>  
                </div>  
                 <div class="group text-center">  
                    <div class="bg-gray-100 rounded-lg p-6 flex items-center justify-center aspect-square group-hover:bg-orange-500 transition-colors duration-300">  
                       <img src="https://placehold.co/80x80/f97316/FFFFFF?text=🏓" alt="Table Tennis Icon" class="h-20 w-20 group-hover:hidden transition-all duration-300"/>  
                       <span class="text-white text-lg font-bold hidden group-hover:block">Table Tennis</span>  
                    </div>  
                    <h3 class="mt-4 font-semibold text-lg">Table Tennis</h3>  
                </div>  
                 <div class="group text-center">  
                    <div class="bg-gray-100 rounded-lg p-6 flex items-center justify-center aspect-square group-hover:bg-orange-500 transition-colors duration-300">  
                       <img src="https://placehold.co/80x80/f97316/FFFFFF?text=♟️" alt="Chess Icon" class="h-20 w-20 group-hover:hidden transition-all duration-300"/>  
                       <span class="text-white text-lg font-bold hidden group-hover:block">Chess</span>  
                    </div>  
                    <h3 class="mt-4 font-semibold text-lg">Chess</h3>  
                </div>  
                 <div class="group text-center">  
                    <div class="bg-gray-100 rounded-lg p-6 flex items-center justify-center aspect-square group-hover:bg-orange-500 transition-colors duration-300">  
                       <img src="https://placehold.co/80x80/f97316/FFFFFF?text=🏅" alt="Athletics Icon" class="h-20 w-20 group-hover:hidden transition-all duration-300"/>  
                       <span class="text-white text-lg font-bold hidden group-hover:block">Athletics</span>  
                    </div>  
                    <h3 class="mt-4 font-semibold text-lg">Athletics</h3>  
                </div>  
            </div>  
        </div>  
    </section>  

    <!-- Selection Trials Section -->  
    <section id="trials" class="py-16 md:py-24">  
        <div class="container mx-auto px-6">  
            <h2 class="text-3xl md:text-4xl font-bold text-center mb-12 section-title">Selection Process</h2>  
            <div class="max-w-3xl mx-auto grid md:grid-cols-3 gap-8 text-center">  
                <!-- Step 1 -->  
                <div class="bg-white p-6 rounded-lg shadow-lg">  
                    <div class="bg-orange-500 text-white rounded-full w-12 h-12 flex items-center justify-center text-2xl font-bold mx-auto mb-4">1</div>  
                    <h3 class="font-semibold text-lg mb-2">Register Online</h3>  
                    <p class="text-gray-600 text-sm">Keep an eye on the announcements for trial dates and fill out the registration form before the deadline.</p>  
                </div>  
                <!-- Step 2 -->  
                <div class="bg-white p-6 rounded-lg shadow-lg">  
                    <div class="bg-orange-500 text-white rounded-full w-12 h-12 flex items-center justify-center text-2xl font-bold mx-auto mb-4">2</div>  
                    <h3 class="font-semibold text-lg mb-2">Attend Trials</h3>  
                    <p class="text-gray-600 text-sm">Attend the selection trials on the specified date with your college ID and proper sports kit.</p>  
                </div>  
                <!-- Step 3 -->  
                <div class="bg-white p-6 rounded-lg shadow-lg">  
                    <div class="bg-orange-500 text-white rounded-full w-12 h-12 flex items-center justify-center text-2xl font-bold mx-auto mb-4">3</div>  
                    <h3 class="font-semibold text-lg mb-2">Get Selected</h3>  
                    <p class="text-gray-600 text-sm">Perform your best! The final list of selected players will be published here and on the department notice board.</p>  
                </div>  
            </div>  
        </div>  
    </section>  
</main>  

<!-- Footer -->  
<footer class="bg-gray-800 text-white">  
    <div class="container mx-auto px-6 py-8">  
        <div class="md:flex justify-between items-center text-center md:text-left">  
            <div>  
                <h3 class="text-xl font-bold">DAVV Sports Department</h3>  
                <p class="text-gray-400 mt-1">Takshashila Campus, Khandwa Road, Indore (M.P.)</p>  
            </div>  
            <div class="mt-6 md:mt-0">  
                <p>&copy; 2025 Devi Ahilya Vishwavidyalaya. All Rights Reserved.</p>  
            </div>  
        </div>  
    </div>  
</footer>  

<!-- JavaScript for Mobile Menu -->  
<script>  
    document.getElementById('mobile-menu-button').addEventListener('click', function() {  
        var menu = document.getElementById('mobile-menu');  
        if (menu.classList.contains('hidden')) {  
            menu.classList.remove('hidden');  
        } else {  
            menu.classList.add('hidden');  
        }  
    });  

    // Close mobile menu when a link is clicked  
    document.querySelectorAll('#mobile-menu a').forEach(function(link) {  
        link.addEventListener('click', function() {  
            document.getElementById('mobile-menu').classList.add('hidden');  
        });  
    });  
</script>

</body>  
</html>  
Output for this code
