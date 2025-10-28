<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pair Pressure | Premium Footwear & Luxury Bags</title>
    <meta name="description" content="Pair Pressure - Nigeria's premier destination for authentic luxury footwear, designer bags, and premium accessories. Grade A originals only.">
    <meta name="keywords" content="luxury shoes Nigeria, designer bags, authentic sneakers, premium footwear, original Jordan, Nike, Adidas, luxury accessories">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@400;700&family=Montserrat:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --gold: #D4AF37;
            --dark-gold: #B8860B;
            --black: #000000;
            --dark-gray: #1A1A1A;
            --light-gray: #F5F5F5;
            --white: #FFFFFF;
            --transition: all 0.3s ease;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Montserrat', sans-serif;
            background-color: var(--black);
            color: var(--white);
            line-height: 1.6;
            overflow-x: hidden;
        }

        h1, h2, h3, h4, h5 {
            font-family: 'Cinzel', serif;
            font-weight: 700;
            margin-bottom: 1rem;
        }

        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
        }

        section {
            padding: 80px 0;
        }

        .btn {
            display: inline-block;
            padding: 12px 30px;
            background-color: var(--gold);
            color: var(--black);
            text-decoration: none;
            font-weight: 600;
            border: none;
            border-radius: 2px;
            cursor: pointer;
            transition: var(--transition);
            text-transform: uppercase;
            letter-spacing: 1px;
            font-size: 0.9rem;
        }

        .btn:hover {
            background-color: var(--dark-gold);
            transform: translateY(-3px);
            box-shadow: 0 10px 20px rgba(212, 175, 55, 0.2);
        }

        .btn-outline {
            background-color: transparent;
            border: 2px solid var(--gold);
            color: var(--gold);
        }

        .btn-outline:hover {
            background-color: var(--gold);
            color: var(--black);
        }

        .section-title {
            text-align: center;
            margin-bottom: 50px;
            position: relative;
        }

        .section-title:after {
            content: '';
            position: absolute;
            bottom: -15px;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 2px;
            background-color: var(--gold);
        }

        /* Header Styles */
        header {
            background-color: rgba(0, 0, 0, 0.95);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            padding: 15px 0;
            transition: var(--transition);
            border-bottom: 1px solid rgba(212, 175, 55, 0.2);
        }

        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-family: 'Cinzel', serif;
            font-size: 2.2rem;
            font-weight: 700;
            color: var(--gold);
            letter-spacing: 2px;
        }

        .logo span {
            color: var(--white);
        }

        nav ul {
            display: flex;
            list-style: none;
        }

        nav ul li {
            margin-left: 30px;
        }

        nav ul li a {
            text-decoration: none;
            color: var(--white);
            font-weight: 500;
            transition: var(--transition);
            position: relative;
        }

        nav ul li a:after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 0;
            height: 1px;
            background-color: var(--gold);
            transition: var(--transition);
        }

        nav ul li a:hover {
            color: var(--gold);
        }

        nav ul li a:hover:after {
            width: 100%;
        }

        .mobile-menu {
            display: none;
            font-size: 1.5rem;
            cursor: pointer;
            color: var(--gold);
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(0, 0, 0, 0.8), rgba(0, 0, 0, 0.8)), url('https://images.unsplash.com/photo-1549298916-b41d501d3772?ixlib=rb-4.0.3&auto=format&fit=crop&w=1350&q=80');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
            min-height: 100vh;
            display: flex;
            align-items: center;
            text-align: center;
            position: relative;
            padding-top: 80px;
        }

        @media (max-width: 768px) {
            .hero {
                background-attachment: scroll;
                background-position: 70% center;
            }
        }

        .hero-content {
            max-width: 800px;
            margin: 0 auto;
        }

        .hero h1 {
            font-size: 4.5rem;
            margin-bottom: 20px;
            text-transform: uppercase;
            letter-spacing: 3px;
        }

        .hero p {
            font-size: 1.3rem;
            margin-bottom: 30px;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
            color: #ddd;
        }

        /* Featured Products */
        .featured-products {
            background-color: var(--dark-gray);
            position: relative;
        }

        .featured-products:before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: url('https://www.transparenttextures.com/patterns/diagmonds.png');
            opacity: 0.1;
        }

        .products-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 30px;
            position: relative;
            z-index: 1;
        }

        .product-card {
            background-color: var(--black);
            border-radius: 5px;
            overflow: hidden;
            transition: var(--transition);
            position: relative;
            border: 1px solid rgba(212, 175, 55, 0.1);
        }

        .product-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(212, 175, 55, 0.15);
            border-color: rgba(212, 175, 55, 0.3);
        }

        .product-image {
            height: 250px;
            overflow: hidden;
            position: relative;
            background-color: var(--dark-gray);
        }

        .product-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: var(--transition);
        }

        .product-card:hover .product-image img {
            transform: scale(1.05);
        }

        .product-overlay {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.7);
            display: flex;
            align-items: center;
            justify-content: center;
            opacity: 0;
            transition: var(--transition);
        }

        .product-card:hover .product-overlay {
            opacity: 1;
        }

        .product-content {
            padding: 20px;
        }

        .product-title {
            font-size: 1.2rem;
            margin-bottom: 10px;
        }

        .product-price {
            color: var(--gold);
            font-weight: 600;
            font-size: 1.1rem;
            margin-bottom: 15px;
        }

        .product-category {
            font-size: 0.8rem;
            color: #aaa;
            text-transform: uppercase;
            letter-spacing: 1px;
            margin-bottom: 5px;
        }

        /* Categories Section */
        .categories {
            background-color: var(--black);
        }

        .categories-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 20px;
        }

        .category-card {
            height: 200px;
            border-radius: 5px;
            overflow: hidden;
            position: relative;
            transition: var(--transition);
            cursor: pointer;
        }

        .category-card:hover {
            transform: translateY(-5px);
        }

        .category-image {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .category-overlay {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(to bottom, transparent, rgba(0,0,0,0.8));
            display: flex;
            align-items: flex-end;
            padding: 20px;
        }

        .category-name {
            color: var(--white);
            font-size: 1.5rem;
            font-weight: 600;
        }

        /* Catalog Section */
        .catalog {
            background-color: var(--dark-gray);
            position: relative;
        }

        .catalog:before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: url('https://www.transparenttextures.com/patterns/diagmonds.png');
            opacity: 0.1;
        }

        .brands-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(150px, 1fr));
            gap: 20px;
            margin-bottom: 50px;
        }

        .brand-card {
            background-color: var(--black);
            border-radius: 5px;
            padding: 20px;
            text-align: center;
            transition: var(--transition);
            border: 1px solid rgba(212, 175, 55, 0.1);
        }

        .brand-card:hover {
            transform: translateY(-5px);
            border-color: rgba(212, 175, 55, 0.3);
        }

        .brand-logo {
            height: 60px;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 10px;
        }

        .brand-logo img {
            max-height: 100%;
            max-width: 100%;
            filter: brightness(0) invert(1);
        }

        .brand-name {
            font-weight: 600;
            font-size: 0.9rem;
        }

        .catalog-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
            gap: 20px;
        }

        .catalog-item {
            background-color: var(--black);
            border-radius: 5px;
            overflow: hidden;
            transition: var(--transition);
            border: 1px solid rgba(212, 175, 55, 0.1);
        }

        .catalog-item:hover {
            transform: translateY(-5px);
            border-color: rgba(212, 175, 55, 0.3);
        }

        .catalog-image {
            height: 180px;
            overflow: hidden;
        }

        .catalog-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .catalog-content {
            padding: 15px;
        }

        .catalog-title {
            font-size: 0.9rem;
            margin-bottom: 5px;
        }

        .catalog-type {
            font-size: 0.8rem;
            color: #aaa;
        }

        /* Bags Section */
        .bags-section {
            background-color: var(--black);
        }

        /* WhatsApp Floating Button */
        .whatsapp-float {
            position: fixed;
            bottom: 30px;
            right: 30px;
            width: 60px;
            height: 60px;
            background-color: #25D366;
            color: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.8rem;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
            z-index: 1000;
            transition: var(--transition);
            animation: pulse 2s infinite;
        }

        .whatsapp-float:hover {
            transform: scale(1.1);
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.4);
        }

        @keyframes pulse {
            0% {
                box-shadow: 0 0 0 0 rgba(37, 211, 102, 0.7);
            }
            70% {
                box-shadow: 0 0 0 15px rgba(37, 211, 102, 0);
            }
            100% {
                box-shadow: 0 0 0 0 rgba(37, 211, 102, 0);
            }
        }

        /* Responsive Styles */
        @media (max-width: 992px) {
            .hero h1 {
                font-size: 3.5rem;
            }
        }

        @media (max-width: 768px) {
            nav ul {
                display: none;
                position: absolute;
                top: 70px;
                left: 0;
                width: 100%;
                background-color: var(--black);
                flex-direction: column;
                padding: 20px;
                box-shadow: 0 10px 20px rgba(0, 0, 0, 0.3);
                border-top: 1px solid rgba(212, 175, 55, 0.2);
            }

            nav ul.show {
                display: flex;
            }

            nav ul li {
                margin: 10px 0;
            }

            .mobile-menu {
                display: block;
            }

            .hero h1 {
                font-size: 2.5rem;
                letter-spacing: 2px;
            }

            .hero p {
                font-size: 1.1rem;
            }

            .logo {
                font-size: 1.8rem;
            }
        }

        @media (max-width: 480px) {
            .hero h1 {
                font-size: 2rem;
            }
            
            .brands-grid {
                grid-template-columns: repeat(auto-fill, minmax(120px, 1fr));
            }
        }
    </style>
</head>
<body>
    <!-- WhatsApp Floating Button -->
    <a href="https://wa.me/2349163702078" class="whatsapp-float" target="_blank">
        <i class="fab fa-whatsapp"></i>
    </a>

    <!-- Header -->
    <header>
        <div class="container header-container">
            <div class="logo">Pair <span>Pressure</span></div>
            <nav>
                <ul id="nav-menu">
                    <li><a href="#home">Home</a></li>
                    <li><a href="#featured">Featured</a></li>
                    <li><a href="#shoes">Shoes</a></li>
                    <li><a href="#bags">Bags</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
                <div class="mobile-menu" id="mobile-menu">
                    <i class="fas fa-bars"></i>
                </div>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="container">
            <div class="hero-content">
                <h1>Pair Pressure</h1>
                <p>Premium Footwear & Luxury Bags. Authentic Grade A Originals Only.</p>
                <a href="#shoes" class="btn">Explore Collection</a>
            </div>
        </div>
    </section>

    <!-- Featured Products Section -->
    <section class="featured-products" id="featured">
        <div class="container">
            <h2 class="section-title">Featured Products</h2>
            <div class="products-grid">
                <!-- Featured Product 1 -->
                <div class="product-card">
                    <div class="product-image">
                        <img src="https://images.unsplash.com/photo-1549298916-b41d501d3772?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Air Jordan 1 Retro High">
                        <div class="product-overlay">
                            <a href="https://wa.me/2349163702078?text=Hi,%20I'm%20interested%20in%20the%20Air%20Jordan%201%20Retro%20High" class="btn" target="_blank">Inquire</a>
                        </div>
                    </div>
                    <div class="product-content">
                        <div class="product-category">Sneakers</div>
                        <h3 class="product-title">Air Jordan 1 Retro High</h3>
                        <p class="product-price">$320</p>
                        <a href="https://wa.me/2349163702078?text=Hi,%20I'm%20interested%20in%20the%20Air%20Jordan%201%20Retro%20High" class="btn btn-outline" target="_blank">Buy Now</a>
                    </div>
                </div>

                <!-- Featured Product 2 -->
                <div class="product-card">
                    <div class="product-image">
                        <img src="https://images.unsplash.com/photo-1606107557195-0e29a4b5b4aa?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Nike Air Force 1">
                        <div class="product-overlay">
                            <a href="https://wa.me/2349163702078?text=Hi,%20I'm%20interested%20in%20the%20Nike%20Air%20Force%201" class="btn" target="_blank">Inquire</a>
                        </div>
                    </div>
                    <div class="product-content">
                        <div class="product-category">Sneakers</div>
                        <h3 class="product-title">Nike Air Force 1 '07</h3>
                        <p class="product-price">$120</p>
                        <a href="https://wa.me/2349163702078?text=Hi,%20I'm%20interested%20in%20the%20Nike%20Air%20Force%201%20'07" class="btn btn-outline" target="_blank">Buy Now</a>
                    </div>
                </div>

                <!-- Featured Product 3 -->
                <div class="product-card">
                    <div class="product-image">
                        <img src="https://images.unsplash.com/photo-1584917865442-de89df76afd3?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Designer Handbag">
                        <div class="product-overlay">
                            <a href="https://wa.me/2349163702078?text=Hi,%20I'm%20interested%20in%20the%20Designer%20Handbag" class="btn" target="_blank">Inquire</a>
                        </div>
                    </div>
                    <div class="product-content">
                        <div class="product-category">Bags</div>
                        <h3 class="product-title">Luxury Leather Handbag</h3>
                        <p class="product-price">$450</p>
                        <a href="https://wa.me/2349163702078?text=Hi,%20I'm%20interested%20in%20the%20Luxury%20Leather%20Handbag" class="btn btn-outline" target="_blank">Buy Now</a>
                    </div>
                </div>

                <!-- Featured Product 4 -->
                <div class="product-card">
                    <div class="product-image">
                        <img src="https://images.unsplash.com/photo-1600185365483-26d7a4cc7519?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Adidas Ultraboost">
                        <div class="product-overlay">
                            <a href="https://wa.me/2349163702078?text=Hi,%20I'm%20interested%20in%20the%20Adidas%20Ultraboost" class="btn" target="_blank">Inquire</a>
                        </div>
                    </div>
                    <div class="product-content">
                        <div class="product-category">Running Shoes</div>
                        <h3 class="product-title">Adidas Ultraboost 22</h3>
                        <p class="product-price">$180</p>
                        <a href="https://wa.me/2349163702078?text=Hi,%20I'm%20interested%20in%20the%20Adidas%20Ultraboost%2022" class="btn btn-outline" target="_blank">Buy Now</a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Categories Section -->
    <section class="categories">
        <div class="container">
            <h2 class="section-title">Collections</h2>
            <div class="categories-grid">
                <div class="category-card" onclick="location.href='#shoes'">
                    <img src="https://images.unsplash.com/photo-1606107557195-0e29a4b5b4aa?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Sneakers" class="category-image">
                    <div class="category-overlay">
                        <h3 class="category-name">Sneakers</h3>
                    </div>
                </div>
                <div class="category-card" onclick="location.href='#bags'">
                    <img src="https://images.unsplash.com/photo-1584917865442-de89df76afd3?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Bags" class="category-image">
                    <div class="category-overlay">
                        <h3 class="category-name">Bags</h3>
                    </div>
                </div>
                <div class="category-card">
                    <img src="https://images.unsplash.com/photo-1525966222134-fcfa99b8ae77?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Casual Shoes" class="category-image">
                    <div class="category-overlay">
                        <h3 class="category-name">Casual Shoes</h3>
                    </div>
                </div>
                <div class="category-card">
                    <img src="https://images.unsplash.com/photo-1575537302964-96cd47c06b1b?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Formal Shoes" class="category-image">
                    <div class="category-overlay">
                        <h3 class="category-name">Formal Shoes</h3>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Shoes Catalog Section -->
    <section class="catalog" id="shoes">
        <div class="container">
            <h2 class="section-title">Premium Footwear Collection</h2>
            
            <div class="brands-grid" id="brands">
                <div class="brand-card">
                    <div class="brand-logo">
                        <span style="font-weight: bold; color: var(--gold);">NIKE</span>
                    </div>
                    <div class="brand-name">Nike</div>
                </div>
                <div class="brand-card">
                    <div class="brand-logo">
                        <span style="font-weight: bold; color: var(--gold);">JORDAN</span>
                    </div>
                    <div class="brand-name">Jordan</div>
                </div>
                <div class="brand-card">
                    <div class="brand-logo">
                        <span style="font-weight: bold; color: var(--gold);">ADIDAS</span>
                    </div>
                    <div class="brand-name">Adidas</div>
                </div>
                <div class="brand-card">
                    <div class="brand-logo">
                        <span style="font-weight: bold; color: var(--gold);">NEW BALANCE</span>
                    </div>
                    <div class="brand-name">New Balance</div>
                </div>
                <div class="brand-card">
                    <div class="brand-logo">
                        <span style="font-weight: bold; color: var(--gold);">PUMA</span>
                    </div>
                    <div class="brand-name">Puma</div>
                </div>
                <div class="brand-card">
                    <div class="brand-logo">
                        <span style="font-weight: bold; color: var(--gold);">REEBOK</span>
                    </div>
                    <div class="brand-name">Reebok</div>
                </div>
            </div>

            <h3 class="section-title" style="margin-top: 60px;">Sneaker Collection</h3>
            <div class="catalog-grid">
                <!-- Nike Shoes -->
                <div class="catalog-item">
                    <div class="catalog-image">
                        <img src="https://images.unsplash.com/photo-1549298916-b41d501d3772?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80" alt="Nike Dunk Low">
                    </div>
                    <div class="catalog-content">
                        <h4 class="catalog-title">Nike Dunk Low Retro</h4>
                        <p class="catalog-type">Nike • Sneakers</p>
                    </div>
                </div>
                <div class="catalog-item">
                    <div class="catalog-image">
                        <img src="https://images.unsplash.com/photo-1606107557195-0e29a4b5b4aa?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80" alt="Nike Air Max 97">
                    </div>
                    <div class="catalog-content">
                        <h4 class="catalog-title">Nike Air Max 97</h4>
                        <p class="catalog-type">Nike • Sneakers</p>
                    </div>
                </div>
                
                <!-- Jordan Shoes -->
                <div class="catalog-item">
                    <div class="catalog-image">
                        <img src="https://images.unsplash.com/photo-1600269452121-4f2416e55c28?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80" alt="Jordan 4 Retro">
                    </div>
                    <div class="catalog-content">
                        <h4 class="catalog-title">Air Jordan 4 Retro</h4>
                        <p class="catalog-type">Jordan • Sneakers</p>
                    </div>
                </div>
                <div class="catalog-item">
                    <div class="catalog-image">
                        <img src="https://images.unsplash.com/photo-1543508282-6319a3e2621f?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80" alt="Jordan 11 Retro">
                    </div>
                    <div class="catalog-content">
                        <h4 class="catalog-title">Air Jordan 11 Retro</h4>
                        <p class="catalog-type">Jordan • Sneakers</p>
                    </div>
                </div>
                
                <!-- Adidas Shoes -->
                <div class="catalog-item">
                    <div class="catalog-image">
                        <img src="https://images.unsplash.com/photo-1600185365483-26d7a4cc7519?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80" alt="Adidas Yeezy Boost">
                    </div>
                    <div class="catalog-content">
                        <h4 class="catalog-title">Adidas Yeezy Boost 350</h4>
                        <p class="catalog-type">Adidas • Sneakers</p>
                    </div>
                </div>
                <div class="catalog-item">
                    <div class="catalog-image">
                        <img src="https://images.unsplash.com/photo-1515955656352-a1fa3ffcd111?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80" alt="Adidas Superstar">
                    </div>
                    <div class="catalog-content">
                        <h4 class="catalog-title">Adidas Superstar</h4>
                        <p class="catalog-type">Adidas • Sneakers</p>
                    </div>
                </div>
                
                <!-- New Balance Shoes -->
                <div class="catalog-item">
                    <div class="catalog-image">
                        <img src="https://images.unsplash.com/photo-1542280756-74b2f55e73ab?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80" alt="New Balance 550">
                    </div>
                    <div class="catalog-content">
                        <h4 class="catalog-title">New Balance 550</h4>
                        <p class="catalog-type">New Balance • Sneakers</p>
                    </div>
                </div>
                <div class="catalog-item">
                    <div class="catalog-image">
                        <img src="https://images.unsplash.com/photo-1606107557195-0e29a4b5b4aa?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80" alt="New Balance 990">
                    </div>
                    <div class="catalog-content">
                        <h4 class="catalog-title">New Balance 990v5</h4>
                        <p class="catalog-type">New Balance • Running</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Bags Section -->
    <section class="bags-section" id="bags">
        <div class="container">
            <h2 class="section-title">Luxury Bags Collection</h2>
            <div class="catalog-grid">
                <!-- Bags -->
                <div class="catalog-item">
                    <div class="catalog-image">
                        <img src="https://images.unsplash.com/photo-1584917865442-de89df76afd3?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80" alt="Designer Handbag">
                    </div>
                    <div class="catalog-content">
                        <h4 class="catalog-title">Luxury Leather Tote</h4>
                        <p class="catalog-type">Handbag • Women</p>
                    </div>
                </div>
                <div class="catalog-item">
                    <div class="catalog-image">
                        <img src="https://images.unsplash.com/photo-1553062407-98eeb64c6a62?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80" alt="Designer Backpack">
                    </div>
                    <div class="catalog-content">
                        <h4 class="catalog-title">Premium Leather Backpack</h4>
                        <p class="catalog-type">Backpack • Unisex</p>
                    </div>
                </div>
                <div class="catalog-item">
                    <div class="catalog-image">
                        <img src="https://images.unsplash.com/photo-1591561954557-26941169b49e?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80" alt="Crossbody Bag">
                    </div>
                    <div class="catalog-content">
                        <h4 class="catalog-title">Designer Crossbody Bag</h4>
                        <p class="catalog-type">Crossbody • Women</p>
                    </div>
                </div>
                <div class="catalog-item">
                    <div class="catalog-image">
                        <img src="https://images.unsplash.com/photo-1584917865442-de89df76afd3?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80" alt="Evening Clutch">
                    </div>
                    <div class="catalog-content">
                        <h4 class="catalog-title">Evening Clutch Purse</h4>
                        <p class="catalog-type">Clutch • Women</p>
                    </div>
                </div>
            </div>
            
            <div style="text-align: center; margin-top: 40px;">
                <a href="https://wa.me/2349163702078?text=Hi,%20I%20would%20like%20to%20see%20the%20full%20shoe%20and%20bag%20catalog" class="btn" target="_blank">View Full Catalog</a>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section class="contact" id="contact">
        <div class="container">
            <h2 class="section-title">Contact Us</h2>
            <div style="text-align: center; max-width: 600px; margin: 0 auto;">
                <p>Ready to elevate your style? Contact us for inquiries about our premium collection of authentic footwear and luxury bags.</p>
                <div style="margin-top: 30px;">
                    <a href="https://wa.me/2349163702078" class="btn" style="margin: 10px;" target="_blank">WhatsApp</a>
                    <a href="tel:+2349163702078" class="btn btn-outline" style="margin: 10px;">Call Us</a>
                </div>
                <div style="margin-top: 30px;">
                    <p><strong>Location:</strong> Edo State, Nigeria</p>
                    <p><strong>Delivery:</strong> Nationwide across Nigeria</p>
                </div>
            </div>
        </div>
    </section>

    <script>
        // Mobile Menu Toggle
        const mobileMenu = document.getElementById('mobile-menu');
        const navMenu = document.getElementById('nav-menu');

        mobileMenu.addEventListener('click', () => {
            navMenu.classList.toggle('show');
        });

        // Header Scroll Effect
        window.addEventListener('scroll', () => {
            const header = document.querySelector('header');
            if (window.scrollY > 100) {
                header.style.backgroundColor = 'rgba(0, 0, 0, 0.98)';
                header.style.padding = '10px 0';
            } else {
                header.style.backgroundColor = 'rgba(0, 0, 0, 0.95)';
                header.style.padding = '15px 0';
            }
        });

        // Smooth Scrolling for Anchor Links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                if (targetId === '#') return;
                
                const targetElement = document.querySelector(targetId);
                if (targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                    
                    // Close mobile menu if open
                    if (navMenu.classList.contains('show')) {
                        navMenu.classList.remove('show');
                    }
                }
            });
        });
    </script>
</body>
</html>
