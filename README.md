<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>NexusCart - Your Online Shopping Destination</title>
    
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Google Fonts: Inter -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">
    
    <!-- Feather Icons -->
    <script src="https://unpkg.com/feather-icons"></script>

    <style>
        /* Custom styles to complement Tailwind */
        body {
            font-family: 'Inter', sans-serif;
            background-color: #0d1117; /* A deep, dark background */
            color: #c9d1d9;
        }
        .glassmorphism {
            background: rgba(13, 17, 23, 0.6);
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        .gradient-text {
            background: linear-gradient(90deg, #38bdf8, #818cf8);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        .hero-gradient-bg {
             background: radial-gradient(circle at top, rgba(56, 189, 248, 0.1), transparent 40%);
        }
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #0d1117;
        }
        ::-webkit-scrollbar-thumb {
            background-color: #1f2937;
            border-radius: 10px;
            border: 2px solid #0d1117;
        }
        ::-webkit-scrollbar-thumb:hover {
            background-color: #374151;
        }
    </style>
</head>
<body class="antialiased">

    <!-- Header Section -->
    <header id="header" class="glassmorphism sticky top-0 z-50 transition-all duration-300">
        <div class="container mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex items-center justify-between h-20">
                <!-- Logo -->
                <div class="flex-shrink-0">
                    <a href="#" class="flex items-center space-x-2">
                        <svg class="h-8 w-8 text-sky-400" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                            <path d="M12 2L2 7l10 5 10-5-10-5z"></path>
                            <path d="M2 17l10 5 10-5"></path>
                            <path d="M2 12l10 5 10-5"></path>
                        </svg>
                        <span class="text-2xl font-bold text-white">NexusCart</span>
                    </a>
                </div>

                <!-- Desktop Navigation -->
                <nav class="hidden md:flex md:items-center md:space-x-8">
                    <a href="#home" class="text-gray-300 hover:text-sky-400 transition-colors duration-300">Home</a>
                    <a href="#shop" class="text-gray-300 hover:text-sky-400 transition-colors duration-300">Shop</a>
                    <a href="#" class="text-gray-300 hover:text-sky-400 transition-colors duration-300">Deals</a>
                    <a href="#" class="text-gray-300 hover:text-sky-400 transition-colors duration-300">About</a>
                </nav>

                <!-- Search and Icons -->
                <div class="flex items-center space-x-4">
                     <div class="hidden lg:block relative">
                        <input type="text" placeholder="Search products..." class="w-64 bg-gray-800 border border-gray-700 rounded-full py-2 pl-10 pr-4 text-white focus:outline-none focus:ring-2 focus:ring-sky-500 transition-all">
                        <div class="absolute inset-y-0 left-0 pl-3 flex items-center pointer-events-none">
                            <i data-feather="search" class="h-5 w-5 text-gray-400"></i>
                        </div>
                    </div>
                    <a href="#" class="text-gray-300 hover:text-sky-400 transition-colors duration-300"><i data-feather="heart"></i></a>
                    <a href="#" class="relative text-gray-300 hover:text-sky-400 transition-colors duration-300">
                        <i data-feather="shopping-cart"></i>
                        <span class="absolute -top-2 -right-2 bg-sky-500 text-white text-xs rounded-full h-5 w-5 flex items-center justify-center">3</span>
                    </a>
                    <button id="mobile-menu-button" class="md:hidden p-2 rounded-md text-gray-300 hover:text-white hover:bg-gray-700">
                        <i data-feather="menu"></i>
                    </button>
                </div>
            </div>
        </div>
        <!-- Mobile Menu -->
        <div id="mobile-menu" class="hidden md:hidden">
            <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3">
                <a href="#home" class="block px-3 py-2 rounded-md text-base font-medium text-gray-300 hover:text-white hover:bg-gray-700">Home</a>
                <a href="#shop" class="block px-3 py-2 rounded-md text-base font-medium text-gray-300 hover:text-white hover:bg-gray-700">Shop</a>
                <a href="#" class="block px-3 py-2 rounded-md text-base font-medium text-gray-300 hover:text-white hover:bg-gray-700">Deals</a>
                <a href="#" class="block px-3 py-2 rounded-md text-base font-medium text-gray-300 hover:text-white hover:bg-gray-700">About</a>
            </div>
        </div>
    </header>
    
    <main>
        <!-- Hero Section -->
        <section id="home" class="relative py-20 md:py-32 hero-gradient-bg">
            <div class="container mx-auto px-4 sm:px-6 lg:px-8 text-center">
                <h1 class="text-4xl md:text-6xl font-extrabold text-white leading-tight mb-4">
                    Discover a New Era of<br><span class="gradient-text">Online Shopping</span>
                </h1>
                <p class="text-lg md:text-xl text-gray-400 max-w-3xl mx-auto mb-8">
                    Explore curated collections of the finest products, delivered with exceptional service. Your next favorite thing is just a click away.
                </p>
                <a href="#shop" class="bg-sky-500 hover:bg-sky-600 text-white font-bold py-3 px-8 rounded-full text-lg transition-all duration-300 transform hover:scale-105 shadow-lg shadow-sky-500/20">
                    Start Exploring
                </a>
            </div>
        </section>

        <!-- Main Shopping Section -->
        <section id="shop" class="py-24">
            <div class="container mx-auto px-4 sm:px-6 lg:px-8">
                <div class="flex flex-col md:flex-row gap-12">
                    
                    <!-- Filters Sidebar -->
                    <aside class="w-full md:w-1/4 lg:w-1/5">
                        <div class="glassmorphism p-6 rounded-2xl sticky top-28">
                            <h3 class="text-xl font-bold text-white mb-6">Filters</h3>
                            
                            <!-- Category Filter -->
                            <div class="mb-6">
                                <h4 class="font-semibold text-gray-300 mb-3">Category</h4>
                                <div class="space-y-2">
                                    <a href="#" class="block text-gray-400 hover:text-sky-400">Electronics</a>
                                    <a href="#" class="block text-gray-400 hover:text-sky-400">Fashion</a>
                                    <a href="#" class="block text-gray-400 hover:text-sky-400">Home & Garden</a>
                                    <a href="#" class="block text-gray-400 hover:text-sky-400">Books</a>
                                    <a href="#" class="block text-gray-400 hover:text-sky-400">Sports</a>
                                </div>
                            </div>

                            <!-- Price Range Filter -->
                            <div class="mb-6">
                                <h4 class="font-semibold text-gray-300 mb-3">Price Range</h4>
                                <input type="range" min="0" max="1000" value="500" class="w-full h-2 bg-gray-700 rounded-lg appearance-none cursor-pointer">
                                <div class="flex justify-between text-sm text-gray-400 mt-2">
                                    <span>$0</span>
                                    <span>$1000+</span>
                                </div>
                            </div>

                            <!-- Rating Filter -->
                            <div>
                                <h4 class="font-semibold text-gray-300 mb-3">Rating</h4>
                                <div class="space-y-2">
                                    <label class="flex items-center text-gray-400 hover:text-sky-400 cursor-pointer">
                                        <input type="radio" name="rating" class="form-radio h-4 w-4 text-sky-500 bg-gray-800 border-gray-600 focus:ring-sky-500">
                                        <span class="ml-2">4 Stars & Up</span>
                                    </label>
                                    <label class="flex items-center text-gray-400 hover:text-sky-400 cursor-pointer">
                                        <input type="radio" name="rating" class="form-radio h-4 w-4 text-sky-500 bg-gray-800 border-gray-600 focus:ring-sky-500">
                                        <span class="ml-2">3 Stars & Up</span>
                                    </label>
                                    <label class="flex items-center text-gray-400 hover:text-sky-400 cursor-pointer">
                                        <input type="radio" name="rating" class="form-radio h-4 w-4 text-sky-500 bg-gray-800 border-gray-600 focus:ring-sky-500">
                                        <span class="ml-2">2 Stars & Up</span>
                                    </label>
                                </div>
                            </div>
                        </div>
                    </aside>

                    <!-- Product Grid -->
                    <div class="w-full md:w-3/4 lg:w-4/5">
                        <h2 class="text-3xl font-bold text-white mb-8">All Products</h2>
                        <div id="product-grid" class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 gap-8">
                            <!-- Products will be injected here by JavaScript -->
                        </div>
                    </div>
                </div>
            </div>
        </section>

    </main>

    <!-- Footer -->
    <footer class="bg-gray-900 border-t border-gray-800">
        <div class="container mx-auto px-4 sm:px-6 lg:px-8 py-12">
            <div class="grid grid-cols-2 md:grid-cols-4 lg:grid-cols-5 gap-8">
                <div class="col-span-2 md:col-span-4 lg:col-span-1">
                     <a href="#" class="flex items-center space-x-2">
                        <svg class="h-8 w-8 text-sky-400" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                            <path d="M12 2L2 7l10 5 10-5-10-5z"></path>
                            <path d="M2 17l10 5 10-5"></path>
                            <path d="M2 12l10 5 10-5"></path>
                        </svg>
                        <span class="text-2xl font-bold text-white">NexusCart</span>
                    </a>
                    <p class="text-gray-400 mt-4">The future of online retail.</p>
                </div>
                <div>
                    <h5 class="font-semibold text-white tracking-wider uppercase">Shop</h5>
                    <ul class="mt-4 space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-sky-400">Electronics</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-sky-400">Fashion</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-sky-400">Home</a></li>
                    </ul>
                </div>
                <div>
                    <h5 class="font-semibold text-white tracking-wider uppercase">About</h5>
                    <ul class="mt-4 space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-sky-400">Our Story</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-sky-400">Careers</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-sky-400">Press</a></li>
                    </ul>
                </div>
                <div>
                    <h5 class="font-semibold text-white tracking-wider uppercase">Support</h5>
                    <ul class="mt-4 space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-sky-400">Contact Us</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-sky-400">FAQ</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-sky-400">Shipping</a></li>
                    </ul>
                </div>
                 <div>
                    <h5 class="font-semibold text-white tracking-wider uppercase">Legal</h5>
                    <ul class="mt-4 space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-sky-400">Terms of Service</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-sky-400">Privacy Policy</a></li>
                    </ul>
                </div>
            </div>
            <div class="mt-8 pt-8 border-t border-gray-800 flex flex-col md:flex-row justify-between items-center">
                <p class="text-gray-500">&copy; 2024 NexusCart. All rights reserved.</p>
                <div class="flex space-x-6 mt-4 md:mt-0">
                    <a href="#" class="text-gray-500 hover:text-sky-400"><i data-feather="twitter"></i></a>
                    <a href="#" class="text-gray-500 hover:text-sky-400"><i data-feather="instagram"></i></a>
                    <a href="#" class="text-gray-500 hover:text-sky-400"><i data-feather="facebook"></i></a>
                </div>
            </div>
        </div>
    </footer>

    <!-- Product Modal -->
    <div id="product-modal" class="fixed inset-0 bg-black bg-opacity-70 backdrop-blur-sm z-50 flex items-center justify-center p-4 hidden">
        <div id="modal-content" class="glassmorphism w-full max-w-4xl max-h-[90vh] rounded-2xl shadow-2xl flex flex-col md:flex-row relative transform scale-95 transition-transform duration-300">
             <!-- Close button for the modal -->
            <button id="close-modal" class="absolute top-4 right-4 text-gray-400 hover:text-white z-10">
                <i data-feather="x" class="h-8 w-8"></i>
            </button>
            <!-- Modal Content will be injected here -->
        </div>
    </div>


    <script>
        document.addEventListener('DOMContentLoaded', function() {
            // Feather Icons
            feather.replace();

            // Mobile menu toggle
            const mobileMenuButton = document.getElementById('mobile-menu-button');
            const mobileMenu = document.getElementById('mobile-menu');
            mobileMenuButton.addEventListener('click', () => {
                mobileMenu.classList.toggle('hidden');
            });
            
            // Header scroll effect
            const header = document.getElementById('header');
            window.addEventListener('scroll', () => {
                if (window.scrollY > 50) {
                    header.classList.add('bg-opacity-80');
                } else {
                    header.classList.remove('bg-opacity-80');
                }
            });

            // Mock Product Data
            const products = [
                { id: 1, name: 'Wireless Noise-Cancelling Headphones', price: 249.99, rating: 4.8, category: 'Electronics', image: 'https://placehold.co/600x600/1e293b/ffffff?text=Headphones' },
                { id: 2, name: 'Smartwatch Series 8', price: 399.00, rating: 4.9, category: 'Electronics', image: 'https://placehold.co/600x600/374151/ffffff?text=Watch' },
                { id: 3, name: 'Organic Cotton Hoodie', price: 79.50, rating: 4.6, category: 'Fashion', image: 'https://placehold.co/600x600/111827/ffffff?text=Hoodie' },
                { id: 4, name: '4K Action Camera', price: 199.99, rating: 4.7, category: 'Electronics', image: 'https://placehold.co/600x600/4b5563/ffffff?text=Camera' },
                { id: 5, name: 'Minimalist Leather Backpack', price: 129.00, rating: 4.8, category: 'Fashion', image: 'https://placehold.co/600x600/1f2937/ffffff?text=Backpack' },
                { id: 6, name: 'Smart Home Hub', price: 99.00, rating: 4.5, category: 'Home & Garden', image: 'https://placehold.co/600x600/334155/ffffff?text=Hub' },
                { id: 7, name: 'Professional Gaming Mouse', price: 69.99, rating: 4.9, category: 'Electronics', image: 'https://placehold.co/600x600/52525b/ffffff?text=Mouse' },
                { id: 8, name: 'Insulated Travel Mug', price: 25.00, rating: 4.7, category: 'Home & Garden', image: 'https://placehold.co/600x600/0f172a/ffffff?text=Mug' },
            ];

            const productGrid = document.getElementById('product-grid');
            const productModal = document.getElementById('product-modal');
            const modalContent = document.getElementById('modal-content');
            const closeModalButton = document.getElementById('close-modal');

            // Function to render products
            function renderProducts(productsToRender) {
                productGrid.innerHTML = ''; // Clear existing products
                productsToRender.forEach(product => {
                    const productCard = document.createElement('div');
                    productCard.className = 'glassmorphism rounded-2xl overflow-hidden group transform hover:-translate-y-2 transition-transform duration-300 shadow-lg';
                    productCard.innerHTML = `
                        <div class="relative">
                            <img src="${product.image}" alt="${product.name}" class="w-full h-64 object-cover">
                            <div class="absolute inset-0 bg-black bg-opacity-0 group-hover:bg-opacity-40 transition-all duration-300 flex items-center justify-center">
                                <button data-product-id="${product.id}" class="view-details-btn text-white bg-sky-500 bg-opacity-80 py-2 px-4 rounded-full opacity-0 group-hover:opacity-100 transition-opacity duration-300">View Details</button>
                            </div>
                        </div>
                        <div class="p-5">
                            <h3 class="text-lg font-semibold text-white truncate">${product.name}</h3>
                            <div class="flex justify-between items-center mt-3">
                                <p class="text-xl font-bold text-sky-400">$${product.price.toFixed(2)}</p>
                                <div class="flex items-center">
                                    <i data-feather="star" class="h-5 w-5 text-amber-400 fill-current"></i>
                                    <span class="ml-1 text-gray-300">${product.rating}</span>
                                </div>
                            </div>
                        </div>
                    `;
                    productGrid.appendChild(productCard);
                });
                feather.replace(); // Re-initialize icons
            }

            // Function to open and populate the modal
            function openModal(productId) {
                const product = products.find(p => p.id === parseInt(productId));
                if (!product) return;
                
                modalContent.innerHTML = `
                    <button id="close-modal-inner" class="absolute top-4 right-4 text-gray-400 hover:text-white z-10">
                        <i data-feather="x" class="h-8 w-8"></i>
                    </button>
                    <div class="w-full md:w-1/2 p-4">
                         <img src="${product.image.replace('?text=', '?height=800&width=800&text=')}" alt="${product.name}" class="w-full h-full object-cover rounded-xl">
                    </div>
                    <div class="w-full md:w-1/2 p-8 flex flex-col justify-center overflow-y-auto">
                        <h2 class="text-3xl font-bold text-white mb-2">${product.name}</h2>
                        <span class="text-sm text-gray-400 mb-4">In ${product.category}</span>
                        <div class="flex items-center mb-4">
                            <div class="flex text-amber-400">
                                <i data-feather="star" class="h-5 w-5 fill-current"></i>
                                <i data-feather="star" class="h-5 w-5 fill-current"></i>
                                <i data-feather="star" class="h-5 w-5 fill-current"></i>
                                <i data-feather="star" class="h-5 w-5 fill-current"></i>
                                <i data-feather="star" class="h-5 w-5 text-gray-500 fill-current"></i>
                            </div>
                            <span class="ml-2 text-gray-300">${product.rating} (${Math.floor(Math.random() * 200 + 50)} reviews)</span>
                        </div>
                        <p class="text-3xl font-bold text-sky-400 mb-6">$${product.price.toFixed(2)}</p>
                        <p class="text-gray-400 mb-6 leading-relaxed">
                            This is a placeholder description. The ${product.name} is a high-quality item perfect for your needs. It features state-of-the-art technology and a sleek design, ensuring both performance and style.
                        </p>
                        <div class="flex items-center space-x-4 mb-6">
                            <label for="quantity" class="font-semibold text-white">Quantity:</label>
                            <input type="number" id="quantity" value="1" min="1" class="w-16 bg-gray-800 border border-gray-700 rounded-lg py-1 px-2 text-white text-center">
                        </div>
                        <button class="w-full bg-sky-500 hover:bg-sky-600 text-white font-bold py-3 px-6 rounded-lg text-lg transition-all duration-300 flex items-center justify-center space-x-2">
                             <i data-feather="shopping-cart"></i>
                             <span>Add to Cart</span>
                        </button>
                    </div>
                `;
                
                productModal.classList.remove('hidden');
                setTimeout(() => {
                    modalContent.classList.remove('scale-95');
                }, 10);
                
                feather.replace();
                
                // Add event listener to the new close button inside the modal
                document.getElementById('close-modal-inner').addEventListener('click', closeModal);
            }
            
            // Function to close the modal
            function closeModal() {
                modalContent.classList.add('scale-95');
                setTimeout(() => {
                    productModal.classList.add('hidden');
                    modalContent.innerHTML = ''; // Clear content for next time
                }, 300);
            }
            
            // Event delegation for "View Details" buttons
            productGrid.addEventListener('click', function(e) {
                if (e.target && e.target.classList.contains('view-details-btn')) {
                    const productId = e.target.getAttribute('data-product-id');
                    openModal(productId);
                }
            });
            
            // Event listeners for closing the modal
            closeModalButton.addEventListener('click', closeModal);
            productModal.addEventListener('click', function(e) {
                if(e.target === productModal) { // Close if clicking on the backdrop
                    closeModal();
                }
            });

            // Initial render
            renderProducts(products);
        });
    </script>
</body>
</html>
