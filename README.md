# Top-up-game
Oke ini amanah
/topup-game-website
│
├── index.html
├── style.css
├── script.js
├── /assets
│   ├── logo.png
│   ├── favicon.ico
│   └── /images
│       ├── mobile-legends.jpg
│       ├── free-fire.jpg
│       ├── pubg.jpg
│       ├── valorant.jpg
│       ├── genshin-impact.jpg
│       ├── cod-mobile.jpg
│       ├── roblox.jpg
│       └── apex-legends.jpg
└── README.txt<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GameTopUp - Top Up Semua Game</title>
    <meta name="description" content="Top up semua game favorit Anda seperti Mobile Legends, Free Fire, PUBG, Valorant dengan proses cepat dan aman">
    <meta name="keywords" content="top up game, voucher game, diamond ml, uc pubg, valorant points">
    <meta name="author" content="GameTopUp">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link rel="stylesheet" href="style.css">
    <link rel="icon" type="image/x-icon" href="assets/favicon.ico">
</head>
<body>
    <!-- Header & Navigation -->
    <header>
        <div class="container">
            <div class="header-content">
                <div class="logo">
                    <i class="fas fa-gamepad"></i>
                    GameTopUp
                </div>
                
                <ul class="nav-links">
                    <li><a href="#home"><i class="fas fa-home"></i> Beranda</a></li>
                    <li><a href="#games"><i class="fas fa-dice"></i> Game</a></li>
                    <li><a href="#popular"><i class="fas fa-fire"></i> Populer</a></li>
                    <li><a href="#promo"><i class="fas fa-gift"></i> Promo</a></li>
                    <li><a href="#help"><i class="fas fa-question-circle"></i> Bantuan</a></li>
                </ul>
                
                <div class="user-actions">
                    <a href="#" class="cart-icon" id="cartIcon">
                        <i class="fas fa-shopping-cart"></i>
                        <span class="cart-count" id="cartCount">0</span>
                    </a>
                    <a href="#" id="loginBtn"><i class="fas fa-user"></i> Masuk</a>
                </div>
                
                <div class="mobile-menu-btn" id="mobileMenuBtn">
                    <i class="fas fa-bars"></i>
                </div>
            </div>
            
            <div class="mobile-menu" id="mobileMenu">
                <ul>
                    <li><a href="#home"><i class="fas fa-home"></i> Beranda</a></li>
                    <li><a href="#games"><i class="fas fa-dice"></i> Game</a></li>
                    <li><a href="#popular"><i class="fas fa-fire"></i> Populer</a></li>
                    <li><a href="#promo"><i class="fas fa-gift"></i> Promo</a></li>
                    <li><a href="#help"><i class="fas fa-question-circle"></i> Bantuan</a></li>
                </ul>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="container">
            <h1>Top Up Semua Game Favoritmu</h1>
            <p>Diamond, Voucher, Item, dan UC untuk game populer seperti Mobile Legends, Free Fire, PUBG, Valorant, dan banyak lagi. Proses cepat & aman!</p>
            
            <div class="search-box">
                <input type="text" id="searchInput" placeholder="Cari game atau item yang kamu mau...">
                <button id="searchBtn"><i class="fas fa-search"></i> Cari</button>
            </div>
        </div>
    </section>

    <!-- Main Content -->
    <main class="container">
        <!-- Game Categories -->
        <h2 class="section-title" id="games">Pilih Game</h2>
        <div class="categories">
            <div class="category-btn active" data-category="all">Semua</div>
            <div class="category-btn" data-category="mobile">Mobile</div>
            <div class="category-btn" data-category="pc">PC</div>
            <div class="category-btn" data-category="console">Console</div>
            <div class="category-btn" data-category="popular">Populer</div>
        </div>

        <!-- Games Grid -->
        <div class="games-grid" id="gamesGrid">
            <!-- Game cards will be dynamically generated -->
        </div>

        <!-- Popular Items -->
        <h2 class="section-title" id="popular">Item Populer</h2>
        <div class="popular-items">
            <div class="item-card">
                <div class="item-icon">
                    <i class="fas fa-gem"></i>
                </div>
                <h3 class="item-title">100 Diamond ML</h3>
                <div class="item-price">Rp 15.000</div>
                <button class="buy-btn" data-id="ml-100">Beli Sekarang</button>
            </div>
            
            <div class="item-card">
                <div class="item-icon">
                    <i class="fas fa-fire"></i>
                </div>
                <h3 class="item-title">100 UC PUBG</h3>
                <div class="item-price">Rp 20.000</div>
                <button class="buy-btn" data-id="pubg-100">Beli Sekarang</button>
            </div>
            
            <div class="item-card">
                <div class="item-icon">
                    <i class="fas fa-crown"></i>
                </div>
                <h3 class="item-title">Voucher Valorant 500</h3>
                <div class="item-price">Rp 75.000</div>
                <button class="buy-btn" data-id="val-500">Beli Sekarang</button>
            </div>
            
            <div class="item-card">
                <div class="item-icon">
                    <i class="fas fa-coins"></i>
                </div>
                <h3 class="item-title">1000 Coin FF</h3>
                <div class="item-price">Rp 12.000</div>
                <button class="buy-btn" data-id="ff-1000">Beli Sekarang</button>
            </div>
        </div>

        <!-- Payment Methods -->
        <h2 class="section-title">Metode Pembayaran</h2>
        <div class="payment-methods">
            <div class="payment-method">
                <i class="fab fa-cc-visa" style="color: #1a1f71;"></i> Visa
            </div>
            <div class="payment-method">
                <i class="fab fa-cc-mastercard" style="color: #eb001b;"></i> Mastercard
            </div>
            <div class="payment-method">
                <i class="fas fa-qrcode" style="color: #00aaff;"></i> QRIS
            </div>
            <div class="payment-method">
                <i class="fas fa-mobile-alt" style="color: #ff6b00;"></i> E-Wallet
            </div>
            <div class="payment-method">
                <i class="fas fa-university" style="color: #008c00;"></i> Transfer Bank
            </div>
            <div class="payment-method">
                <i class="fas fa-store" style="color: #ff0080;"></i> Alfamart/Indomaret
            </div>
        </div>

        <!-- Promo Section -->
        <h2 class="section-title" id="promo">Promo & Diskon</h2>
        <div class="promo-section">
            <div class="promo-card">
                <div class="promo-badge">HOT</div>
                <h3>New User Discount</h3>
                <p>Diskon 20% untuk pembelian pertama</p>
                <span class="promo-code">Kode: NEWUSER20</span>
            </div>
            <div class="promo-card">
                <div class="promo-badge">LIMITED</div>
                <h3>Weekend Special</h3>
                <p>Cashback 10% setiap akhir pekan</p>
                <span class="promo-code">Kode: WEEKEND10</span>
            </div>
            <div class="promo-card">
                <div class="promo-badge">BEST</div>
                <h3>Beli 2 Gratis 1</h3>
                <p>Untuk pembelian diamond ML minimal 500</p>
                <span class="promo-code">Kode: MLBUY2GET1</span>
            </div>
        </div>
    </main>

    <!-- Cart Modal -->
    <div class="cart-modal" id="cartModal">
        <div class="cart-content">
            <div class="cart-header">
                <h2><i class="fas fa-shopping-cart"></i> Keranjang Belanja</h2>
                <button id="closeCartBtn" style="background:none; border:none; color:white; font-size:1.5rem; cursor:pointer;">
                    <i class="fas fa-times"></i>
                </button>
            </div>
            
            <div class="cart-items" id="cartItems">
                <p id="emptyCartMessage">Keranjang belanja kamu masih kosong.</p>
            </div>
            
            <div class="cart-footer">
                <div class="cart-total">
                    <span>Total:</span>
                    <span id="cartTotal">Rp 0</span>
                </div>
                
                <div class="cart-actions">
                    <button class="close-cart-btn" id="continueShoppingBtn">Lanjut Belanja</button>
                    <button class="checkout-btn" id="checkoutBtn">Checkout</button>
                </div>
            </div>
        </div>
    </div>

    <!-- Login Modal -->
    <div class="login-modal" id="loginModal">
        <div class="login-content">
            <div class="login-header">
                <h2><i class="fas fa-user"></i> Masuk ke Akun</h2>
                <button id="closeLoginBtn" style="background:none; border:none; color:white; font-size:1.5rem; cursor:pointer;">
                    <i class="fas fa-times"></i>
                </button>
            </div>
            
            <div class="login-body">
                <div class="login-form">
                    <div class="form-group">
                        <label for="email">Email atau Username</label>
                        <input type="text" id="email" placeholder="masukkan email atau username">
                    </div>
                    
                    <div class="form-group">
                        <label for="password">Password</label>
                        <input type="password" id="password" placeholder="masukkan password">
                    </div>
                    
                    <button class="login-submit-btn" id="loginSubmitBtn">Masuk</button>
                    
                    <div class="login-links">
                        <a href="#">Lupa Password?</a>
                        <a href="#" id="registerLink">Buat Akun Baru</a>
                    </div>
                    
                    <div class="login-divider">
                        <span>atau masuk dengan</span>
                    </div>
                    
                    <div class="social-login">
                        <button class="social-btn google-btn">
                            <i class="fab fa-google"></i> Google
                        </button>
                        <button class="social-btn facebook-btn">
                            <i class="fab fa-facebook-f"></i> Facebook
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content" id="help">
                <div class="footer-column">
                    <h3>GameTopUp</h3>
                    <p>Platform top up game terpercaya dengan proses cepat dan aman. Mendukung berbagai game populer di seluruh platform.</p>
                    <div class="social-links">
                        <a href="#"><i class="fab fa-facebook-f"></i></a>
                        <a href="#"><i class="fab fa-twitter"></i></a>
                        <a href="#"><i class="fab fa-instagram"></i></a>
                        <a href="#"><i class="fab fa-youtube"></i></a>
                    </div>
                </div>
                
                <div class="footer-column">
                    <h3>Layanan</h3>
                    <ul>
                        <li><a href="#">Top Up Game</a></li>
                        <li><a href="#">Voucher Game</a></li>
                        <li><a href="#">Item Game</a></li>
                        <li><a href="#">Akun Game</a></li>
                        <li><a href="#">Joki Rank</a></li>
                    </ul>
                </div>
                
                <div class="footer-column">
                    <h3>Bantuan</h3>
                    <ul>
                        <li><a href="#">Cara Order</a></li>
                        <li><a href="#">FAQ</a></li>
                        <li><a href="#">Syarat & Ketentuan</a></li>
                        <li><a href="#">Kebijakan Privasi</a></li>
                        <li><a href="#">Hubungi Kami</a></li>
                    </ul>
                </div>
                
                <div class="footer-column">
                    <h3>Game Populer</h3>
                    <ul>
                        <li><a href="#">Mobile Legends</a></li>
                        <li><a href="#">Free Fire</a></li>
                        <li><a href="#">PUBG Mobile</a></li>
                        <li><a href="#">Valorant</a></li>
                        <li><a href="#">Genshin Impact</a></li>
                    </ul>
                </div>
            </div>
            
            <div class="copyright">
                &copy; <span id="currentYear"></span> GameTopUp. All rights reserved. Semua merek dagang adalah hak cipta dari pemiliknya masing-masing.
            </div>
        </div>
    </footer>

    <script src="script.js"></script>
</body>
</html>
