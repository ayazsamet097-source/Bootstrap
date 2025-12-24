# Bootstrap
<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Grarft Wear - Tarzını Yansıt</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.1/font/bootstrap-icons.css">
    <style>
        /* GİYİM MAĞAZASI ÖZEL CSS */
        body {
            font-family: 'Playfair Display', serif; /* Moda için daha şık bir font */
            background-color: #ffffff;
            color: #1a1a1a;
        }

        .text-theme { color: #8e7f70; } /* Toprak tonu/Bej detaylar */

        .btn-theme {
            background-color: #1a1a1a;
            color: #fff;
            font-weight: 500;
            border: none;
            letter-spacing: 1px;
        }
        .btn-theme:hover {
            background-color: #333;
            color: #fff;
        }

        /* HERO BÖLÜMÜ - GİYİM KONSEPTİ */
        .hero-section {
            background: linear-gradient(rgba(0,0,0,0.3), rgba(0,0,0,0.3)), 
                        url('https://images.unsplash.com/photo-1441986300917-64674bd600d8?q=80&w=2070'); 
            background-size: cover;
            background-position: center;
            height: 100vh;
            display: flex;
            align-items: center;
            border-bottom: 1px solid #eee;
        }

        .card {
            background-color: #f9f9f9;
            border: none;
            transition: all 0.4s ease;
        }
        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.05);
        }
        
        .navbar-brand span { color: #8e7f70; }
        .navbar { background-color: rgba(255,255,255,0.95) !important; }
        .nav-link { color: #1a1a1a !important; }
    </style>
</head>
<body>

    <nav class="navbar navbar-expand-lg navbar-light fixed-top shadow-sm">
        <div class="container">
            <a class="navbar-brand fw-bold fs-3 text-uppercase" href="#">Grarft <span>Wear</span></a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto text-uppercase small fw-bold">
                    <li class="nav-item"><a class="nav-link text-theme" href="#home">Koleksiyonlar</a></li>
                    <li class="nav-item"><a class="nav-link" href="#categories">Kategoriler</a></li>
                    <li class="nav-item"><a class="nav-link" href="#about">Hikayemiz</a></li>
                    <li class="nav-item"><a class="nav-link" href="#contact">İletişim</a></li>
                </ul>
                <a href="#shop" class="btn btn-theme ms-3 rounded-0 px-4 shadow-sm">ALIŞVERİŞE BAŞLA</a>
            </div>
        </div>
    </nav>

    <header id="home" class="hero-section text-center">
        <div class="container">
            <h1 class="display-2 fw-bold text-uppercase text-white mb-3" style="letter-spacing: 5px;">Yeni Sezon</h1>
            <p class="lead text-white mb-5 fs-4">Minimalist çizgiler, zamansız tasarımlar.</p>
            <div class="d-flex justify-content-center gap-3">
                <a href="#categories" class="btn btn-light btn-lg px-5 py-3 rounded-0 fw-bold">Koleksiyonu Gör</a>
                <a href="#contact" class="btn btn-outline-light btn-lg px-5 py-3 rounded-0">Bize Ulaşın</a>
            </div>
        </div>
    </header>

    <section id="categories" class="py-5">
        <div class="container">
            <div class="text-center mb-5">
                <h2 class="fw-bold text-uppercase display-6">Öne Çıkanlar</h2>
                <div style="width: 40px; height: 2px; background-color: #8e7f70; margin: 15px auto;"></div>
            </div>
            <div class="row g-4">
                <div class="col-md-4">
                    <div class="card h-100">
                        <div class="card-body text-center p-5">
                            <i class="bi bi-suit-club fs-1 text-theme mb-3"></i>
                            <h4 class="card-title">Premium Kumaş</h4>
                            <p class="card-text text-muted small">En kaliteli dokularla gün boyu süren konforu hissedin.</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="card h-100">
                        <div class="card-body text-center p-5">
                            <i class="bi bi-watch fs-1 text-theme mb-3"></i>
                            <h4 class="card-title">Aksesuar</h4>
                            <p class="card-text text-muted small">Stilinizi tamamlayan ince detaylar ve özel tasarımlar.</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="card h-100">
                        <div class="card-body text-center p-5">
                            <i class="bi bi-stars fs-1 text-theme mb-3"></i>
                            <h4 class="card-title">Sürdürülebilirlik</h4>
                            <p class="card-text text-muted small">Doğaya saygılı üretim süreçleri ve organik materyaller.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="about" class="py-5" style="background-color: #fafafa;">
        <div class="container">
            <div class="row align-items-center">
                <div class="col-md-6 mb-4 mb-md-0">
                    <img src="https://images.unsplash.com/photo-1490481651871-ab68de25d43d?q=80&w=2070" class="img-fluid grayscale shadow" alt="Moda">
                </div>
                <div class="col-md-6 ps-md-5">
                    <h5 class="text-theme text-uppercase fw-bold small">Hikayemiz</h5>
                    <h2 class="fw-bold mb-4">Zarafet Ayrıntıda Gizlidir</h2>
                    <p class="text-muted mb-4">
                        Grarft Wear olarak, modayı sadece giyinmek değil, bir ifade biçimi olarak görüyoruz. Şehir hayatının dinamizmini klasik dokunuşlarla birleştiriyoruz.
                    </p>
                    <ul class="list-unstyled">
                        <li class="mb-2"><i class="bi bi-check2 text-theme me-2"></i> Ücretsiz Hızlı Teslimat</li>
                        <li class="mb-2"><i class="bi bi-check2 text-theme me-2"></i> 30 Gün İade Garantisi</li>
                        <li class="mb-2"><i class="bi bi-check2 text-theme me-2"></i> Özel Paketleme Seçeneği</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <section id="contact" class="py-5">
        <div class="container">
            <div class="row justify-content-center">
                <div class="col-lg-8">
                    <div class="p-5 border" style="background-color: #fff;">
                        <h2 class="text-center fw-bold mb-4">Özel Teklifler İçin Kaydolun</h2>
                        <form>
                            <div class="row g-3">
                                <div class="col-md-6">
                                    <input type="text" class="form-control rounded-0 p-3" placeholder="Adınız">
                                </div>
                                <div class="col-md-6">
                                    <input type="email" class="form-control rounded-0 p-3" placeholder="E-posta Adresiniz">
                                </div>
                                <div class="col-12 mt-4">
                                    <button type="submit" class="btn btn-theme w-100 py-3 fw-bold text-uppercase">Bültene Abone Ol</button>
                                </div>
                            </div>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <footer class="py-4 text-center text-muted border-top">
        <div class="container">
            <p class="mb-0 small text-uppercase fw-bold">&copy; 2025 Grarft Wear Studio.</p>
        </div>
    </footer>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
