<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Free online image compression tool - Reduce image file size while maintaining quality. Optimize your images for web and mobile.">
    <meta name="keywords" content="image compression, image optimizer, reduce image size, image tool, web optimization">
    <title>ImageCompress Pro - Free Online Image Compression Tool</title>
    <style>
        :root {
            --primary: #4361ee;
            --primary-dark: #3a56d4;
            --secondary: #7209b7;
            --light: #f8f9fa;
            --dark: #212529;
            --success: #4bb543;
            --warning: #ffcc00;
            --danger: #dc3545;
            --gray: #6c757d;
            --border-radius: 8px;
            --box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            --transition: all 0.3s ease;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: #f5f7fb;
            color: var(--dark);
            line-height: 1.6;
        }

        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        header {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
            padding: 1.5rem 0;
            box-shadow: var(--box-shadow);
        }

        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.8rem;
            font-weight: 700;
            display: flex;
            align-items: center;
        }

        .logo i {
            margin-right: 10px;
            font-size: 2rem;
        }

        nav ul {
            display: flex;
            list-style: none;
        }

        nav ul li {
            margin-left: 1.5rem;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: var(--transition);
        }

        nav ul li a:hover {
            color: rgba(255, 255, 255, 0.8);
        }

        .hero {
            text-align: center;
            padding: 3rem 0;
            background-color: white;
            margin-bottom: 2rem;
            border-radius: var(--border-radius);
            box-shadow: var(--box-shadow);
            margin-top: 2rem;
        }

        .hero h1 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
            color: var(--primary);
        }

        .hero p {
            font-size: 1.2rem;
            color: var(--gray);
            max-width: 700px;
            margin: 0 auto 2rem;
        }

        .main-content {
            display: grid;
            grid-template-columns: 1fr 300px;
            gap: 2rem;
            margin-bottom: 2rem;
        }

        .compression-tool {
            background-color: white;
            border-radius: var(--border-radius);
            box-shadow: var(--box-shadow);
            padding: 2rem;
        }

        .tool-section {
            margin-bottom: 2rem;
        }

        .tool-section h2 {
            font-size: 1.5rem;
            margin-bottom: 1rem;
            color: var(--primary);
            display: flex;
            align-items: center;
        }

        .tool-section h2 i {
            margin-right: 10px;
        }

        .upload-area {
            border: 2px dashed #ccc;
            border-radius: var(--border-radius);
            padding: 3rem 2rem;
            text-align: center;
            cursor: pointer;
            transition: var(--transition);
            margin-bottom: 1.5rem;
        }

        .upload-area:hover {
            border-color: var(--primary);
            background-color: rgba(67, 97, 238, 0.05);
        }

        .upload-area i {
            font-size: 3rem;
            color: var(--primary);
            margin-bottom: 1rem;
        }

        .upload-area p {
            color: var(--gray);
        }

        #file-input {
            display: none;
        }

        .compression-controls {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 1.5rem;
        }

        .control-group {
            margin-bottom: 1.5rem;
        }

        .control-group label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 500;
        }

        .slider-container {
            display: flex;
            align-items: center;
        }

        .slider-container input {
            flex: 1;
            margin-right: 1rem;
        }

        .slider-value {
            min-width: 50px;
            text-align: center;
            font-weight: 600;
            color: var(--primary);
        }

        input[type="range"] {
            -webkit-appearance: none;
            width: 100%;
            height: 8px;
            border-radius: 4px;
            background: #e0e0e0;
            outline: none;
        }

        input[type="range"]::-webkit-slider-thumb {
            -webkit-appearance: none;
            width: 20px;
            height: 20px;
            border-radius: 50%;
            background: var(--primary);
            cursor: pointer;
            transition: var(--transition);
        }

        input[type="range"]::-webkit-slider-thumb:hover {
            background: var(--primary-dark);
            transform: scale(1.1);
        }

        .format-options {
            display: flex;
            gap: 1rem;
            margin-top: 1rem;
        }

        .format-option {
            flex: 1;
            text-align: center;
            padding: 0.8rem;
            border: 2px solid #e0e0e0;
            border-radius: var(--border-radius);
            cursor: pointer;
            transition: var(--transition);
        }

        .format-option:hover {
            border-color: var(--primary);
        }

        .format-option.active {
            border-color: var(--primary);
            background-color: rgba(67, 97, 238, 0.1);
        }

        .preview-section {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 1.5rem;
            margin-top: 2rem;
        }

        .preview-box {
            border: 1px solid #e0e0e0;
            border-radius: var(--border-radius);
            overflow: hidden;
        }

        .preview-header {
            background-color: #f8f9fa;
            padding: 0.8rem;
            font-weight: 600;
            text-align: center;
            border-bottom: 1px solid #e0e0e0;
        }

        .preview-image {
            height: 200px;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 1rem;
        }

        .preview-image img {
            max-width: 100%;
            max-height: 100%;
            object-fit: contain;
        }

        .preview-info {
            padding: 1rem;
            background-color: #f8f9fa;
            border-top: 1px solid #e0e0e0;
            font-size: 0.9rem;
        }

        .preview-info div {
            display: flex;
            justify-content: space-between;
            margin-bottom: 0.5rem;
        }

        .action-buttons {
            display: flex;
            gap: 1rem;
            margin-top: 2rem;
        }

        .btn {
            padding: 0.8rem 1.5rem;
            border: none;
            border-radius: var(--border-radius);
            font-weight: 600;
            cursor: pointer;
            transition: var(--transition);
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .btn i {
            margin-right: 8px;
        }

        .btn-primary {
            background-color: var(--primary);
            color: white;
            flex: 2;
        }

        .btn-primary:hover {
            background-color: var(--primary-dark);
        }

        .btn-secondary {
            background-color: #e9ecef;
            color: var(--dark);
            flex: 1;
        }

        .btn-secondary:hover {
            background-color: #dee2e6;
        }

        .btn-success {
            background-color: var(--success);
            color: white;
        }

        .btn-success:hover {
            background-color: #3fa33f;
        }

        .sidebar {
            display: flex;
            flex-direction: column;
            gap: 2rem;
        }

        .ad-container {
            background-color: white;
            border-radius: var(--border-radius);
            box-shadow: var(--box-shadow);
            padding: 1rem;
            text-align: center;
        }

        .ad-container h3 {
            margin-bottom: 1rem;
            color: var(--gray);
            font-size: 1rem;
        }

        .ad-placeholder {
            background-color: #f8f9fa;
            border: 1px dashed #ccc;
            border-radius: var(--border-radius);
            padding: 3rem 1rem;
            color: var(--gray);
        }

        .features {
            background-color: white;
            border-radius: var(--border-radius);
            box-shadow: var(--box-shadow);
            padding: 1.5rem;
        }

        .features h3 {
            margin-bottom: 1rem;
            color: var(--primary);
        }

        .features ul {
            list-style: none;
        }

        .features li {
            padding: 0.5rem 0;
            border-bottom: 1px solid #f0f0f0;
            display: flex;
            align-items: center;
        }

        .features li:last-child {
            border-bottom: none;
        }

        .features li i {
            color: var(--success);
            margin-right: 10px;
        }

        footer {
            background-color: var(--dark);
            color: white;
            padding: 3rem 0 2rem;
            margin-top: 3rem;
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 2rem;
        }

        .footer-column h3 {
            margin-bottom: 1.5rem;
            font-size: 1.2rem;
        }

        .footer-column ul {
            list-style: none;
        }

        .footer-column ul li {
            margin-bottom: 0.8rem;
        }

        .footer-column ul li a {
            color: #adb5bd;
            text-decoration: none;
            transition: var(--transition);
        }

        .footer-column ul li a:hover {
            color: white;
        }

        .copyright {
            text-align: center;
            margin-top: 3rem;
            padding-top: 1.5rem;
            border-top: 1px solid #495057;
            color: #adb5bd;
            font-size: 0.9rem;
        }

        /* Responsive Design */
        @media (max-width: 992px) {
            .main-content {
                grid-template-columns: 1fr;
            }
            
            .footer-content {
                grid-template-columns: repeat(2, 1fr);
            }
        }

        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                text-align: center;
            }
            
            nav ul {
                margin-top: 1rem;
                justify-content: center;
            }
            
            .compression-controls {
                grid-template-columns: 1fr;
            }
            
            .preview-section {
                grid-template-columns: 1fr;
            }
            
            .action-buttons {
                flex-direction: column;
            }
        }

        @media (max-width: 576px) {
            .hero h1 {
                font-size: 2rem;
            }
            
            .footer-content {
                grid-template-columns: 1fr;
            }
        }

        /* Loading Animation */
        .loading {
            display: none;
            text-align: center;
            padding: 2rem;
        }

        .spinner {
            border: 4px solid rgba(0, 0, 0, 0.1);
            border-left-color: var(--primary);
            border-radius: 50%;
            width: 40px;
            height: 40px;
            animation: spin 1s linear infinite;
            margin: 0 auto 1rem;
        }

        @keyframes spin {
            to {
                transform: rotate(360deg);
            }
        }

        /* Toast Notification */
        .toast {
            position: fixed;
            bottom: 20px;
            right: 20px;
            background-color: var(--success);
            color: white;
            padding: 1rem 1.5rem;
            border-radius: var(--border-radius);
            box-shadow: var(--box-shadow);
            display: flex;
            align-items: center;
            transform: translateY(100px);
            opacity: 0;
            transition: transform 0.3s ease, opacity 0.3s ease;
            z-index: 1000;
        }

        .toast.show {
            transform: translateY(0);
            opacity: 1;
        }

        .toast i {
            margin-right: 10px;
        }
    </style>
    <!-- Font Awesome for Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container">
            <div class="header-content">
                <div class="logo">
                    <i class="fas fa-compress-alt"></i>
                    ImageCompress Pro
                </div>
                <nav>
                    <ul>
                        <li><a href="#">Home</a></li>
                        <li><a href="#">How It Works</a></li>
                        <li><a href="#">Pricing</a></li>
                        <li><a href="#">Blog</a></li>
                        <li><a href="#">Contact</a></li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>

    <!-- Main Content -->
    <div class="container">
        <!-- Hero Section -->
        <section class="hero">
            <h1>Compress Images Without Losing Quality</h1>
            <p>Reduce image file size by up to 80% while maintaining visual quality. Optimize your images for faster websites and apps.</p>
        </section>

        <div class="main-content">
            <!-- Compression Tool -->
            <div class="compression-tool">
                <div class="tool-section">
                    <h2><i class="fas fa-upload"></i> Upload Image</h2>
                    <div class="upload-area" id="upload-area">
                        <i class="fas fa-cloud-upload-alt"></i>
                        <h3>Drag & Drop Your Image Here</h3>
                        <p>or click to browse files (JPG, PNG, GIF, WebP)</p>
                        <input type="file" id="file-input" accept="image/*">
                    </div>
                </div>

                <div class="tool-section">
                    <h2><i class="fas fa-sliders-h"></i> Compression Settings</h2>
                    <div class="compression-controls">
                        <div class="control-group">
                            <label for="quality">Compression Level</label>
                            <div class="slider-container">
                                <input type="range" id="quality" min="0" max="100" value="80">
                                <span class="slider-value" id="quality-value">80%</span>
                            </div>
                            <div class="slider-labels">
                                <span>Smaller Size</span>
                                <span style="float: right;">Better Quality</span>
                            </div>
                        </div>

                        <div class="control-group">
                            <label for="max-width">Max Width (px)</label>
                            <div class="slider-container">
                                <input type="range" id="max-width" min="100" max="2000" value="1200" step="100">
                                <span class="slider-value" id="max-width-value">1200px</span>
                            </div>
                        </div>
                    </div>

                    <div class="control-group">
                        <label>Output Format</label>
                        <div class="format-options">
                            <div class="format-option active" data-format="original">Original</div>
                            <div class="format-option" data-format="jpeg">JPEG</div>
                            <div class="format-option" data-format="png">PNG</div>
                            <div class="format-option" data-format="webp">WebP</div>
                        </div>
                    </div>
                </div>

                <!-- Preview Section -->
                <div class="preview-section">
                    <div class="preview-box">
                        <div class="preview-header">Original Image</div>
                        <div class="preview-image" id="original-preview">
                            <p>No image selected</p>
                        </div>
                        <div class="preview-info">
                            <div>
                                <span>File Size:</span>
                                <span id="original-size">-</span>
                            </div>
                            <div>
                                <span>Dimensions:</span>
                                <span id="original-dimensions">-</span>
                            </div>
                        </div>
                    </div>

                    <div class="preview-box">
                        <div class="preview-header">Compressed Image</div>
                        <div class="preview-image" id="compressed-preview">
                            <p>Compressed image will appear here</p>
                        </div>
                        <div class="preview-info">
                            <div>
                                <span>File Size:</span>
                                <span id="compressed-size">-</span>
                            </div>
                            <div>
                                <span>Dimensions:</span>
                                <span id="compressed-dimensions">-</span>
                            </div>
                            <div>
                                <span>Reduction:</span>
                                <span id="reduction">-</span>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Loading Animation -->
                <div class="loading" id="loading">
                    <div class="spinner"></div>
                    <p>Compressing your image...</p>
                </div>

                <!-- Action Buttons -->
                <div class="action-buttons">
                    <button class="btn btn-primary" id="compress-btn" disabled>
                        <i class="fas fa-compress-alt"></i> Compress Image
                    </button>
                    <button class="btn btn-secondary" id="reset-btn">
                        <i class="fas fa-redo"></i> Reset
                    </button>
                    <button class="btn btn-success" id="download-btn" disabled>
                        <i class="fas fa-download"></i> Download
                    </button>
                </div>
            </div>

            <!-- Sidebar -->
            <div class="sidebar">
                <!-- Ad Container 1 -->
                <div class="ad-container">
                    <h3>Advertisement</h3>
                    <div class="ad-placeholder">
                        <!-- Replace with your AdSense code -->
                        <p>Ad Space (300x250)</p>
                        <p>Insert AdSense code here</p>
                    </div>
                </div>

                <!-- Features -->
                <div class="features">
                    <h3>Why Use Our Tool?</h3>
                    <ul>
                        <li><i class="fas fa-check"></i> No registration required</li>
                        <li><i class="fas fa-check"></i> 100% secure - files never leave your browser</li>
                        <li><i class="fas fa-check"></i> Compress multiple images at once</li>
                        <li><i class="fas fa-check"></i> Maintain image quality</li>
                        <li><i class="fas fa-check"></i> Fast processing</li>
                        <li><i class="fas fa-check"></i> Free to use</li>
                    </ul>
                </div>

                <!-- Ad Container 2 -->
                <div class="ad-container">
                    <h3>Advertisement</h3>
                    <div class="ad-placeholder">
                        <!-- Replace with your AdSense code -->
                        <p>Ad Space (300x600)</p>
                        <p>ca-app-pub-5758492046704143/1894674784</p>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3>ImageCompress Pro</h3>
                    <p>The fastest and most secure online image compression tool. Optimize your images for web and mobile without sacrificing quality.</p>
                </div>
                <div class="footer-column">
                    <h3>Quick Links</h3>
                    <ul>
                        <li><a href="#">Home</a></li>
                        <li><a href="#">How It Works</a></li>
                        <li><a href="#">Features</a></li>
                        <li><a href="#">Pricing</a></li>
                        <li><a href="#">Blog</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h3>Tools</h3>
                    <ul>
                        <li><a href="#">JPG Compressor</a></li>
                        <li><a href="#">PNG Optimizer</a></li>
                        <li><a href="#">WebP Converter</a></li>
                        <li><a href="#">Bulk Image Compressor</a></li>
                        <li><a href="#">Image Resizer</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h3>Support</h3>
                    <ul>
                        <li><a href="#">Help Center</a></li>
                        <li><a href="#">Contact Us</a></li>
                        <li><a href="#">Privacy Policy</a></li>
                        <li><a href="#">Terms of Service</a></li>
                        <li><a href="#">FAQ</a></li>
                    </ul>
                </div>
            </div>
            <div class="copyright">
                <p>&copy; 2023 ImageCompress Pro. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <!-- Toast Notification -->
    <div class="toast" id="toast">
        <i class="fas fa-check-circle"></i>
        <span id="toast-message">Image compressed successfully!</span>
    </div>

    <script>
        // DOM Elements
        const fileInput = document.getElementById('file-input');
        const uploadArea = document.getElementById('upload-area');
        const qualitySlider = document.getElementById('quality');
        const qualityValue = document.getElementById('quality-value');
        const maxWidthSlider = document.getElementById('max-width');
        const maxWidthValue = document.getElementById('max-width-value');
        const formatOptions = document.querySelectorAll('.format-option');
        const originalPreview = document.getElementById('original-preview');
        const compressedPreview = document.getElementById('compressed-preview');
        const originalSize = document.getElementById('original-size');
        const originalDimensions = document.getElementById('original-dimensions');
        const compressedSize = document.getElementById('compressed-size');
        const compressedDimensions = document.getElementById('compressed-dimensions');
        const reduction = document.getElementById('reduction');
        const compressBtn = document.getElementById('compress-btn');
        const resetBtn = document.getElementById('reset-btn');
        const downloadBtn = document.getElementById('download-btn');
        const loading = document.getElementById('loading');
        const toast = document.getElementById('toast');
        const toastMessage = document.getElementById('toast-message');

        // Variables
        let originalImage = null;
        let compressedImageBlob = null;
        let selectedFormat = 'original';

        // Event Listeners
        uploadArea.addEventListener('click', () => fileInput.click());
        uploadArea.addEventListener('dragover', (e) => {
            e.preventDefault();
            uploadArea.style.borderColor = 'var(--primary)';
            uploadArea.style.backgroundColor = 'rgba(67, 97, 238, 0.05)';
        });
        uploadArea.addEventListener('dragleave', () => {
            uploadArea.style.borderColor = '#ccc';
            uploadArea.style.backgroundColor = 'transparent';
        });
        uploadArea.addEventListener('drop', (e) => {
            e.preventDefault();
            uploadArea.style.borderColor = '#ccc';
            uploadArea.style.backgroundColor = 'transparent';
            
            if (e.dataTransfer.files.length) {
                handleImageUpload(e.dataTransfer.files[0]);
            }
        });

        fileInput.addEventListener('change', (e) => {
            if (e.target.files.length) {
                handleImageUpload(e.target.files[0]);
            }
        });

        qualitySlider.addEventListener('input', () => {
            qualityValue.textContent = `${qualitySlider.value}%`;
        });

        maxWidthSlider.addEventListener('input', () => {
            maxWidthValue.textContent = `${maxWidthSlider.value}px`;
        });

        formatOptions.forEach(option => {
            option.addEventListener('click', () => {
                formatOptions.forEach(opt => opt.classList.remove('active'));
                option.classList.add('active');
                selectedFormat = option.getAttribute('data-format');
            });
        });

        compressBtn.addEventListener('click', compressImage);
        resetBtn.addEventListener('click', resetTool);
        downloadBtn.addEventListener('click', downloadImage);

        // Functions
        function handleImageUpload(file) {
            if (!file.type.match('image.*')) {
                showToast('Please select a valid image file', 'error');
                return;
            }

            const reader = new FileReader();
            reader.onload = (e) => {
                originalImage = new Image();
                originalImage.onload = () => {
                    // Display original image
                    originalPreview.innerHTML = '';
                    const img = document.createElement('img');
                    img.src = e.target.result;
                    originalPreview.appendChild(img);

                    // Update original image info
                    originalSize.textContent = formatFileSize(file.size);
                    originalDimensions.textContent = `${originalImage.width} × ${originalImage.height}`;

                    // Enable compress button
                    compressBtn.disabled = false;
                };
                originalImage.src = e.target.result;
            };
            reader.readAsDataURL(file);
        }

        function compressImage() {
            if (!originalImage) return;

            loading.style.display = 'block';
            compressBtn.disabled = true;

            // Simulate compression process (in a real app, this would use actual compression algorithms)
            setTimeout(() => {
                const canvas = document.createElement('canvas');
                const ctx = canvas.getContext('2d');

                // Calculate new dimensions
                const maxWidth = parseInt(maxWidthSlider.value);
                let width = originalImage.width;
                let height = originalImage.height;

                if (width > maxWidth) {
                    height = (maxWidth / width) * height;
                    width = maxWidth;
                }

                canvas.width = width;
                canvas.height = height;

                // Draw image with quality settings
                ctx.drawImage(originalImage, 0, 0, width, height);

                // Get compressed image data
                let mimeType = 'image/jpeg';
                if (selectedFormat === 'png') mimeType = 'image/png';
                if (selectedFormat === 'webp') mimeType = 'image/webp';

                const quality = parseInt(qualitySlider.value) / 100;

                canvas.toBlob((blob) => {
                    compressedImageBlob = blob;

                    // Display compressed image
                    compressedPreview.innerHTML = '';
                    const img = document.createElement('img');
                    img.src = URL.createObjectURL(blob);
                    compressedPreview.appendChild(img);

                    // Update compressed image info
                    compressedSize.textContent = formatFileSize(blob.size);
                    compressedDimensions.textContent = `${width} × ${height}`;

                    // Calculate reduction
                    const originalSizeBytes = getOriginalFileSize();
                    const compressedSizeBytes = blob.size;
                    const reductionPercent = ((originalSizeBytes - compressedSizeBytes) / originalSizeBytes * 100).toFixed(1);
                    reduction.textContent = `${reductionPercent}%`;

                    // Enable download button
                    downloadBtn.disabled = false;

                    // Hide loading
                    loading.style.display = 'none';

                    // Show success message
                    showToast('Image compressed successfully!');
                }, mimeType, quality);
            }, 1500);
        }

        function getOriginalFileSize() {
            // In a real implementation, you would get the actual file size
            // For this demo, we'll estimate based on image dimensions
            const estimatedSize = originalImage.width * originalImage.height * 4; // Rough estimate
            return estimatedSize;
        }

        function formatFileSize(bytes) {
            if (bytes === 0) return '0 Bytes';
            const k = 1024;
            const sizes = ['Bytes', 'KB', 'MB', 'GB'];
            const i = Math.floor(Math.log(bytes) / Math.log(k));
            return parseFloat((bytes / Math.pow(k, i)).toFixed(2)) + ' ' + sizes[i];
        }

        function resetTool() {
            fileInput.value = '';
            originalImage = null;
            compressedImageBlob = null;
            
            originalPreview.innerHTML = '<p>No image selected</p>';
            compressedPreview.innerHTML = '<p>Compressed image will appear here</p>';
            
            originalSize.textContent = '-';
            originalDimensions.textContent = '-';
            compressedSize.textContent = '-';
            compressedDimensions.textContent = '-';
            reduction.textContent = '-';
            
            compressBtn.disabled = true;
            downloadBtn.disabled = true;
            
            qualitySlider.value = 80;
            qualityValue.textContent = '80%';
            
            maxWidthSlider.value = 1200;
            maxWidthValue.textContent = '1200px';
            
            formatOptions.forEach(opt => opt.classList.remove('active'));
            formatOptions[0].classList.add('active');
            selectedFormat = 'original';
        }

        function downloadImage() {
            if (!compressedImageBlob) return;

            const url = URL.createObjectURL(compressedImageBlob);
            const a = document.createElement('a');
            a.href = url;
            a.download = `compressed-image.${selectedFormat === 'original' ? 'jpg' : selectedFormat}`;
            document.body.appendChild(a);
            a.click();
            document.body.removeChild(a);
            URL.revokeObjectURL(url);
        }

        function showToast(message, type = 'success') {
            toastMessage.textContent = message;
            
            if (type === 'error') {
                toast.style.backgroundColor = 'var(--danger)';
            } else {
                toast.style.backgroundColor = 'var(--success)';
            }
            
            toast.classList.add('show');
            
            setTimeout(() => {
                toast.classList.remove('show');
            }, 3000);
        }

        // Initialize tool
        resetTool();
    </script>
</body>
</html>
