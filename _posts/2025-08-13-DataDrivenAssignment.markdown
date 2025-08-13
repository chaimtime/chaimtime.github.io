---
title: "Data-Driven Resource Allocation: Enhancing Campus Safety"
layout: post
date: 2025-08-13 11:55
author: Haim Cohen
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
        body {
            font-family: 'Inter', sans-serif;
        }
        .slide {
            display: none;
            animation: fadeIn 0.5s;
        }
        .slide.active {
            display: flex;
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        .slide-content {
            width: 100%;
            max-width: 1024px;
        }
    </style>
</head>
<body class="bg-gray-100 flex flex-col items-center justify-center min-h-screen p-4">

    <div id="presentation-container" class="w-full max-w-5xl bg-white rounded-2xl shadow-2xl flex flex-col overflow-hidden max-h-[95vh]">
        
        <div id="slides-wrapper" class="flex-grow flex items-center justify-center p-8 md:p-12 overflow-y-auto min-h-0">
            
            <div class="slide active" data-slide="1">
                <div class="slide-content text-center">
                    <h1 class="text-3xl md:text-5xl font-bold text-blue-900 mb-4">Data-Driven Resource Allocation</h1>
                    <p class="text-xl md:text-2xl text-blue-800 mb-8">Enhancing Campus Safety and Security at Trenton State</p>
                    <p class="text-lg text-gray-600">A Presentation for the Trenton State Executive Leadership Team</p>
                    <p class="text-lg text-gray-600 mt-8">By: Haim Cohen</p>
                </div>
            </div>

            <div class="slide" data-slide="2">
                <div class="slide-content flex flex-col h-full">
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
                    <footer class="mt-auto pt-4 text-xs italic text-gray-500">
                        (The College of New Jersey, 2024)
                    </footer>
                </div>
            </div>

            <div class="slide" data-slide="3">
                <div class="slide-content flex flex-col h-full">
                    <div>
                        <h2 class="text-2xl md:text-3xl font-bold text-blue-900 mb-2">Recommendation 1: Proactive Community Engagement</h2>
                        <p class="text-xl text-blue-800 mb-6">Reallocate one patrol officer position to establish a dedicated Community Resource Officer (CRO).</p>
                        <div class="space-y-4 text-gray-800">
                            <div>
                                <h3 class="font-semibold text-lg">Data-Driven Rationale:</h3>
                                <ul class="list-disc list-inside ml-4">
                                    <li>Creates a focused role for the proactive prevention of VAWA offenses (rape, stalking), which are the most significant safety issues identified in our data.</li>
                                    <li>Shifts from a reactive enforcement model to a proactive, relationship-based philosophy to better address interpersonal crime.</li>
                                </ul>
                            </div>
                            <div>
                                <h