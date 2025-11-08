
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cmore Healthcare</title>
    <!-- Load Tailwind CSS via CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Load Inter font -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@100..900&display=swap" rel="stylesheet">
    <style>
        /* Custom font application */
        body {
            font-family: 'Inter', sans-serif;
        }
        /* Style for the logo text - larger font, darker color */
        .logo-text {
            font-size: 2.5rem; /* Large size */
            font-weight: 800; /* Extra bold */
            color: #1e3a8a; /* Dark Blue */
            letter-spacing: -1px;
        }
    </style>
</head>
<body class="bg-blue-100 text-black min-h-screen">

    <!-- Header / Navigation Bar -->
    <header class="shadow-lg bg-white p-4 sticky top-0 z-10">
        <div class="container mx-auto flex items-center justify-between">
            
            <!-- LEFT: Caduceus Medicine Symbol (SVG) -->
            <div class="flex items-center space-x-2">
                <!-- Caduceus SVG Icon -->
                <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="#1e3a8a" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-8 h-8 md:w-10 md:h-10">
                    <path d="M12 2L12 12M12 12L15 9M12 12L9 9M15 12C15 15.3137 12 18 12 18C12 18 9 15.3137 9 12M12 18L12 22"/>
                    <path d="M18 16L6 8"/>
                </svg>
            </div>

            <!-- CENTER: Company Logo Text (Visible on larger screens) -->
            <div class="hidden md:block absolute left-1/2 transform -translate-x-1/2">
                <h1 class="logo-text">Cmore Healthcare</h1>
            </div>
            <!-- CENTER (Mobile Fallback): Company Title (Visible on smaller screens) -->
            <div class="md:hidden">
                 <h1 class="text-xl font-bold text-blue-900">Cmore Healthcare</h1>
            </div>
            
            <!-- RIGHT: Navigation Links -->
            <nav>
                <!-- Link container for responsive wrapping -->
                <!-- The 'justify-end' class ensures the links are pushed to the right boundary. -->
                <div class="flex flex-wrap justify-end gap-2 text-sm md:text-base">
                    <!-- Links -->
                    <a href="#" class="nav-link">Family Care</a>
                    <a href="#" class="nav-link">Opioid Dependence</a>
                    <a href="#" class="nav-link">Immigration Physicals</a>
                    <a href="#" class="nav-link">Weight Loss</a>
                    <a href="#" class="nav-link">VA Disability assistance</a>
                    <a href="#" class="nav-link">Patient Pay portal</a>
                    <a href="#" class="nav-link">About Cmore Healthcare</a>
                </div>
            </nav>
        </div>
    </header>

    <!-- Main Content Area -->
    <main class="container mx-auto p-8 pt-12">
        <div class="bg-white p-8 rounded-xl shadow-xl max-w-4xl mx-auto">
            <h2 class="text-3xl font-semibold text-blue-800 mb-4">Comprehensive, Coordinated Care</h2>
            <p class="text-gray-700 leading-relaxed mb-6">
                Cmore Healthcare provides integrated medical services, including direct patient care (in-office, via Zoom, and in-home visits), specialized consulting services, and professional placement for medical providers. We are committed to high-quality care and streamlined administrative support for both patients and industry partners.
            </p>

            <div class="grid md:grid-cols-3 gap-6 mt-8">
                <div class="p-4 bg-blue-50 rounded-lg border border-blue-200">
                    <h3 class="font-bold text-blue-700">Patient Services</h3>
                    <p class="text-sm mt-1">Visit our office, schedule a telehealth call, or request an in-home visit for comprehensive care.</p>
                </div>
                <div class="p-4 bg-blue-50 rounded-lg border border-blue-200">
                    <h3 class="font-bold text-blue-700">Consulting & Contracting</h3>
                    <p class="text-sm mt-1">We specialize in managing consultant relationships and recruiting specialized medical staff.</p>
                </div>
                <div class="p-4 bg-blue-50 rounded-lg border border-blue-200">
                    <h3 class="font-bold text-blue-700">Access Your Services</h3>
                    <p class="text-sm mt-1">Click on the links above to quickly access our service pages or the patient payment portal.</p>
                </div>
            </div>
        </div>
    </main>

    <!-- Hidden Style Definition for Navigation Links -->
    <style>
        .nav-link {
            /* White background, dark blue text, rounded corners */
            @apply bg-white text-blue-900 font-medium py-2 px-4 rounded-full shadow-md transition duration-300 ease-in-out hover:bg-blue-100 hover:shadow-lg focus:outline-none focus:ring-2 focus:ring-blue-500 focus:ring-opacity-50 whitespace-nowrap;
        }
    </style>
</body>
</html>
