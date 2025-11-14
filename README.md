<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Star Explorer - Storybook Website</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&family=Playfair+Display:ital,wght@0,400..900;1,400..900&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary-color: #fca5a5; /* Rose-300 */
            --secondary-color: #9333ea; /* Violet-700 */
            --bg-color: #f7f3e8; /* Off-White/Cream */
            --text-color: #1e293b; /* Slate-800 */
        }
        body {
            font-family: 'Inter', sans-serif;
            background-color: var(--bg-color);
            color: var(--text-color);
            scroll-behavior: smooth;
        }
        .title-font {
            font-family: 'Playfair Display', serif;
        }
    </style>
</head>
<body>

    <!-- Scroll function -->
    <script>
        function scrollToSection(id) {
            const element = document.getElementById(id);
            if (element) {
                element.scrollIntoView({ behavior: 'smooth' });
            }
        }
    </script>

    <!-- Header / Navigation -->
    <header class="sticky top-0 z-10 bg-white/90 backdrop-blur-sm shadow-md">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-4 flex justify-between items-center">
            <h1 class="title-font text-2xl font-bold text-secondary-color">
                The Star Explorer
            </h1>
            <nav>
                <button 
                    onclick="scrollToSection('story-content')" 
                    class="px-4 py-2 bg-secondary-color text-white text-sm font-semibold rounded-full hover:bg-violet-800 transition shadow-lg"
                >
                    Read Now
                </button>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section id="hero" class="pt-16 pb-24 px-4 sm:px-6 lg:px-8">
        <div class="max-w-6xl mx-auto flex flex-col md:flex-row items-center gap-12">
            <!-- Text Content -->
            <div class="md:w-1/2 text-center md:text-left">
                <p class="text-xl text-primary-color font-semibold mb-4">A Tale of Adventure and Wonder</p>
                <h2 class="title-font text-5xl sm:text-6xl font-extrabold leading-tight mb-6 text-gray-900">
                    Find the Light. Find Home.
                </h2>
                <p class="text-lg text-gray-600 mb-8 max-w-lg mx-auto md:mx-0">
                    Join young Leo, the little astronaut, as he pilots his tiny spaceship, "The Comet," across nebulas and past sleeping planets in search of the brightest star he's ever seen.
                </p>
                <button 
                    onclick="scrollToSection('story-content')" 
                    class="px-8 py-3 bg-primary-color text-white text-lg font-bold rounded-xl hover:bg-rose-400 transition transform hover:scale-105 shadow-xl"
                >
                    Start the Adventure
                </button>
            </div>

            <!-- Image/Visual -->
            <div class="md:w-1/2 w-full mt-10 md:mt-0">
                <img 
                    src="https://placehold.co/600x400/9333ea/ffffff/png?text=Leo+The+Star+Explorer" 
                    alt="Illustration of a small astronaut floating in space" 
                    class="w-full h-auto object-cover rounded-[30px] shadow-2xl border-4 border-white"
                    onerror="this.onerror=null; this.src='https://placehold.co/600x400/8B5CF6/ffffff/png?text=Storybook+Cover';"
                >
            </div>
        </div>
    </section>

    <!-- Story Content / Chapters -->
    <section id="story-content" class="bg-white py-20 px-4 sm:px-6 lg:px-8 rounded-t-[50px] shadow-inner">
        <div class="max-w-4xl mx-auto">
            <h3 class="title-font text-4xl font-bold text-center mb-16 text-secondary-color">
                The Chapters of The Comet
            </h3>

            <!-- Chapter 1 -->
            <article class="mb-16 p-8 border-l-4 border-primary-color bg-gray-50 rounded-lg shadow-md hover:shadow-xl transition-shadow duration-300">
                <p class="text-sm font-semibold text-primary-color uppercase mb-1">Chapter I</p>
                <h4 class="title-font text-2xl font-semibold text-gray-900 mb-4">The Launch from Lavender Moon</h4>
                <p class="text-gray-700 leading-relaxed">
                    Leo packed his last granola bar and waved goodbye to his pet space-squirrel, Zippy. The controls of The Comet glowed softly. It was time. He tightened his helmet and, with a silent countdown, blasted off the dusty plains of Lavender Moon, leaving a shimmering trail behind him. His mission: to find the legendary Wishing Star, said to be made of pure happiness.
                </p>
            </article>

            <!-- Chapter 2 -->
            <article class="mb-16 p-8 border-l-4 border-violet-500 bg-gray-50 rounded-lg shadow-md hover:shadow-xl transition-shadow duration-300">
                <p class="text-sm font-semibold text-violet-500 uppercase mb-1">Chapter II</p>
                <h4 class="title-font text-2xl font-semibold text-gray-900 mb-4">The Whispering Nebula</h4>
                <p class="text-gray-700 leading-relaxed">
                    The Nebula was a swirl of pinks and blues, but it was eerily quiet. Leo could hear whispers on the ship's comms—ancient stories carried on solar winds. He had to navigate carefully, avoiding the sleepy space whales and following the faint echo of a celestial chime, which he hoped was the Wishing Star's song.
                </p>
            </article>

            <!-- Chapter 3 -->
            <article class="mb-16 p-8 border-l-4 border-primary-color bg-gray-50 rounded-lg shadow-md hover:shadow-xl transition-shadow duration-300">
                <p class="text-sm font-semibold text-primary-color uppercase mb-1">Chapter III</p>
                <h4 class="title-font text-2xl font-semibold text-gray-900 mb-4">The Planet of Giant Daisies</h4>
                <p class="text-gray-700 leading-relaxed">
                    A detour! He landed on a planet where the flowers were taller than his ship. Giant daisies, striped with every color imaginable, swayed gently in the low gravity. He met a family of gentle, green-skinned creatures who taught him how to make space jam from moonberries. It was a wonderful break, but the Wishing Star still called him forward.
                </p>
            </article>
            
            <!-- Call to Action for the rest of the book -->
            <div class="text-center mt-12 p-8 bg-secondary-color rounded-xl shadow-2xl text-white">
                <p class="title-font text-3xl font-bold mb-4">Want to finish Leo's journey?</p>
                <p class="text-lg mb-6">
                    Read the final chapters to discover the Wishing Star's secret and see if Leo makes it home to Zippy!
                </p>
                <!-- Placeholder for purchase/download link -->
                <a href="#" class="inline-block px-8 py-3 bg-white text-secondary-color font-bold rounded-full hover:bg-gray-200 transition transform hover:scale-105 shadow-lg">
                    Get the Full Story
                </a>
            </div>

        </div>
    </section>
    
    <!-- Video Trailer / Interactive Content (New Section with Iframe) -->
    <section id="video-trailer" class="py-20 px-4 sm:px-6 lg:px-8">
        <div class="max-w-4xl mx-auto">
            <h3 class="title-font text-4xl font-bold text-center mb-10 text-gray-900">
                Watch the Official Trailer
            </h3>
            
            <!-- Iframe Container for 16:9 aspect ratio (56.25% padding-top is 9/16) -->
            <div class="relative overflow-hidden w-full rounded-xl shadow-2xl" style="padding-top: 56.25%;">
                <!-- The iframe is absolutely positioned to cover the container and achieve responsiveness -->
                <iframe 
                    src="https://www.youtube.com/embed/g6j8sPz7334" 
                    title="Storybook Trailer Placeholder" 
                    frameborder="0" 
                    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
                    allowfullscreen
                    class="absolute top-0 left-0 w-full h-full border-4 border-secondary-color rounded-xl"
                ></iframe>
<iframe 
                    src="https://gemini.google.com/share/9fdecb4b86be" 
                    title="Storybook Trailer Placeholder" 
                    frameborder="0" 
                    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
                    allowfullscreen
                    class="absolute top-0 left-0 w-full h-full border-4 border-secondary-color rounded-xl"
                ></iframe>
            </div>

            <p class="text-center text-gray-600 mt-6 italic text-sm">
                A preview of Leo's cosmic journey. (The `iframe` is the element above, loading a mock YouTube video.)
            </p>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-800 text-white py-10">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <p class="text-sm text-gray-400 mb-2">&copy; 2025 The Star Explorer. All Rights Reserved.</p>
            <p class="text-xs text-gray-500">Website design inspired by cosmic wonder and interstellar dreams.</p>
        </div>
    </footer>

</body>
</html>

