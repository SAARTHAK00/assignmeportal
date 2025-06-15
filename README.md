<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Saarthak Kudiyal - Portfolio</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts: Inter for a clean, modern look -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <!-- Font Awesome for social icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        /* Ensures the entire body uses the Inter font */
        body {
            font-family: 'Inter', sans-serif;
            -webkit-font-smoothing: antialiased; /* Smoother font rendering on WebKit browsers */
            -moz-osx-font-smoothing: grayscale; /* Smoother font rendering on Firefox */
        }
        /* Custom class for the unique blob shape (optional, can be an SVG mask as well) */
        .blob-shape {
            border-radius: 50% 50% 50% 50% / 60% 60% 40% 40%;
        }
        /* Adjusted body padding to account for fixed top bar */
        body {
            padding-top: 56px; /* Adjust this value to match the height of your top bar */
        }
        /* Responsive adjustments for smaller screens */
        @media (max-width: 768px) {
            .flex-container {
                flex-direction: column; /* Stack sidebar and main content vertically */
            }
            aside {
                width: 100%; /* Sidebar takes full width */
                height: auto; /* Allow sidebar height to adjust */
                padding-bottom: 20px; /* Add some padding at the bottom for smaller screens */
            }
            main {
                padding: 20px; /* Adjust main content padding */
            }
            /* Adjust dropdown position for mobile */
            #portfolio-dropdown-content {
                left: 0; /* Position dropdown under the button */
                margin-top: 10px; /* Space from the button */
                width: 100%; /* Make dropdown full width of sidebar */
                position: relative; /* Change position to relative within flow */
            }
            /* Adjust body padding for fixed top bar on small screens */
            body {
                padding-top: 56px; /* Ensure consistency */
            }
        }
    </style>
</head>
<body class="flex flex-col md:flex-row min-h-screen bg-gray-100 text-gray-800 flex-container">

    <!-- Top Grade Bar -->
    <div id="gradeBar" class="fixed top-0 left-0 w-full bg-blue-600 text-white p-3 flex items-center justify-center shadow-md z-50">
        <button id="checkGradeBtn" class="bg-blue-700 hover:bg-blue-800 text-white font-bold py-1 px-3 rounded-md shadow transition duration-200 ease-in-out focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-blue-500">
            Check My Grade
        </button>
        <span id="gradeDisplay" class="text-lg font-medium ml-4 hidden"></span>
        <!-- Optional: Loading spinner inside the bar -->
        <svg id="gradeLoadingSpinner" class="animate-spin -ml-1 mr-2 h-5 w-5 text-white hidden" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24">
            <circle class="opacity-25" cx="12" cy="12" r="10" stroke="currentColor" stroke-width="4"></circle>
            <path class="opacity-75" fill="currentColor" d="M4 12a8 8 0 018-8V0C5.373 0 0 5.373 0 12h4zm2 5.291A7.962 7.962 0 014 12H0c0 3.042 1.135 5.824 3 7.938l3-2.647z"></path>
        </svg>
    </div>

    <!-- Left Sidebar -->
    <aside class="w-full md:w-64 bg-white flex flex-col p-8 shadow-lg z-10 flex-shrink-0">
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
                    <!-- Dropdown content for Portfolio -->
                    <div id="portfolio-dropdown-content" class="hidden md:absolute md:left-full md:top-0 md:ml-4 w-48 bg-white rounded-lg shadow-lg py-2 z-20 transition-all duration-300 ease-out origin-top-left scale-95 opacity-0">
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

            <!-- "PORTAL" bar below the profile -->
            <div class="mb-8">
                <h1 class="text-2xl font-bold uppercase tracking-wider text-gray-900">PORTAL</h1>
            </div>

            <!-- Name and Title -->
            <h2 class="text-4xl md:text-5xl font-extrabold uppercase tracking-wide mb-2 text-gray-900">SAARTHAK KUDIYAL</h2>
            <p class="text-lg md:text-xl text-gray-600 mb-8">Student at Dong-A University pursuing Integrated Business Management.</p>

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

            // Hif Lumen password protection
            const modal = document.getElementById('passwordModal');
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

            // --- Grade Fetching for Top Bar ---
            const WEB_APP_URL = 'https://script.google.com/macros/s/AKfycbygySpoqdNcUVNZ8TuFwMKGP6Ofu9axR382C13prSA/dev';
            const CURRENT_STUDENT_NAME = 'Saarthak Kudiyal';

            const checkGradeBtn = document.getElementById('checkGradeBtn');
            const gradeDisplay = document.getElementById('gradeDisplay');
            const gradeLoadingSpinner = document.getElementById('gradeLoadingSpinner');

            // Event listener for the "Check My Grade" button
            checkGradeBtn.addEventListener('click', fetchGrade);

            async function fetchGrade() {
                // Hide button, show spinner and initial text
                checkGradeBtn.classList.add('hidden');
                gradeDisplay.classList.remove('hidden');
                gradeLoadingSpinner.classList.remove('hidden');
                gradeDisplay.textContent = 'Fetching your grade...';
                gradeDisplay.classList.remove('text-red-300', 'text-yellow-300'); // Clear any previous error/warning styling

                try {
                    const response = await fetch(WEB_APP_URL);
                    if (!response.ok) {
                        throw new Error(`HTTP error! status: ${response.status}`);
                    }
                    const data = await response.json();

                    gradeLoadingSpinner.classList.add('hidden'); // Hide spinner on completion

                    if (data.error) {
                        gradeDisplay.textContent = `Error: ${data.message}`;
                        gradeDisplay.classList.add('text-red-300');
                        console.error("Apps Script Error:", data.message);
                        return;
                    }

                    const studentData = data.find(row => row['Name'] === CURRENT_STUDENT_NAME);

                    if (studentData) {
                        const studentGrade = studentData['Grade'];
                        if (studentGrade !== undefined && studentGrade !== null && studentGrade !== '') {
                            gradeDisplay.textContent = `Your Total Grade: ${studentGrade}`;
                            // Example: if (studentGrade >= 90) gradeDisplay.classList.add('text-green-300');
                        } else {
                            gradeDisplay.textContent = `${CURRENT_STUDENT_NAME}'s grade not found or is empty.`;
                            gradeDisplay.classList.add('text-yellow-300');
                        }
                    } else {
                        gradeDisplay.textContent = `Grade for ${CURRENT_STUDENT_NAME} not found.`;
                        gradeDisplay.classList.add('text-red-300');
                    }
                } catch (error) {
                    gradeLoadingSpinner.classList.add('hidden'); // Ensure spinner is hidden on error
                    gradeDisplay.textContent = `Failed to load grade: ${error.message}`;
                    gradeDisplay.classList.add('text-red-300');
                    console.error("Grade fetch failed:", error);
                }
            }
        });
    </script>
</body>
</html>
