<?php
session_start();
if (!isset($_SESSION['admin'])) {
    header("Location: login.php");
    exit;
}
?>

<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <title>Dashboard Admin</title>
    <meta name="viewport" content="width=device-width, initial-scale=1">

    <!-- Bootstrap & Font Awesome -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css" rel="stylesheet">

    <style>
        body {
            background-color: #f8f9fa;
        }

        .dashboard-title {
            font-weight: 700;
            font-size: 1.5rem;
        }

        .card-menu {
            transition: all 0.3s ease;
            border-radius: 15px;
        }

        .card-menu:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
        }

        .icon-box {
            font-size: 2rem;
            color: #0d6efd;
        }
    </style>
</head>

<body>
    <nav class="navbar navbar-dark bg-dark px-3">
        <span class="navbar-brand mb-0 h1">CMS CV Darma Bakti</span>
        <a href="logout.php" class="btn btn-outline-light btn-sm">Logout</a>
    </nav>

    <div class="container my-5">
        <div class="mb-4 text-center">
            <h2 class="dashboard-title">Selamat Datang, <?= htmlspecialchars($_SESSION['admin']) ?>!</h2>
            <p class="text-muted">Silakan pilih menu di bawah ini untuk mengelola konten.</p>
        </div>

        <div class="row g-4">
            <div class="col-md-4">
                <a href="seragam.php" class="text-decoration-none text-dark">
                    <div class="card card-menu shadow-sm p-3 h-100">
                        <div class="d-flex align-items-center gap-3">
                            <i class="fas fa-tshirt icon-box"></i>
                            <div>
                                <h5 class="mb-1">Pakaian Dinas Harian</h5>
                                <small class="text-muted">Kelola katalog seragam PDH</small>
                            </div>
                        </div>
                    </div>
                </a>
            </div>

            <div class="col-md-4">
                <a href="pdl.php" class="text-decoration-none text-dark">
                    <div class="card card-menu shadow-sm p-3 h-100">
                        <div class="d-flex align-items-center gap-3">
                            <i class="fas fa-hard-hat icon-box"></i>
                            <div>
                                <h5 class="mb-1">Pakaian Dinas Lapangan</h5>
                                <small class="text-muted">Kelola katalog seragam PDL</small>
                            </div>
                        </div>
                    </div>
                </a>
            </div>

            <div class="col-md-4">
                <a href="klien.php" class="text-decoration-none text-dark">
                    <div class="card card-menu shadow-sm p-3 h-100">
                        <div class="d-flex align-items-center gap-3">
                            <i class="fas fa-handshake icon-box"></i>
                            <div>
                                <h5 class="mb-1">Logo Klien</h5>
                                <small class="text-muted">Atur logo perusahaan klien</small>
                            </div>
                        </div>
                    </div>
                </a>
            </div>
        </div>
    </div>

    <!-- Bootstrap JS -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
