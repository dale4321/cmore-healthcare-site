<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- 
        *** IMPORTANT ***
        This is where the text "cmore-healthcare-site" was likely located.
        We have updated it to reflect the new, official site title.
    -->
    <title>CMORE Healthcare Site</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f8f9fa; /* Light grey background */
        }
    </style>
</head>
<body class="min-h-screen flex flex-col antialiased">

    <!-- Header / Navigation Bar -->
    <header class="bg-white shadow-md">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-4 flex justify-between items-center">
            <!-- 
                *** IMPORTANT ***
                Ensure this logo or text matches your new company name 
            -->
            <h1 class="text-2xl font-bold text-indigo-700">CMORE Healthcare</h1>
            <nav class="hidden md:flex space-x-8">
                <a href="#" class="text-gray-600 hover:text-indigo-600 transition duration-150">Home</a>
                <a href="#" class="text-gray-600 hover:text-indigo-600 transition duration-150">Services</a>
                <a href="#" class="text-gray-600 hover:text-indigo-600 transition duration-150">About Us</a>
                <a href="#" class="text-gray-600 hover:text-indigo-600 transition duration-150">Contact</a>
            </nav>
            <button class="md:hidden p-2 rounded-md text-gray-400 hover:text-gray-500 hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-inset focus:ring-indigo-500">
                <!-- Mobile menu icon (Placeholder SVG for simplicity) -->
                <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7" />
                </svg>
            </button>
        </div>
    </header>

    <!-- Main Content Area -->
    <main class="flex-grow">
        <div class="max-w-7xl mx-auto py-12 px-4 sm:px-6 lg:px-8">
            <div class="bg-white p-8 md:p-12 rounded-xl shadow-2xl text-center">
                <!-- 
                    *** IMPORTANT ***
                    This is the visible H1 heading on the page itself.
                    We have updated it to match the new company name.
                -->
                <h2 class="text-5xl font-extrabold text-gray-900 tracking-tight mb-4">
                    Welcome to CMORE Healthcare
                </h2>
                <p class="mt-4 text-xl text-gray-500 max-w-3xl mx-auto">
                    Your custom domain, <span class="font-bold text-indigo-600">cmorehealthcare.com</span>, is now correctly resolving to this page!
                </p>
                
                <div class="mt-10 flex justify-center">
                    <a href="#" class="inline-flex items-center justify-center px-6 py-3 border border-transparent text-base font-medium rounded-xl shadow-sm text-white bg-indigo-600 hover:bg-indigo-700 transition duration-150 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500">
                        Explore Our Services
                    </a>
                </div>
            </div>
        </div>
    </main>

    <!-- Footer -->
    <footer class="bg-gray-800 mt-12">
        <div class="max-w-7xl mx-auto py-8 px-4 sm:px-6 lg:px-8 text-center text-gray-400">
            &copy; 2025 CMORE Healthcare. All rights reserved.
        </div>
    </footer>

</body>
</html>
