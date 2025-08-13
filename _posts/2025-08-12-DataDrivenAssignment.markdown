---
title: "Data-Driven Resource Allocation: Enhancing Campus Safety"
layout: post
date: 2025-08-12 11:55
image: /assets/images/markdown.jpg
headerImage: false
tag:
- ACE
category: blog
author: Chaim
description: An interactive presentation on enhancing campus safety at Trenton State.

---
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Trenton State Campus Safety Presentation</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
    <style>
        /* Base styles that are unlikely to conflict */
        .presentation-body {
            font-family: 'Inter', sans-serif;
        }
        .slide {
            display: none;
            width: 100%;
            max-width: 1024px;
            animation: fadeIn 0.5s;
        }
        .slide.active {
            display: flex;
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
    </style>
</head>
<body class="presentation-body bg-gray-100 flex items-center justify-center min-h-screen p-4">

    <div id="presentation-container" 
         style="display: flex; flex-direction: column; width: 100%; max-width: 64rem; max-height: 95vh; background-color: white; border-radius: 1rem; box-shadow: 0 25px 50px -12px rgba(0, 0, 0, 0.25); overflow: hidden;">
        
        <div id="slides-wrapper" 
             style="flex-grow: 1; min-height: 0; overflow-y: auto; display: flex; align-items: center; justify-content: center; padding: 2rem;">
            
            <div class="slide active" data-slide="1">
                <div class="text-center">
                    <h1 class="text-3xl md:text-5xl font-bold text-blue-900 mb-4">Data-Driven Resource Allocation</h1>
                    <p class="text-xl md:text-2xl text-blue-800 mb-8">Enhancing Campus Safety and Security at Trenton State</p>
                    <p class="text-lg text-gray-600">A Presentation for the Trenton State Executive Leadership Team</p>
                    <p class="text-lg text-gray-600 mt-8">By: Haim Cohen</p>
                </div>
            </div>

            <div class="slide" data-slide="2">
                <div class="flex flex-col h-full">
                    <div>
                        <h2 class="text-2xl md:text-3xl font-bold text-blue-900 mb-4">The Core Safety Challenge: Post-Pandemic Trends (2021-2023)</h2>
                        <p class="text-gray-700 mb-4 text-lg">An analysis of Clery Act crime statistics shows Trenton State's primary safety issues are not random violence, but internal and interpersonal offenses.</p>
                        <div class="grid md:grid-cols-2 gap-6">
                            <div>
                                 <ul class="list-disc list-inside space-y-2 text-gray-800">
                                    <li><strong class="font-semibold">Low Violent & Property Crime:</strong> Reports of robbery and aggravated assault remain at zero. Burglary incidents are minimal.</li>
                                    <li><strong class="font-semibold">High Interpersonal Offenses:</strong> The most persistent issues are VAWA offenses (rape, stalking, dating violence) and substance use violations, concentrated in on-campus residence halls.</li>
                                </ul>
                                <p class="mt-4 text-sm text-gray-600 italic"><strong>Implication:</strong> These offenses are not deterred by traditional police presence. Reducing them requires a fundamental shift in our security model toward one focused on changing campus culture through awareness, prevention, and education.</p>
                            </div>
                            <div class="bg-gray-50 p-4 rounded-lg">
                                <h3 class="font-semibold text-center mb-2 text-blue-800">On-Campus Crime Statistics (2021-2023)</h3>
                                <table class="w-full text-sm text-left text-gray-600">
                                    <thead class="text-xs text-gray-700 uppercase bg-gray-200">
                                        <tr><th class="px-4 py-2">Crime Category</th><th class="px-4 py-2 text-center">2021</th><th class="px-4 py-2 text-center">2022</th><th class="px-4 py-2 text-center">2023</th></tr>
                                    </thead>
                                    <tbody>
                                        <tr class="bg-white border-b"><td class="px-4 py-2 font-medium">Robbery / Agg. Assault</td><td class="px-4 py-2 text-center">0</td><td class="px-4 py-2 text-center">0</td><td class="px-4 py-2 text-center">0</td></tr>
                                        <tr class="bg-white border-b"><td class="px-4 py-2 font-medium">Burglary</td><td class="px-4 py-2 text-center">0</td><td class="px-4 py-2 text-center">0</td><td class="px-4 py-2 text-center">3</td></tr>
                                        <tr class="bg-red-50 border-b"><td class="px-4 py-2 font-medium text-red-900">Rape</td><td class="px-4 py-2 text-center text-red-900 font-bold">8</td><td class="px-4 py-2 text-center text-red-900 font-bold">5</td><td class="px-4 py-2 text-center text-red-900 font-bold">4</td></tr>
                                        <tr class="bg-red-50 border-b"><td class="px-4 py-2 font-medium text-red-900">Stalking</td><td class="px-4 py-2 text-center text-red-900 font-bold">7</td><td class="px-4 py-2 text-center text-red-900 font-bold">10</td><td class="px-4 py-2 text-center text-red-900 font-bold">4</td></tr>
                                        <tr class="bg-red-50 border-b"><td class="px-4 py-2 font-medium text-red-900">Dating Violence</td><td class="px-4 py-2 text-center text-red-900 font-bold">3</td><td class="px-4 py-2 text-center text-red-900 font-bold">3</td><td class="px-4 py-2 text-center text-red-900 font-bold">1</td></tr>
                                        <tr class="bg-yellow-50 border-b"><td class="px-4 py-2 font-medium text-yellow-900">Liquor Law Referrals</td><td class="px-4 py-2 text-center text-yellow-900 font-bold">215</td><td class="px-4 py-2 text-center text-yellow-900 font-bold">157</td><td class="px-4 py-2 text-center text-yellow-900 font-bold">107</td></tr>
                                        <tr class="bg-yellow-50"><td class="px-4 py-2 font-medium text-yellow-900">Drug Law Referrals</td><td class="px-4 py-2 text-center text-yellow-900 font-bold">45</td><td class="px-4 py-2 text-center text-yellow-900 font-bold">36</td><td class="px-4 py-2 text-center text-yellow-900 font-bold">27</td></tr>
                                    </tbody>
                                </table>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            </div>

        <div style="flex-shrink: 0; background-color: #1F2937; color: white; padding: 0.75rem; display: flex; align-items: center; justify-content: space-between;">
            <button id="prevBtn" style="padding: 0.5rem 1rem; background-color: #2563EB; color: white; border-radius: 0.5rem; border: none; cursor: pointer; transition: background-color 0.2s;">Previous</button>
            <div id="slide-counter" style="font-size: 0.875rem; font-weight: 500;">Slide 1 of 7</div>
            <button id="nextBtn" style="padding: 0.5rem 1rem; background-color: #2563EB; color: white; border-radius: 0.5rem; border: none; cursor: pointer; transition: background-color 0.2s;">Next</button>
        </div>
    </div>

    <script>
        // Get all the necessary DOM elements
        const slides = document.querySelectorAll('.slide');
        const prevBtn = document.getElementById('prevBtn');
        const nextBtn = document.getElementById('nextBtn');
        const slideCounter = document.getElementById('slide-counter');
        
        // This check ensures the script doesn't run if the elements are not found
        if (slides.length && prevBtn && nextBtn && slideCounter) {
            let currentSlide = 0;
            const totalSlides = slides.length; // For this example, I'll hardcode 7, but it would normally be dynamic
            
            const enabledColor = '#2563EB'; // Blue
            const disabledColor = '#6B7280'; // Gray

            function showSlide(n) {
                slides.forEach(slide => slide.classList.remove('active'));
                slides[n].classList.add('active');
                slideCounter.textContent = `Slide ${n + 1} of ${slides.length}`;
                updateButtonStates(n);
            }

            function updateButtonStates(n) {
                // Previous Button
                if (n === 0) {
                    prevBtn.disabled = true;
                    prevBtn.style.backgroundColor = disabledColor;
                    prevBtn.style.cursor = 'not-allowed';
                } else {
                    prevBtn.disabled = false;
                    prevBtn.style.backgroundColor = enabledColor;
                    prevBtn.style.cursor = 'pointer';
                }

                // Next Button
                if (n === slides.length - 1) {
                    nextBtn.disabled = true;
                    nextBtn.style.backgroundColor = disabledColor;
                    nextBtn.style.cursor = 'not-allowed';
                } else {
                    nextBtn.disabled = false;
                    nextBtn.style.backgroundColor = enabledColor;
                    nextBtn.style.cursor = 'pointer';
                }
            }

            nextBtn.addEventListener('click', () => {
                if (currentSlide < slides.length - 1) {
                    currentSlide++;
                    showSlide(currentSlide);
                }
            });

            prevBtn.addEventListener('click', () => {
                if (currentSlide > 0) {
                    currentSlide--;
                    showSlide(currentSlide);
                }
            });
            
            showSlide(currentSlide);
        }
    </script>
</body>
</html>