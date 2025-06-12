<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Saarthak Kudiyal - Portfolio</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <!-- Font Awesome for social icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            -webkit-font-smoothing: antialiased;
            -moz-osx-font-smoothing: grayscale;
        }
        /* Custom class for the unique blob shape (optional, can be an SVG mask as well) */
        .blob-shape {
            /* This is a simplified circle, for a true blob more complex CSS or SVG would be needed */
            border-radius: 50% 50% 50% 50% / 60% 60% 40% 40%;
        }
    </style>
</head>
<body class="flex min-h-screen bg-gray-100 text-gray-800">

    <!-- Left Sidebar -->
    <aside class="w-64 bg-white flex flex-col p-8 shadow-lg z-10 flex-shrink-0">
        <div class="mb-10">
            <h1 class="text-2xl font-bold uppercase tracking-wider text-gray-900">PORTAL</h1>
        </div>
        <nav class="flex-grow">
            <ul class="space-y-4">
                <li><a href="#" class="block text-gray-700 hover:text-gray-900 font-medium transition duration-300">Home</a></li>
                <li><a href="#" class="block text-gray-700 hover:text-gray-900 font-medium transition duration-300">About</a></li>
                <!-- Portfolio Dropdown -->
                <li class="relative">
                    <button id="portfolio-dropdown-btn" class="flex items-center justify-between w-full text-left text-gray-700 hover:text-gray-900 font-medium transition duration-300 focus:outline-none">
                        <span>Portfolio</span>
                        <svg class="w-4 h-4 ml-2 transform rotate-0 transition-transform duration-300" id="dropdown-arrow" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7"></path>
                        </svg>
                    </button>
                    <div id="portfolio-dropdown-content" class="hidden absolute left-full top-0 ml-4 w-48 bg-white rounded-lg shadow-lg py-2 z-20 transition-all duration-300 ease-out origin-top-left scale-95 opacity-0">
                        <a href="https://drive.google.com/drive/folders/14iWDTLV-28TxzduObKtcng0zCyJuS3NV?usp=drive_link" class="block px-4 py-2 text-gray-700 hover:bg-gray-100 rounded-md transition duration-200" target="_blank">Assignments Folder</a>
                        <a href="https://drive.google.com/drive/folders/1bIQHXFesTAdOqbS_Rk5hFueO6Oad6_Pc?usp=drive_link" class="block px-4 py-2 text-gray-700 hover:bg-gray-100 rounded-md transition duration-200" target="_blank">Virtual Lib</a>
                        <a href="https://2417735.github.io/crypterror/" class="block px-4 py-2 text-gray-700 hover:bg-gray-100 rounded-md transition duration-200" target="_blank">Press Enter Project</a>
                        <a href="tutoring_conversation.html" class="block px-4 py-2 text-gray-700 hover:bg-gray-100 rounded-md transition duration-200" target="_blank">AI Tutor Conversation</a>
                        <!-- Hif Lumen button functionality kept in JS, but UI removed to match image -->
                        <!-- If you want Hif Lumen as a dropdown item, uncomment and modify below -->
                        <!-- <a href="#" id="hifLumenBtnDropdown" class="block px-4 py-2 text-gray-700 hover:bg-gray-100 rounded-md transition duration-200">🔒 Hif Lumen</a> -->
                    </div>
                </li>
                <li><a href="#" class="block text-gray-700 hover:text-gray-900 font-medium transition duration-300">Contact</a></li>
            </ul>
        </nav>
        <div class="mt-auto text-gray-500 text-sm">
            <p>&copy; 2021 Portal</p>
            <p>Created by Marketify</p>
            <!-- Original content for your site: -->
            <p class="mt-2">&copy; 2025 Saarthak Kudiyal</p>
            <p>Dong-A University</p>
        </div>
    </aside>

    <!-- Main Content Area -->
    <main class="flex-grow flex items-center justify-center p-8">
        <div class="text-center max-w-2xl px-4">
            <!-- Profile Picture -->
            <div class="relative w-48 h-48 mx-auto mb-8 rounded-full overflow-hidden bg-gray-300 flex items-center justify-center blob-shape border-4 border-gray-300">
                <img src="https://placehold.co/192x192/cccccc/333333?text=Profile" alt="Profile Picture" class="w-full h-full object-cover">
                <!-- For a more realistic blob shape, you'd typically use an SVG mask or a more complex clip-path property.
                     The 'blob-shape' class above is a simplified attempt at an organic, rounded form. -->
            </div>

            <!-- Name and Title -->
            <h2 class="text-4xl md:text-5xl font-extrabold uppercase tracking-wide mb-2 text-gray-900">SAARTHAK KUDIYAL</h2>
            <p class="text-lg md:text-xl text-gray-600 mb-8">Creative Photographer based in New York and happy to travel all over Europe to capture photos.</p>
            <!-- Replace with your actual details: -->
            <p class="text-lg md:text-xl text-gray-600 mb-8">Saarthak Kudiyal, Student at Dong-A University pursuing Integrated Business Management.</p>


            <!-- Social Media Icons -->
            <div class="flex justify-center space-x-6 text-gray-500 text-2xl mb-12">
                <a href="#" class="hover:text-gray-900 transition duration-300"><i class="fab fa-facebook-f"></i></a>
                <a href="#" class="hover:text-gray-900 transition duration-300"><i class="fab fa-twitter"></i></a>
                <a href="#" class="hover:text-gray-900 transition duration-300"><i class="fab fa-instagram"></i></a>
                <a href="#" class="hover:text-gray-900 transition duration-300"><i class="fab fa-dribbble"></i></a>
                <a href="#" class="hover:text-gray-900 transition duration-300"><i class="fab fa-tiktok"></i></a>
            </div>

            <!-- Dot element -->
            <div class="w-5 h-5 rounded-full border-2 border-gray-400 mx-auto"></div>
        </div>
    </main>

    <!-- Password Modal (kept for functionality, hidden by default) -->
    <div id="passwordModal" class="hidden fixed z-50 inset-0 overflow-y-auto bg-black bg-opacity-60 flex items-center justify-center">
        <div class="bg-white rounded-lg shadow-xl p-8 w-80 max-w-sm transform transition-all sm:my-8 sm:align-middle sm:max-w-lg sm:w-full">
            <h3 class="text-lg leading-6 font-medium text-gray-900 mb-4">Protected Link</h3>
            <p class="text-sm text-gray-500 mb-4">Please enter the passcode to access Hif Lumen</p>
            <input type="password" id="passwordInput" placeholder="Enter passcode" class="w-full px-3 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-blue-500 focus:border-blue-500 sm:text-sm">
            <div id="errorMessage" class="text-red-600 text-sm mt-2 hidden">Incorrect passcode. Please try again.</div>
            <div class="mt-5 sm:mt-6 flex justify-end space-x-3">
                <button type="button" id="cancelBtn" class="inline-flex justify-center rounded-md border border-gray-300 shadow-sm px-4 py-2 bg-white text-base font-medium text-gray-700 hover:bg-gray-50 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500 sm:text-sm">
                    Cancel
                </button>
                <button type="button" id="submitBtn" class="inline-flex justify-center rounded-md border border-transparent shadow-sm px-4 py-2 bg-blue-600 text-base font-medium text-white hover:bg-blue-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-blue-500 sm:text-sm">
                    Submit
                </button>
            </div>
        </div>
    </div>


    <script>
        // Dropdown functionality
        document.addEventListener('DOMContentLoaded', function() {
            const dropdownBtn = document.getElementById('portfolio-dropdown-btn');
            const dropdownContent = document.getElementById('portfolio-dropdown-content');
            const dropdownArrow = document.getElementById('dropdown-arrow');

            // Toggle dropdown visibility
            dropdownBtn.addEventListener('click', function(event) {
                event.stopPropagation(); // Prevent click from immediately closing it if body listener is present
                const isHidden = dropdownContent.classList.contains('hidden');
                if (isHidden) {
                    dropdownContent.classList.remove('hidden', 'opacity-0', 'scale-95');
                    dropdownContent.classList.add('opacity-100', 'scale-100');
                    dropdownArrow.classList.add('rotate-180');
                } else {
                    dropdownContent.classList.remove('opacity-100', 'scale-100');
                    dropdownContent.classList.add('opacity-0', 'scale-95');
                    dropdownArrow.classList.remove('rotate-180');
                    // Add hidden back after transition
                    setTimeout(() => {
                        dropdownContent.classList.add('hidden');
                    }, 300);
                }
            });

            // Close dropdown if clicked outside
            document.addEventListener('click', function(event) {
                if (!dropdownBtn.contains(event.target) && !dropdownContent.contains(event.target)) {
                    if (!dropdownContent.classList.contains('hidden')) {
                        dropdownContent.classList.remove('opacity-100', 'scale-100');
                        dropdownContent.classList.add('opacity-0', 'scale-95');
                        dropdownArrow.classList.remove('rotate-180');
                        setTimeout(() => {
                            dropdownContent.classList.add('hidden');
                        }, 300);
                    }
                }
            });

            // Original Grade Bar and Password Modal JavaScript (functionality retained, UI elements for grade bar removed)
            // Hif Lumen password protection
            const modal = document.getElementById('passwordModal');
            // const hifLumenBtn = document.getElementById('hifLumenBtn'); // This button is no longer directly in the main nav
            const hifLumenBtnDropdown = document.getElementById('hifLumenBtnDropdown'); // For future use if added to dropdown
            const cancelBtn = document.getElementById('cancelBtn');
            const submitBtn = document.getElementById('submitBtn');
            const passwordInput = document.getElementById('passwordInput');
            const errorMessage = document.getElementById('errorMessage');

            const correctPasscode = '1234';
            const protectedUrl = 'https://chatgpt.com/share/682c90ea-bcec-8001-a6ad-3ddf11eb3ddf';

            // Listener for Hif Lumen button (if it's in the dropdown)
            if (hifLumenBtnDropdown) {
                hifLumenBtnDropdown.addEventListener('click', function(e) {
                    e.preventDefault();
                    modal.classList.remove('hidden'); // Show modal
                    passwordInput.value = '';
                    errorMessage.classList.add('hidden');
                });
            }

            cancelBtn.addEventListener('click', function() {
                modal.classList.add('hidden'); // Hide modal
            });

            submitBtn.addEventListener('click', function() {
                checkPassword();
            });

            passwordInput.addEventListener('keyup', function(e) {
                if (e.key === 'Enter') checkPassword();
            });

            // Close modal if clicked outside of its content
            modal.addEventListener('click', function(e) {
                if (e.target === modal) {
                    modal.classList.add('hidden');
                }
            });

            function checkPassword() {
                if (passwordInput.value === correctPasscode) {
                    window.open(protectedUrl, '_blank');
                    modal.classList.add('hidden'); // Hide modal on success
                } else {
                    errorMessage.classList.remove('hidden');
                    passwordInput.value = '';
                    passwordInput.focus();
                }
            }
<script>
            // Grade fetch script (functionality retained, UI removed to match Tokyo design)
            fetch("https://script.google.com/macros/s/AKfycbygySpoqdNcUVNZ8TuFwMKGP6Ofu9axR382C13prSA/dev/ecex")
                .then(response => {
                    if (!response.ok) throw new Error('Network response was not ok');
                    return response.text();
                })
                .then(grade => {
                    // console.log("Fetched Grade:", grade); // For debugging: you can see the grade in console
                    // The element for grade display was removed to match the Tokyo.webp design.
                })
                .catch(error => {
                    console.error("Grade fetch failed:", error);
                    // The element for grade display was removed.
                });
        });
    </script>
</body>
</html>
