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
        .preso-body { font-family: 'Inter', sans-serif; }
        .preso-slide { display: none; width: 100%; max-width: 1024px; animation: preso-fadeIn 0.5s; }
        .preso-slide.active { display: flex; justify-content: center; align-items: center; }
        @keyframes preso-fadeIn { from { opacity: 0; } to { opacity: 1; } }
    </style>
</head>
<body class="preso-body bg-gray-100 flex items-center justify-center min-h-screen p-4">

    <div id="preso-container" style="display: flex; flex-direction: column; width: 100%; max-width: 64rem; max-height: 95vh; background-color: white; border-radius: 1rem; box-shadow: 0 25px 50px -12px rgba(0, 0, 0, 0.25); overflow: hidden;">
        
        <div id="preso-slides-wrapper" style="flex-grow: 1; min-height: 0; overflow-y: auto; display: flex; align-items: center; justify-content: center; padding: 2rem;">
            
            <div class="preso-slide active">
                <div class="text-center">
                    <h1 class="text-3xl md:text-5xl font-bold text-blue-900 mb-4">Data-Driven Resource Allocation</h1>
                    <p class="text-xl md:text-2xl text-blue-800 mb-8">Enhancing Campus Safety and Security at Trenton State</p>
                    <p class="text-lg text-gray-600">A Presentation for the Trenton State Executive Leadership Team</p>
                    <p class="text-lg text-gray-600 mt-8">By: Haim Cohen</p>
                </div>
            </div>

            <div class="preso-slide">
                <div class="text-center">
                    <h2 class="text-2xl md:text-3xl font-bold text-blue-900 mb-4">The Core Safety Challenge: Post-Pandemic Trends (2021-2023)</h2>
                    <p class="text-lg text-gray-700">An analysis of Clery Act crime statistics shows Trenton State's primary safety issues are not random violence, but internal and interpersonal offenses.</p>
                </div>
            </div>
            
            <div class="preso-slide">
                 <div class="text-center">
                    <h2 class="text-2xl md:text-3xl font-bold text-blue-900 mb-4">Summary & Strategic Impact</h2>
                    <p class="text-lg text-gray-700">This integrated strategy realigns our resources to address Trenton State's actual, data-defined needs.</p>
                </div>
            </div>
            
             </div>

        <div style="flex-shrink: 0; background-color: #1F2937; color: white; padding: 0.75rem; display: flex; align-items: center; justify-content: space-between;">
            <button id="preso-prevBtn" style="padding: 0.5rem 1rem; background-color: #2563EB; color: white; border-radius: 0.5rem; border: none; cursor: pointer;">Previous</button>
            <div id="preso-slide-counter" style="font-size: 0.875rem; font-weight: 500;"></div>
            <button id="preso-nextBtn" style="padding: 0.5rem 1rem; background-color: #2563EB; color: white; border-radius: 0.5rem; border: none; cursor: pointer;">Next</button>
        </div>
    </div>

    <script>
        const pres_container = document.getElementById('preso-container');
        if (pres_container) {
            const slides = pres_container.querySelectorAll('.preso-slide');
            const prevBtn = pres_container.querySelector('#preso-prevBtn');
            const nextBtn = pres_container.querySelector('#preso-nextBtn');
            const slideCounter = pres_container.querySelector('#preso-slide-counter');
            
            if (slides.length && prevBtn && nextBtn && slideCounter) {
                let currentSlide = 0;
                const enabledColor = '#2563EB';
                const disabledColor = '#6B7280';

                const showSlide = (n) => {
                    slides.forEach(slide => slide.classList.remove('active'));
                    slides[n].classList.add('active');
                    slideCounter.textContent = `Slide ${n + 1} of ${slides.length}`;
                    
                    prevBtn.disabled = (n === 0);
                    prevBtn.style.backgroundColor = (n === 0) ? disabledColor : enabledColor;
                    prevBtn.style.cursor = (n === 0) ? 'not-allowed' : 'pointer';

                    nextBtn.disabled = (n === slides.length - 1);
                    nextBtn.style.backgroundColor = (n === slides.length - 1) ? disabledColor : enabledColor;
                    nextBtn.style.cursor = (n === slides.length - 1) ? 'not-allowed' : 'pointer';
                };

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
        }
    </script>
</body>
</html>
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
                                <h3 class="font-semibold text-lg">Proposed Actions:</h3>
                                <ul class="list-disc list-inside ml-4">
                                    <li>Serve as primary liaison to Residential Education, Title IX Office, and student organizations.</li>
                                    <li>Develop and deliver targeted safety programming in residence halls.</li>
                                    <li>Organize community events to build positive, non-enforcement relationships.</li>
                                </ul>
                            </div>
                        </div>
                    </div>
                    <footer class="mt-auto pt-4 text-xs italic text-gray-500">
                        (California Community Colleges Chancellor's Office, 2022)
                    </footer>
                </div>
            </div>

            <div class="slide" data-slide="4">
                <div class="slide-content flex flex-col h-full">
                    <div>
                        <h2 class="text-2xl md:text-3xl font-bold text-blue-900 mb-2">Recommendation 2: Modernizing Safety with Technology</h2>
                        <p class="text-xl text-blue-800 mb-6">Invest in a unified, Trenton State-branded mobile safety application.</p>
                        <div class="space-y-4 text-gray-800">
                            <div>
                                <h3 class="font-semibold text-lg">Data-Driven Rationale:</h3>
                                <ul class="list-disc list-inside ml-4">
                                    <li>Meets the expectations of a tech-native student body.</li>
                                    <li>Provides a discreet and accessible tool for reporting sensitive crimes like stalking, which is a persistent issue according to campus data.</li>
                                </ul>
                            </div>
                            <div>
                                <h3 class="font-semibold text-lg">Proposed Core Features:</h3>
                                <ul class="list-disc list-inside ml-4">
                                    <li><strong class="font-medium">Mobile Blue Light:</strong> One-touch panic button sending location to dispatch.</li>
                                    <li><strong class="font-medium">Anonymous Tip Reporting:</strong> Confidential channel for reporting concerns.</li>
                                    <li><strong class="font-medium">Resource Hub:</strong> Direct-dial links to Title IX, counseling, etc.</li>
                                </ul>
                            </div>
                             <div>
                                <h3 class="font-semibold text-lg">Strategic Implication:</h3>
                                <p class="ml-4 text-gray-800">A mobile app significantly reduces the friction of reporting. Students are more likely to engage with an app than to make a formal phone call, especially for sensitive issues. The anonymity feature encourages more accurate reporting, providing a clearer picture of campus safety.</p>
                            </div>
                        </div>
                    </div>
                     <footer class="mt-auto pt-4 text-xs italic text-gray-500">
                        (Benson, 2025)
                    </footer>
                </div>
            </div>

            <div class="slide" data-slide="5">
                <div class="slide-content flex flex-col h-full">
                    <div>
                        <h2 class="text-2xl md:text-3xl font-bold text-blue-900 mb-4">Recommendations 3 & 4: Enhancing Officer Skills & Physical Security</h2>
                        <p class="text-lg text-gray-600 mb-6">A two-pronged approach to strengthen both our human and physical infrastructure.</p>
                        <div class="grid md:grid-cols-2 gap-8">
                            <div class="bg-blue-50 p-6 rounded-lg">
                                <h3 class="font-bold text-xl text-blue-800 mb-2">3. Mandate Advanced, Specialized Training</h3>
                                <div class="space-y-2">
                                    <p class="font-semibold">Rationale:</p>
                                    <ul class="list-disc list-inside ml-4 text-gray-800">
                                        <li>The prevalence of VAWA crimes requires skills beyond standard police training to ensure a trauma-informed response.</li>
                                        <li>De-escalation training directly addresses student concerns about use of force, showing a commitment to resolving situations with minimal physical intervention.</li>
                                    </ul>
                                </div>
                                <p class="mt-2"><strong class="font-semibold">Action:</strong> Allocate recurring budget for annual certification in <span class="font-bold">Trauma-Informed Response</span> and <span class="font-bold">Mental Health Crisis De-escalation</span> for all officers.</p>
                            </div>
                            <div class="bg-blue-50 p-6 rounded-lg">
                                <h3 class="font-bold text-xl text-blue-800 mb-2">4. Conduct a Comprehensive Physical Security Audit</h3>
                                <p><strong class="font-semibold">Rationale:</strong> Clery data shows an overwhelming concentration of offenses in and around on-campus residence halls.</p>
                                <p class="mt-2"><strong class="font-semibold">Action:</strong> Commission a professional audit of lighting and surveillance on pathways connecting residence halls.</p>
                            </div>
                        </div>
                    </div>
                    <footer class="mt-auto pt-4 text-xs italic text-gray-500">
                        (Goodall & Brodie, 2024; University of Bridgeport, 2025)
                    </footer>
                </div>
            </div>

            <div class="slide" data-slide="6">
                <div class="slide-content">
                    <h2 class="text-2xl md:text-3xl font-bold text-blue-900 mb-4">Summary & Strategic Impact</h2>
                    <p class="text-lg text-gray-700 mb-6">This integrated strategy realigns our resources to address Trenton State's actual, data-defined needs.</p>
                    <div class="grid md:grid-cols-2 gap-8">
                        <div>
                            <h3 class="font-bold text-xl text-blue-800 mb-2">The Five Pillars of a Safer Trenton State:</h3>
                            <ol class="list-decimal list-inside space-y-2 text-gray-800">
                                <li><strong>Community Resource Officer:</strong> To build trust and focus on prevention.</li>
                                <li><strong>Mobile Safety App:</strong> To modernize tools and lower reporting barriers.</li>
                                <li><strong>Specialized Training:</strong> To equip officers with critical response skills.</li>
                                <li><strong>Physical Security Audit:</strong> To harden our most vulnerable areas.</li>
                                <li><strong>Public Transparency:</strong> To build awareness and clarify safety procedures.</li>
                            </ol>
                        </div>
                        <div>
                            <h3 class="font-bold text-xl text-blue-800 mb-2">Expected Outcomes:</h3>
                            <ul class="list-disc list-inside space-y-2 text-gray-800">
                                <li>Increased community trust.</li>
                                <li>Improved reporting of sensitive crimes.</li>
                                <li>Enhanced prevention of interpersonal violence.</li>
                                <li>A safer physical environment.</li>
                                <li>Clear and accessible safety information for the community.</li>
                                <li>Positioning Trenton State as a leader in proactive campus safety.</li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>

            <div class="slide" data-slide="7">
                 <div class="slide-content">
                    <h2 class="text-2xl md:text-3xl font-bold text-blue-900 mb-4">References</h2>
                    <ul class="text-xs text-gray-700 space-y-3">
                        <li>
                            Benson, E. (2025, April 2). How mobile-integrated security technology is changing campus safety. *Campus Safety Magazine*. https://www.campussafetymagazine.com/insights/how-mobile-integrated-security-technology-is-changing-campus-safety/168563/
                        </li>
                        <li>
                            California Community Colleges Chancellor's Office. (2022). *A call to action: The California community colleges' task force report on reimagining campus policing*. https://www.cccco.edu/About-Us/News-and-Media/ccc-outlook-newsletter-archive/2022--campus-policing
                        </li>
                        <li>
                            The College of New Jersey. (2024). *The College's annual security and fire safety report 2024*. Campus Police Services. https://campuspolice.tcnj.edu/wp-content/uploads/sites/163/2024/09/M048-CP-Clery-Report_web-final.pdf
                        </li>
                        <li>
                            Goodall, K., & Brodie, R. (2024). Foundations of empathy and resilience: Integrating trauma-informed policing from recruit training onward. *Journal of Community Safety and Well-Being, 9*(1). https://journalcswb.ca/index.php/cswb/article/view/408
                        </li>
                        <li>
                            University of Bridgeport. (2025, February 20). *How colleges are enhancing campus safety measures in 2025*. https://www.bridgeport.edu/news/campus-safety-in-2025/
                        </li>
                    </ul>
                </div>
            </div>
        </div>

        <div class="bg-gray-800 text-white p-3 flex items-center justify-between">
            <button id="prevBtn" style="padding: 0.5rem 1rem; background-color: #2563EB; color: white; border-radius: 0.5rem; border: none; cursor: pointer;">Previous</button>
            <div id="slide-counter" class="text-sm font-medium">Slide 1 of 7</div>
            <button id="nextBtn" style="padding: 0.5rem 1rem; background-color: #2563EB; color: white; border-radius: 0.5rem; border: none; cursor: pointer;">Next</button>
        </div>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const slides = document.querySelectorAll('.slide');
            const prevBtn = document.getElementById('prevBtn');
            const nextBtn = document.getElementById('nextBtn');
            const slideCounter = document.getElementById('slide-counter');
            
            let currentSlide = 0;
            const totalSlides = slides.length;

            const enabledColor = '#2563EB'; // Original blue color
            const disabledColor = '#6B7280'; // Gray color for disabled state

            function showSlide(n) {
                slides.forEach(slide => slide.classList.remove('active'));
                slides[n].classList.add('active');
                slideCounter.textContent = `Slide ${n + 1} of ${totalSlides}`;
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
                if (n === totalSlides - 1) {
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
                if (currentSlide < totalSlides - 1) {
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
        });
    </script>
</body>
</html>