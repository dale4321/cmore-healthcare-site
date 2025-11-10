
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cmore Healthcare</title>
    <!-- Load Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Configure Tailwind for Inter font -->
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@100..900&display=swap');
        body {
            font-family: 'Inter', sans-serif;
            /* Ensure the page uses flex to push footer to bottom */
            min-height: 100vh;
            display: flex;
            flex-direction: column;
        }
    </style>
</head>
<body class="bg-blue-100 text-black">

    <!-- Header Section -->
    <header class="bg-white shadow-md p-4 sticky top-0 z-10">
        <div class="container mx-auto flex flex-col md:flex-row items-center justify-between">
            
            <!-- Left: Asclepius Symbol -->
            <div class="text-blue-900 text-5xl mr-5">&#9764;</div>

            <!-- Center: Logo/Heading - STACKED VERTICALLY -->
            <div class="flex flex-col items-center space-y-2 mb-4 md:mb-0">
                <!-- LOGO IMAGE PLACEMENT: Use your relative path here (e.g., ./assets/cmore_logo.jpeg) -->
                <img 
                    src="cmore_logo image.jpg" 
                    alt="Cmore Healthcare Logo" 
                    class="h-20 w-auto rounded-md shadow-inner" 
                    onerror="this.onerror=null; this.src='https://placehold.co/80x40/003366/FFFFFF?text=Logo';"
                >
                <h1 class="text-3xl md:text-3xl font-extrabold text-blue-900 text-center">
                    Cmore Healthcare
                </h1>
            </div>

            <!-- Right: Photo Placeholder -->
            <div class="hidden md:block">
                <!-- PHOTO IMAGE PLACEMENT: Use your relative path here (e.g., ./assets/doctor_patient.png) -->
                <img 
                    src="cmore_website photo .png" 
                    alt="African American Doctor treating elderly patient" 
                    class="h-20 w-20 rounded-full shadow-lg"
                    onerror="this.onerror=null; this.src='https://placehold.co/40x40/CCCCCC/333333?text=Photo';"
                >
            </div>
        </div>
    </header>

    <!-- Main Content Area -->
    <main class="flex-grow container mx-auto p-6 md:p-12">
        <section class="text-center bg-white p-8 md:p-12 rounded-xl shadow-lg border border-blue-200">
            <h2 class="text-2xl md:text-3xl font-semibold mb-4 text-blue-800">Welcome to Comprehensive Care</h2>
            <p class="text-lg text-gray-700 max-w-3xl mx-auto">
                Cmore Healthcare provides integrated medical, consulting, and contracting services. We are dedicated to providing accessible, high-quality care to our patients whether in the office, via Zoom, or through in-home visits.
            </p>
            <div class="mt-8">
                <!-- THIS DIV IS NOW LIGHT GREEN -->
                <div class="inline-block bg-green-50 border border-green-300 p-6 rounded-xl shadow-md transition transform hover:scale-[1.02] duration-300">
                    <h3 class="text-xl font-bold text-blue-900">Patient Services Overview</h3>
                    <p class="text-sm text-gray-600 mt-1">Click below to explore our full range of medical programs and specialties.</p>
                </div>
            </div>
        </section>
        
        <!-- Additional Content Sections can go here -->

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
                <a href="#" class="block p-4 rounded-xl shadow-md border border-green-200 bg-green-50 text-center transition transform hover:scale-[1.05] hover:shadow-lg duration-300">
                    <span class="text-lg font-semibold text-blue-900">Opioid Dependence</span>
                </a>
                <a href="#" class="block p-4 rounded-xl shadow-md border border-green-200 bg-green-50 text-center transition transform hover:scale-[1.05] hover:shadow-lg duration-300">
                    <span class="text-lg font-semibold text-blue-900">Immigration Physicals</span>
                </a>
                <a href="#" class="block p-4 rounded-xl shadow-md border border-green-200 bg-green-50 text-center transition transform hover:scale-[1.05] hover:shadow-lg duration-300">
                    <span class="text-lg font-semibold text-blue-900">Weight Loss</span>
                </a>
                <a href="#" class="block p-4 rounded-xl shadow-md border border-green-200 bg-green-50 text-center transition transform hover:scale-[1.05] hover:shadow-lg duration-300">
                    <span class="text-lg font-semibold text-blue-900">VA Disability assistance</span>
                </a>
                <a href="#" class="block p-4 rounded-xl shadow-md border border-green-200 bg-green-50 text-center transition transform hover:scale-[1.05] hover:shadow-lg duration-300">
                    <span class="text-lg font-semibold text-blue-900">Patient Pay portal</span>
                </a>
                <a href="#" class="block p-4 rounded-xl shadow-md border border-green-200 bg-green-50 text-center transition transform hover:scale-[1.05] hover:shadow-lg duration-300">
                    <span class="text-lg font-semibold text-blue-900">About Cmore Healthcare</span>
                </a>
                <a href="#" class="block p-4 rounded-xl shadow-md border border-green-200 bg-green-50 text-center transition transform hover:scale-[1.05] hover:shadow-lg duration-300">
                    <span class="text-lg font-semibold text-blue-900">Scheduling</span>
                </a>
            </div>

            <p class="text-center text-sm text-gray-500 mt-8">&copy; 2025 Cmore Healthcare, LLC. All rights reserved.</p>
        </div>
    </footer>

</body>
</html>
