
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cmore Healthcare</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@100..900&display=swap');
        
        /* Custom utility for better text contrast over the background image */
        .text-shadow-sm {
            text-shadow: 1px 1px 2px rgba(255, 255, 255, 0.7); /* Subtle white glow */
        }

        body { 
            font-family: 'Inter', sans-serif; 
            /* Ensure the page uses flex to push footer to bottom */ 
            min-height: 100vh; 
            display: flex; 
            flex-direction: column; 
            background-color: #f7fafc; /* Light background for contrast */ 
        } 
        
        .container { 
            max-width: 1000px; 
        } 
        
        /* Style for the active navigation link */ 
        .nav-link.active { 
            color: #1e40af; /* Tailwind blue-700 */ 
            border-bottom: 3px solid #1e40af; 
            font-weight: 700; 
        } 
        
        /* Hide all pages by default, JavaScript handles showing the active one */ 
        .page-content { 
            display: none; 
        }

        /* NEW: Header background style with logo watermark (Adjusted to 50% width and slightly tinted background) */
        .header-watermark {
            /* Changed to a very subtle light blue background for better contrast against the logo */
            background-color: #f0f8ff; 
            
            background-image: url('uploaded:image_15f626.png-8a0cadcb-b528-410d-a50d-44d076dcfdc8'); 
            
            background-repeat: no-repeat;
            
            /* CRITICAL CHANGE: Reduced size to 50% for greater color density */
            background-size: 50% auto;
            
            /* Center the background image */
            background-position: center; 
        }
    </style>
</head>
<body>

<div class="flex-grow">
    <!-- Header Section (Increased vertical padding for better logo display area) -->
    <header class="header-watermark shadow-lg py-6 px-4 sticky top-0 z-10">
        <div class="container mx-auto flex flex-col items-center">
            
            <!-- Top Row: Icons and Logo -->
            <div class="flex items-center justify-between w-full max-w-lg">
                <!-- Left: Asclepius Symbol -->
                <div class="text-blue-900 text-5xl mr-5 text-shadow-sm">&#9764;</div>

                <!-- Center: Logo/Heading (Simplified to text, relying on CSS for background logo) -->
                <div class="flex flex-col items-center space-y-2 mb-4 md:mb-0">
                    <!-- Title Text sits on top of the logo background -->
                    <h1 class="text-4xl md:text-4xl font-black text-blue-900 text-center leading-tight text-shadow-sm">
                        Cmore Healthcare
                    </h1>
                    <p class="text-sm text-gray-700 italic text-shadow-sm">Comprehensive healthcare when it counts!</p>
                </div>

                <!-- Right: Photo Placeholder -->
                <div class="hidden md:block">
                    <img 
                        src="cmore_website photo .png" 
                        alt="African American Doctor treating elderly patient" 
                        class="h-20 w-20 rounded-full shadow-lg"
                        onerror="this.onerror=null; this.src='https://placehold.co/40x40/CCCCCC/333333?text=Photo';"
                    >
                </div>
            </div>

            <!-- Navigation Links (NEW: Added to manage pages) -->
            <nav class="flex space-x-8 mt-4 border-t border-gray-100 pt-3">
                <a href="#" data-page="home" class="nav-link text-gray-700 hover:text-blue-600 p-2 transition duration-150">Home</a>
                <a href="#" data-page="contact" class="nav-link text-gray-700 hover:text-blue-600 p-2 transition duration-150">Contact Us</a>
                <!-- You can add more links here (e.g., data-page="services") -->
            </nav>
        </div>
    </header>

    <!-- Main Content Area -->
    <main class="container mx-auto p-4 md:p-6 lg:p-8 flex-grow">
        
        <!-- 1. HOME Page Content (Your original content) -->
        <section id="page-home" class="page-content bg-white p-8 md:p-12 rounded-xl shadow-lg border border-blue-200">
            <h2 class="text-2xl md:text-3xl font-semibold mb-4 text-blue-800 text-center">Welcome to Comprehensive Care</h2>
            <p class="text-lg text-gray-700 max-w-3xl mx-auto text-center">
                Cmore Healthcare is dedicated to providing accessible, high-quality care to our patients whether in the office, via Zoom, or through in-home visits.
            </p>
            <div class="mt-8 text-center">
                <div class="inline-block bg-green-50 border border-green-300 p-6 rounded-xl shadow-md transition transform hover:scale-[1.02] duration-300">
                    <h3 class="text-xl font-bold text-blue-900">Patient Services Overview</h3>
                    <p class="text-sm text-gray-600 mt-1">Click below to explore our full range of medical programs and specialties.</p>
                </div>
            </div>
        </section>
        
        <!-- 2. CONTACT Page Content (The requested section) -->
        <section id="page-contact" class="page-content bg-white p-6 rounded-xl shadow-lg border border-blue-200">
            <h2 class="text-4xl font-black text-gray-900 mb-6 border-b-4 border-blue-100 pb-3">
                Contact Our Family Care Team
            </h2>
            <div class="space-y-6">
                <p class="text-lg text-gray-600">
                    We are here to support your family's health journey. Please use the information below to reach out.
                </p>
                
                <!-- Contact Details: Grid layout for Phone/Email -->
                <div class="grid md:grid-cols-2 gap-6 p-4 bg-gray-50 rounded-lg shadow-inner">
                    <!-- Phone & Appointments -->
                    <div class="space-y-2">
                        <h3 class="font-bold text-xl text-blue-700">Phone & Appointments</h3>
                        <p class="text-gray-700">
                            <span class="font-semibold">Main Office:</span> <a href="tel:+1-425-347-3689" class="text-blue-600 hover:text-blue-800 underline block">(425) 347-3689</a>
                            <span class="text-sm text-gray-500 block">Call during business hours for appointments.</span>
                        </p>
                    </div>
                    <!-- Email Inquiry -->
                    <div class="space-y-2">
                        <h3 class="font-bold text-xl text-blue-700">Email Inquiry</h3>
                        <p class="text-gray-700">
                            <span class="font-semibold">General Inquiries:</span> <a href="mailto:cmorehealthcare@hotmail.com" class="text-blue-600 hover:text-blue-800 underline block">cmorehealthcare@hotmail.com</a>
                            <span class="text-sm text-gray-500 block">Please do not send urgent medical questions via email.</span>
                        </p>
                    </div>
                </div>

                <!-- Location Mockup -->
                <div class="p-4 bg-white rounded-lg border border-gray-200 shadow-sm">
                    <h3 class="font-bold text-xl text-blue-700 mb-2">Clinic Location</h3>
                    <p class="text-gray-700">12822 SE 32nd St Suite: 216 Bellevue Wa. 98005</p>
                    <p class="text-sm text-gray-500 mt-1">We are located conveniently near down town.</p>
                </div>
            </div>
        </section>
        
        <!-- Additional Content Sections (Footer Boxes moved to footer) -->

    </main>

    <!-- Footer Navigation Section (Styled as Boxes) -->
    <footer class="bg-white p-6 md:p-10 shadow-inner mt-auto">
        <div class="container mx-auto">
            <h3 class="text-center text-2xl font-bold mb-6 text-blue-800">Our Services & Access Points</h3>
            
            <!-- Grid for the 8 Service Links -->
            <div class="grid grid-cols-2 sm:grid-cols-3 lg:grid-cols-4 gap-4 md:gap-6">
                <!-- Link Box Structure (Dark Blue Text, Light Green Background) -->
                <a href="family-medicine.html" class="block p-4 rounded-xl shadow-md border border-green-200 bg-green-50 text-center transition transform hover:scale-[1.05] hover:shadow-lg duration-300">
                    <span class="text-lg font-semibold text-blue-900">Family Care</span>
                </a>
                <a href="opioid-dependence.html" class="block p-4 rounded-xl shadow-md border border-green-200 bg-green-50 text-center transition transform hover:scale-[1.05] hover:shadow-lg duration-300">
                    <span class="text-lg font-semibold text-blue-900">Opioid Dependence</span>
                </a>
                <a href="immigration-physical.html" class="block p-4 rounded-xl shadow-md border border-green-200 bg-green-50 text-center transition transform hover:scale-[1.05] hover:shadow-lg duration-300">
                    <span class="text-lg font-semibold text-blue-900">Immigration Physicals</span>
                </a>
                <a href="weight-loss.html" class="block p-4 rounded-xl shadow-md border border-green-200 bg-green-50 text-center transition transform hover:scale-[1.05] hover:shadow-lg duration-300">
                    <span class="text-lg font-semibold text-blue-900">Weight Loss</span>
                </a>
                <a href="veterans-disability.html" class="block p-4 rounded-xl shadow-md border border-green-200 bg-green-50 text-center transition transform hover:scale-[1.05] hover:shadow-lg duration-300">
                    <span class="text-lg font-semibold text-blue-900">VA Disability assistance</span>
                </a>
                <a href="business-cardss.html" class="block p-4 rounded-xl shadow-md border border-green-200 bg-green-50 text-center transition transform hover:scale-[1.05] hover:shadow-lg duration-300">
                    <span class="text-lg font-semibold text-blue-900">Patient Pay portal</span>
                </a>
                <a href="about-uss.html" class="block p-4 rounded-xl shadow-md border border-green-200 bg-green-50 text-center transition transform hover:scale-[1.05] hover:shadow-lg duration-300">
                    <span class="text-lg font-semibold text-blue-900">About Cmore Healthcare</span>
                </a>
                <a href="scheduling-options.html" class="block p-4 rounded-xl shadow-md border border-green-200 bg-green-50 text-center transition transform hover:scale-[1.05] hover:shadow-lg duration-300">
                    <span class="text-lg font-semibold text-blue-900">Scheduling</span>
                </a>
            </div>

            <p class="text-center text-sm text-gray-500 mt-8">&copy; 2025 Cmore Healthcare, LLC. All rights reserved.</p>
        </div>
    </footer>
</div>

<!-- JavaScript for Page Navigation -->
<script>
    document.addEventListener('DOMContentLoaded', () => {
        const navLinks = document.querySelectorAll('.nav-link');
        const contentSections = document.querySelectorAll('.page-content');

        // Function to handle showing the correct page
        function showPage(pageId) {
            // 1. Hide all content sections
            contentSections.forEach(section => {
                section.style.display = 'none';
            });

            // 2. Show the requested content section
            const targetSection = document.getElementById(`page-${pageId}`);
            if (targetSection) {
                targetSection.style.display = 'block';
            }

            // 3. Update active link class
            navLinks.forEach(link => {
                link.classList.remove('active');
                if (link.getAttribute('data-page') === pageId) {
                    link.classList.add('active');
                }
            });
        }

        // Add click listeners to navigation links
        navLinks.forEach(link => {
            link.addEventListener('click', (e) => {
                e.preventDefault(); 
                const pageId = e.target.getAttribute('data-page');
                if (pageId) {
                    showPage(pageId);
                }
            });
        });

        // Set the default page to 'home' on initial load
        showPage('home');
    });
</script>
</body>
</html>
