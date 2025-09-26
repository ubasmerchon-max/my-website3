<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Apology Letter</title>
    <script src="https://cdn.tailwindcss.com"></script> <!-- Tailwind CDN for easy styling -->
    <style>
        /* Custom envelope flap animation */
        .envelope-flap { transition: transform 0.3s ease; }
        .letter-hidden { display: none; }
        .letter-visible { display: block; animation: fadeIn 0.5s ease-in; }
        @keyframes fadeIn { from { opacity: 0; transform: translateY(20px); } to { opacity: 1; transform: translateY(0); } }
    </style>
</head>
<body class="min-h-screen bg-gradient-to-br from-blue-50 to-purple-50 flex items-center justify-center p-4">
    <div class="w-full max-w-md">
        <!-- Envelope View -->
        <div id="envelope" class="relative">
            <div class="bg-red-100 p-6 rounded-lg shadow-lg border-2 border-red-200 transform -rotate-2">
                <div class="text-center mb-4">
                    <div class="w-16 h-16 mx-auto mb-2 flex items-center justify-center">
                        <img 
                            src="https://placeholder-image-service.onrender.com/image/64x64?prompt=A sad cartoon envelope with teardrop and heart&id=85308696-c0e7-4ede-ad34-1103d6a85e1d" 
                            alt="Sad envelope with teardrop and heart" 
                            class="w-full h-full object-contain"
                        />
                    </div>
                    <h2 class="text-xl font-bold text-red-800">An Apology Awaits</h2>
                    <p class="text-red-600 mt-1">Click to open</p>
                </div>
                
                <div class="absolute top-0 right-0 w-0 h-0 border-l-[20px] border-l-transparent border-t-[20px] border-t-red-300 border-r-[20px] border-r-transparent"></div>
                
                <button
                    onclick="openLetter()"
                    class="w-full bg-red-500 hover:bg-red-600 text-white font-semibold py-3 px-4 rounded-md transition-colors duration-200 flex items-center justify-center"
                >
                    <span>Open Letter</span>
                    <span class="ml-2">
                        <img 
                            src="https://placeholder-image-service.onrender.com/image/24x24?prompt=Tiny heart breaking in half&id=92348696-c0e7-4ede-ad34-1103d6a85e1d" 
                            alt="Heart breaking in half" 
                            class="inline-block"
                        />
                    </span>
                </button>
            </div>
            
            <!-- Envelope flap -->
            <div class="absolute top-0 left-1/2 transform -translate-x-1/2 w-11/12">
                <div class="w-full h-8 bg-red-200 rounded-t-lg"></div>
                <div class="w-0 h-0 border-l-[160px] border-l-transparent border-b-[30px] border-b-red-200 border-r-[160px] border-r-transparent mx-auto"></div>
            </div>
        </div>

        <!-- Letter View (Hidden Initially) -->
        <div id="letter" class="letter-hidden">
            <div class="bg-amber-50 p-8 rounded-lg shadow-lg border-2 border-amber-200 transform rotate-0 transition-transform duration-500">
                <div class="text-center mb-6">
                    <h1 class="text-2xl font-bold text-amber-900 mb-2">I'm Sorry</h1>
                    <div class="flex justify-center space-x-2 mb-4">
                        <div class="w-10 h-10">
                            <img 
                                src="https://placeholder-image-service.onrender.com/image/40x40?prompt=Cartoon sad cat with teardrop eyes&id=76348696-c0e7-4ede-ad34-1103d6a85e1d" 
                                alt="Cartoon sad cat with teardrop eyes" 
                                class="w-full h-full object-contain"
                            />
                        </div>
                        <div class="w-10 h-10">
                            <img 
                                src="https://placeholder-image-service.onrender.com/image/40x40?prompt=Broken heart with crack lines&id=66348696-c0e7-4ede-ad34-1103d6a85e1d" 
                                alt="Broken heart with crack lines" 
                                class="w-full h-full object-contain"
                            />
                        </div>
                        <div class="w-10 h-10">
                            <img 
                                src="https://placeholder-image-service.onrender.com/image/40x40?prompt=Sad cat looking apologetic with big eyes&id=56348696-c0e7-4ede-ad34-1103d6a85e1d" 
                                alt="Sad cat looking apologetic with big eyes" 
                                class="w-full h-full object-contain"
                            />
                        </div>
                    </div>
                </div>
                
                <div class="space-y-4 text-amber-800">
                    <p class="leading-relaxed">
                        I'm writing this letter Lens to sincerely apologize for my actions. I realize that was wrong, and I deeply regret any pain or inconvenience I may have caused you😢.
                    </p>
                    
                    <p class="leading-relaxed">
                        My behavior was thoughtless and unacceptable. I should have considered your feelings more carefully and acted with more respect and understanding Lens😢.
                    </p>
                    
                    <p class="leading-relaxed">
                        Please know that I am truly sorry, and I'm committed to making things right. I value our relationship greatly and hope you can find it in your heart to forgive me😢. I have a trust in you Lens sorry for everything I did to you, sorry Lens and I Love you😢
                    </p>
                </div>
                
                <div class="mt-6 flex justify-center">
                    <div class="w-12 h-12">
                        <img 
                            src="https://placeholder-image-service.onrender.com/image/48x48?prompt=Flower wilting with a sad face&id=46348696-c0e7-4ede-ad34-1103d6a85e1d" 
                            alt="Flower wilting with a sad face" 
                            class="w-full h-full object-contain"
                        />
                    </div>
                </div>
            </div>
        </div>
    </div>

    <script>
        function openLetter() {
            document.getElementById('envelope').style.display = 'none';
            document.getElementById('letter').classList.remove('letter-hidden');
            document.getElementById('letter').classList.add('letter-visible');
        }
    </script>
</body>
</html>
