<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Colorful Invoice Generator</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/pdfmake@0.2.7/build/pdfmake.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/pdfmake@0.2.7/build/vfs_fonts.js"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary: #6c5ce7;
            --secondary: #a29bfe;
            --accent1: #fd79a8;
            --accent2: #00cec9;
            --accent3: #fdcb6e;
            --light: #f8f9fa;
            --dark: #2d3436;
            --success: #00b894;
            --danger: #d63031;
            --transition: all 0.3s ease;
        }
        
        body {
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            color: var(--dark);
            min-height: 100vh;
            padding-bottom: 2rem;
        }
        
        .header {
            background: linear-gradient(120deg, var(--primary), var(--accent2));
            color: white;
            border-radius: 0 0 20px 20px;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.15);
            padding: 1.5rem 0;
            margin-bottom: 2rem;
        }
        
        .card {
            border: none;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            margin-bottom: 2rem;
            transition: transform 0.3s ease;
        }
        
        .card:hover {
            transform: translateY(-5px);
        }
        
        .card-header {
            background: linear-gradient(120deg, var(--primary), var(--secondary));
            color: white;
            padding: 1.2rem 1.5rem;
            border-bottom: none;
        }
        
        .section-title {
            border-bottom: 3px solid var(--accent1);
            padding-bottom: 10px;
            margin: 20px 0;
            color: var(--primary);
            font-weight: 600;
        }
        
        .item-row {
            margin-bottom: 10px;
            padding-bottom: 10px;
            border-bottom: 1px dashed #e0e0e0;
            transition: background-color 0.2s;
        }
        
        .item-row:hover {
            background-color: rgba(162, 155, 254, 0.05);
        }
        
        .totals-box {
            background: linear-gradient(135deg, #f6d365 0%, #fda085 100%);
            padding: 20px;
            border-radius: 10px;
            margin-top: 20px;
            color: white;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
        .btn-primary {
            background: linear-gradient(120deg, var(--primary), var(--secondary));
            border: none;
            border-radius: 50px;
            padding: 10px 25px;
            font-weight: 600;
            box-shadow: 0 4px 15px rgba(108, 92, 231, 0.3);
            transition: var(--transition);
        }
        
        .btn-primary:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 20px rgba(108, 92, 231, 0.4);
            background: linear-gradient(120deg, var(--secondary), var(--primary));
        }
        
        .btn-success {
            background: linear-gradient(120deg, var(--success), #00a896);
            border: none;
            border-radius: 50px;
            padding: 10px 25px;
            font-weight: 600;
            box-shadow: 0 4px 15px rgba(0, 184, 148, 0.3);
            transition: var(--transition);
        }
        
        .btn-success:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 20px rgba(0, 184, 148, 0.4);
        }
        
        .btn-info {
            background: linear-gradient(120deg, #74b9ff, #0984e3);
            border: none;
            border-radius: 50px;
            padding: 10px 25px;
            font-weight: 600;
            box-shadow: 0 4px 15px rgba(116, 185, 255, 0.3);
            transition: var(--transition);
        }
        
        .btn-info:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 20px rgba(116, 185, 255, 0.4);
        }
        
        .btn-secondary {
            background: linear-gradient(120deg, #636e72, #b2bec3);
            border: none;
            border-radius: 50px;
            padding: 10px 25px;
            font-weight: 600;
            box-shadow: 0 4px 15px rgba(99, 110, 114, 0.3);
            transition: var(--transition);
        }
        
        .btn-secondary:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 20px rgba(99, 110, 114, 0.4);
        }
        
        .form-control {
            border-radius: 10px;
            padding: 12px 15px;
            border: 2px solid #e0e0e0;
            transition: var(--transition);
        }
        
        .form-control:focus {
            border-color: var(--primary);
            box-shadow: 0 0 0 0.25rem rgba(108, 92, 231, 0.25);
        }
        
        .invoice-preview {
            border: none;
            padding: 25px;
            margin-top: 20px;
            background: linear-gradient(135deg, #f0f2f5 0%, #e6e9ef 100%);
            border-radius: 15px;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.1);
        }
        
        .gradient-bg {
            background: linear-gradient(120deg, var(--accent1), var(--accent3));
            color: white;
            padding: 8px 15px;
            border-radius: 8px;
            text-align: center;
        }
        
        .floating-btn {
            position: fixed;
            bottom: 30px;
            right: 30px;
            width: 60px;
            height: 60px;
            border-radius: 50%;
            background: linear-gradient(120deg, var(--primary), var(--secondary));
            color: white;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 24px;
            box-shadow: 0 6px 20px rgba(108, 92, 231, 0.4);
            z-index: 100;
            animation: pulse 2s infinite;
            text-decoration: none;
            transition: var(--transition);
        }
        
        .floating-btn:hover {
            transform: scale(1.1);
        }
        
        @keyframes pulse {
            0% {
                transform: scale(1);
                box-shadow: 0 6px 20px rgba(108, 92, 231, 0.4);
            }
            50% {
                transform: scale(1.1);
                box-shadow: 0 9px 25px rgba(108, 92, 231, 0.6);
            }
            100% {
                transform: scale(1);
                box-shadow: 0 6px 20px rgba(108, 92, 231, 0.4);
            }
        }
        
        .feature-icon {
            background: linear-gradient(120deg, var(--primary), var(--secondary));
            color: white;
            width: 40px;
            height: 40px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-right: 10px;
        }
        
        .feature-list {
            background: rgba(255, 255, 255, 0.7);
            border-radius: 15px;
            padding: 20px;
            margin-bottom: 20px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
        }
        
        /* Toast notification */
        .toast-container {
            position: fixed;
            top: 20px;
            right: 20px;
            z-index: 9999;
        }
        
        .toast {
            background: white;
            border-left: 5px solid var(--success);
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
            border-radius: 8px;
            padding: 15px 20px;
            margin-bottom: 10px;
            display: flex;
            align-items: center;
            transform: translateX(100%);
            opacity: 0;
            transition: transform 0.3s ease, opacity 0.3s ease;
        }
        
        .toast.show {
            transform: translateX(0);
            opacity: 1;
        }
        
        .toast.error {
            border-left-color: var(--danger);
        }
        
        .toast-icon {
            margin-right: 10px;
            font-size: 20px;
        }
        
        /* Loading spinner */
        .spinner {
            width: 40px;
            height: 40px;
            border: 4px solid rgba(0, 0, 0, 0.1);
            border-radius: 50%;
            border-top: 4px solid var(--primary);
            animation: spin 1s linear infinite;
            margin: 0 auto;
        }
        
        @keyframes spin {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }
        
        /* Print styles */
        @media print {
            body * {
                visibility: hidden;
            }
            #invoicePreview, #invoicePreview * {
                visibility: visible;
            }
            #invoicePreview {
                position: absolute;
                left: 0;
                top: 0;
                width: 100%;
            }
        }
        
        /* Responsive adjustments */
        @media (max-width: 768px) {
            .btn {
                width: 100%;
                margin-bottom: 10px;
            }
            
            .btn-group .btn {
                width: auto;
            }
            
            .floating-btn {
                bottom: 20px;
                right: 20px;
                width: 50px;
                height: 50px;
                font-size: 20px;
            }
        }
    </style>
</head>
<body>
    <!-- Toast container -->
    <div class="toast-container" id="toastContainer"></div>

    <!-- Header -->
    <div class="header">
        <div class="container text-center">
            <h1><i class="fas fa-receipt me-2"></i>Colorful Invoice Generator</h1>
            <p class="lead">Create beautiful, professional invoices in minutes</p>
        </div>
    </div>

    <div class="container">
        <div class="row">
            <div class="col-lg-8">
                <!-- Invoice Form -->
                <div class="card shadow">
                    <div class="card-header">
                        <h3 class="mb-0"><i class="fas fa-pencil-alt me-2"></i>Create New Invoice</h3>
                    </div>
                    <div class="card-body">
                        <form id="invoiceForm">
                            <div class="row">
                                <div class="col-md-6">
                                    <h4 class="section-title"><i class="fas fa-building me-2"></i>Sender Information</h4>
                                    <div class="mb-3">
                                        <label class="form-label">Business Name</label>
                                        <input type="text" class="form-control" id="businessName" value="Your Business Name" required>
                                    </div>
                                    <div class="mb-3">
                                        <label class="form-label">Address</label>
                                        <textarea class="form-control" id="businessAddress" rows="2" required>123 Business St, City, Country</textarea>
                                    </div>
                                    <div class="row">
                                        <div class="col-md-6 mb-3">
                                            <label class="form-label">Email</label>
                                            <input type="email" class="form-control" id="businessEmail" value="contact@yourbusiness.com" required>
                                        </div>
                                        <div class="col-md-6 mb-3">
                                            <label class="form-label">Phone</label>
                                            <input type="tel" class="form-control" id="businessPhone" value="+1 (555) 123-4567" required>
                                        </div>
                                    </div>
                                </div>
                                
                                <div class="col-md-6">
                                    <h4 class="section-title"><i class="fas fa-user me-2"></i>Client Information</h4>
                                    <div class="mb-3">
                                        <label class="form-label">Client Name</label>
                                        <input type="text" class="form-control" id="clientName" placeholder="Enter client name" required>
                                    </div>
                                    <div class="mb-3">
                                        <label class="form-label">Address</label>
                                        <textarea class="form-control" id="clientAddress" rows="2" placeholder="Enter client address" required></textarea>
                                    </div>
                                    <div class="row">
                                        <div class="col-md-6 mb-3">
                                            <label class="form-label">Email</label>
                                            <input type="email" class="form-control" id="clientEmail" placeholder="Enter client email" required>
                                        </div>
                                        <div class="col-md-6 mb-3">
                                            <label class="form-label">Phone</label>
                                            <input type="tel" class="form-control" id="clientPhone" placeholder="Enter client phone" required>
                                        </div>
                                    </div>
                                </div>
                            </div>
                            
                            <h4 class="section-title"><i class="fas fa-file-invoice me-2"></i>Invoice Details</h4>
                            <div class="row">
                                <div class="col-md-3 mb-3">
                                    <label class="form-label">Invoice Number</label>
                                    <input type="text" class="form-control" id="invoiceNumber" value="INV-001" required>
                                </div>
                                <div class="col-md-3 mb-3">
                                    <label class="form-label">Invoice Date</label>
                                    <input type="date" class="form-control" id="invoiceDate" required>
                                </div>
                                <div class="col-md-3 mb-3">
                                    <label class="form-label">Due Date</label>
                                    <input type="date" class="form-control" id="dueDate" required>
                                </div>
                                <div class="col-md-3 mb-3">
                                    <label class="form-label">Currency</label>
                                    <select class="form-select" id="currency">
                                        <option value="USD">USD ($)</option>
                                        <option value="EUR">EUR (€)</option>
                                        <option value="GBP">GBP (£)</option>
                                        <option value="JPY">JPY (¥)</option>
                                    </select>
                                </div>
                            </div>
                            
                            <h4 class="section-title"><i class="fas fa-list me-2"></i>Items</h4>
                            <div id="itemsContainer">
                                <div class="item-row">
                                    <div class="row">
                                        <div class="col-md-5 mb-2">
                                            <input type="text" class="form-control" placeholder="Description" required>
                                        </div>
                                        <div class="col-md-2 mb-2">
                                            <input type="number" class="form-control quantity" placeholder="Qty" min="1" value="1" required>
                                        </div>
                                        <div class="col-md-2 mb-2">
                                            <input type="number" class="form-control price" placeholder="Price" min="0" step="0.01" required>
                                        </div>
                                        <div class="col-md-2 mb-2">
                                            <input type="text" class="form-control item-total" value="0.00" readonly>
                                        </div>
                                        <div class="col-md-1 mb-2">
                                            <button type="button" class="btn btn-danger remove-item"><i class="fas fa-times"></i></button>
                                        </div>
                                    </div>
                                </div>
                            </div>
                            
                            <div class="row mt-3">
                                <div class="col-12">
                                    <button type="button" id="addItem" class="btn btn-secondary"><i class="fas fa-plus me-2"></i>Add Item</button>
                                </div>
                            </div>
                            
                            <div class="row mt-4">
                                <div class="col-md-6">
                                    <div class="mb-3">
                                        <label class="form-label">Notes/Terms</label>
                                        <textarea class="form-control" id="notes" rows="3">Thank you for your business!</textarea>
                                    </div>
                                </div>
                                
                                <div class="col-md-6">
                                    <div class="totals-box">
                                        <div class="row mb-2">
                                            <div class="col-6">Subtotal:</div>
                                            <div class="col-6 text-end" id="subtotal">$0.00</div>
                                        </div>
                                        <div class="row mb-2">
                                            <div class="col-6">
                                                <label class="form-label">Tax Rate (%)</label>
                                            </div>
                                            <div class="col-6">
                                                <input type="number" class="form-control" id="taxRate" value="10" min="0" step="0.1">
                                            </div>
                                        </div>
                                        <div class="row mb-2">
                                            <div class="col-6">Tax Amount:</div>
                                            <div class="col-6 text-end" id="taxAmount">$0.00</div>
                                        </div>
                                        <div class="row mb-2">
                                            <div class="col-6">
                                                <label class="form-label">Discount</label>
                                            </div>
                                            <div class="col-6">
                                                <input type="number" class="form-control" id="discount" value="0" min="0" step="0.01">
                                            </div>
                                        </div>
                                        <div class="row mb-2">
                                            <div class="col-6">
                                                <strong>Total:</strong>
                                            </div>
                                            <div class="col-6 text-end">
                                                <strong id="total">$0.00</strong>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                            
                            <div class="row mt-4">
                                <div class="col-12 text-center">
                                    <div class="btn-group" role="group">
                                        <button type="button" id="previewInvoice" class="btn btn-info me-2"><i class="fas fa-eye me-2"></i>Preview</button>
                                        <button type="button" id="downloadPdf" class="btn btn-success me-2"><i class="fas fa-download me-2"></i>PDF</button>
                                        <button type="button" id="printInvoice" class="btn btn-primary me-2"><i class="fas fa-print me-2"></i>Print</button>
                                        <button type="reset" class="btn btn-secondary me-2"><i class="fas fa-redo me-2"></i>Reset</button>
                                        <button type="button" id="saveInvoice" class="btn btn-primary"><i class="fas fa-save me-2"></i>Save</button>
                                    </div>
                                </div>
                            </div>
                        </form>
                    </div>
                </div>
                
                <!-- Invoice Preview -->
                <div class="invoice-preview mt-5" id="invoicePreview" style="display: none;">
                    <div class="d-flex justify-content-between align-items-center mb-3">
                        <h3 class="gradient-bg mb-0"><i class="fas fa-file-invoice me-2"></i>Invoice Preview</h3>
                        <button type="button" id="hidePreview" class="btn btn-secondary"><i class="fas fa-times me-2"></i>Hide Preview</button>
                    </div>
                    <div id="previewContent"></div>
                </div>
            </div>
            
            <div class="col-lg-4">
                <!-- Features Card -->
                <div class="feature-list">
                    <h4 class="section-title"><i class="fas fa-star me-2"></i>Why Use Our Invoice Generator?</h4>
                    <div class="d-flex mb-3">
                        <div class="feature-icon">
                            <i class="fas fa-bolt"></i>
                        </div>
                        <div>
                            <h5>Quick & Easy</h5>
                            <p class="mb-0">Create professional invoices in minutes</p>
                        </div>
                    </div>
                    <div class="d-flex mb-3">
                        <div class="feature-icon">
                            <i class="fas fa-palette"></i>
                        </div>
                        <div>
                            <h5>Beautiful Design</h5>
                            <p class="mb-0">Impress your clients with stylish invoices</p>
                        </div>
                    </div>
                    <div class="d-flex mb-3">
                        <div class="feature-icon">
                            <i class="fas fa-calculator"></i>
                        </div>
                        <div>
                            <h5>Auto Calculations</h5>
                            <p class="mb-0">Automatic totals, tax and discount calculations</p>
                        </div>
                    </div>
                    <div class="d-flex">
                        <div class="feature-icon">
                            <i class="fas fa-file-pdf"></i>
                        </div>
                        <div>
                            <h5>PDF Export</h5>
                            <p class="mb-0">Download or print your invoices as PDF</p>
                        </div>
                    </div>
                </div>
                
                <!-- Tips Card -->
                <div class="card">
                    <div class="card-header">
                        <h4 class="mb-0"><i class="fas fa-lightbulb me-2"></i>Pro Tips</h4>
                    </div>
                    <div class="card-body">
                        <ul class="list-group list-group-flush">
                            <li class="list-group-item">Add your logo for brand recognition</li>
                            <li class="list-group-item">Use clear item descriptions</li>
                            <li class="list-group-item">Set reasonable payment terms</li>
                            <li class="list-group-item">Send invoices promptly</li>
                            <li class="list-group-item">Follow up on overdue payments</li>
                        </ul>
                    </div>
                </div>
                
                <!-- Stats Card -->
                <div class="card">
                    <div class="card-header">
                        <h4 class="mb-0"><i class="fas fa-chart-line me-2"></i>Invoice Stats</h4>
                    </div>
                    <div class="card-body">
                        <div class="text-center">
                            <div class="gradient-bg mb-3">
                                <h2 id="invoicesCreated">127</h2>
                                <p class="mb-0">Invoices Created</p>
                            </div>
                            <div class="gradient-bg mb-3">
                                <h2 id="totalRevenue">$42.8K</h2>
                                <p class="mb-0">Total Revenue</p>
                            </div>
                            <div class="gradient-bg">
                                <h2 id="paidInvoices">94%</h2>
                                <p class="mb-0">Paid Invoices</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <a href="#" class="floating-btn" id="scrollToTop">
        <i class="fas fa-arrow-up"></i>
    </a>

    <script>
        // Invoice Manager Class
        class InvoiceManager {
            constructor() {
                this.invoices = JSON.parse(localStorage.getItem('invoices')) || [];
                this.currentInvoice = null;
                this.init();
            }
            
            init() {
                // Set default dates
                this.setDefaultDates();
                
                // Initialize event listeners
                this.initEventListeners();
                
                // Initialize calculations
                this.calculateTotals();
                
                // Update stats
                this.updateStats();
            }
            
            setDefaultDates() {
                document.getElementById('invoiceDate').valueAsDate = new Date();
                const dueDate = new Date();
                dueDate.setDate(dueDate.getDate() + 30);
                document.getElementById('dueDate').valueAsDate = dueDate;
            }
            
            initEventListeners() {
                // Add item row
                document.getElementById('addItem').addEventListener('click', () => this.addItemRow());
                
                // Remove item event delegation
                document.getElementById('itemsContainer').addEventListener('click', (e) => {
                    if (e.target.closest('.remove-item')) {
                        e.target.closest('.item-row').remove();
                        this.calculateTotals();
                    }
                });
                
                // Input event listeners
                document.querySelectorAll('.quantity, .price').forEach(input => {
                    input.addEventListener('input', (e) => this.calculateItemTotal(e.target));
                });
                
                document.getElementById('taxRate').addEventListener('input', () => this.calculateTotals());
                document.getElementById('discount').addEventListener('input', () => this.calculateTotals());
                document.getElementById('currency').addEventListener('change', () => this.calculateTotals());
                
                // Button event listeners
                document.getElementById('previewInvoice').addEventListener('click', () => this.previewInvoice());
                document.getElementById('hidePreview').addEventListener('click', () => this.hidePreview());
                document.getElementById('downloadPdf').addEventListener('click', () => this.downloadPdf());
                document.getElementById('printInvoice').addEventListener('click', () => this.printInvoice());
                document.getElementById('saveInvoice').addEventListener('click', () => this.saveInvoice());
                document.getElementById('scrollToTop').addEventListener('click', (e) => {
                    e.preventDefault();
                    window.scrollTo({ top: 0, behavior: 'smooth' });
                });
                
                // Form reset
                document.getElementById('invoiceForm').addEventListener('reset', () => {
                    setTimeout(() => {
                        this.setDefaultDates();
                        this.calculateTotals();
                    }, 0);
                });
            }
            
            addItemRow() {
                const itemsContainer = document.getElementById('itemsContainer');
                const newRow = document.createElement('div');
                newRow.className = 'item-row';
                newRow.innerHTML = `
                    <div class="row">
                        <div class="col-md-5 mb-2">
                            <input type="text" class="form-control" placeholder="Description" required>
                        </div>
                        <div class="col-md-2 mb-2">
                            <input type="number" class="form-control quantity" placeholder="Qty" min="1" value="1" required>
                        </div>
                        <div class="col-md-2 mb-2">
                            <input type="number" class="form-control price" placeholder="Price" min="0" step="0.01" required>
                        </div>
                        <div class="col-md-2 mb-2">
                            <input type="text" class="form-control item-total" value="0.00" readonly>
                        </div>
                        <div class="col-md-1 mb-2">
                            <button type="button" class="btn btn-danger remove-item"><i class="fas fa-times"></i></button>
                        </div>
                    </div>
                `;
                itemsContainer.appendChild(newRow);
                
                // Add event listeners to new inputs
                const quantityInput = newRow.querySelector('.quantity');
                const priceInput = newRow.querySelector('.price');
                
                quantityInput.addEventListener('input', (e) => this.calculateItemTotal(e.target));
                priceInput.addEventListener('input', (e) => this.calculateItemTotal(e.target));
            }
            
            calculateItemTotal(input) {
                const row = input.closest('.item-row');
                const quantity = parseFloat(row.querySelector('.quantity').value) || 0;
                const price = parseFloat(row.querySelector('.price').value) || 0;
                const total = quantity * price;
                row.querySelector('.item-total').value = total.toFixed(2);
                this.calculateTotals();
            }
            
            calculateTotals() {
                let subtotal = 0;
                document.querySelectorAll('.item-row').forEach(row => {
                    const total = parseFloat(row.querySelector('.item-total').value) || 0;
                    subtotal += total;
                });
                
                const taxRate = parseFloat(document.getElementById('taxRate').value) || 0;
                const discount = parseFloat(document.getElementById('discount').value) || 0;
                const taxAmount = subtotal * (taxRate / 100);
                const total = subtotal + taxAmount - discount;
                
                const currencySymbol = this.getCurrencySymbol();
                
                document.getElementById('subtotal').textContent = `${currencySymbol}${subtotal.toFixed(2)}`;
                document.getElementById('taxAmount').textContent = `${currencySymbol}${taxAmount.toFixed(2)}`;
                document.getElementById('total').textContent = `${currencySymbol}${total.toFixed(2)}`;
            }
            
            getCurrencySymbol() {
                const currency = document.getElementById('currency').value;
                switch(currency) {
                    case 'EUR': return '€';
                    case 'GBP': return '£';
                    case 'JPY': return '¥';
                    default: return '$';
                }
            }
            
            validateForm() {
                const requiredFields = document.querySelectorAll('#invoiceForm [required]');
                let isValid = true;
                
                requiredFields.forEach(field => {
                    if (!field.value.trim()) {
                        isValid = false;
                        field.classList.add('is-invalid');
                    } else {
                        field.classList.remove('is-invalid');
                    }
                });
                
                return isValid;
            }
            
            previewInvoice() {
                if (!this.validateForm()) {
                    this.showToast('Please fill all required fields', 'error');
                    return;
                }
                
                this.generatePreview();
                document.getElementById('invoicePreview').style.display = 'block';
                
                // Scroll to preview
                document.getElementById('invoicePreview').scrollIntoView({ behavior: 'smooth' });
            }
            
            hidePreview() {
                document.getElementById('invoicePreview').style.display = 'none';
            }
            
            generatePreview() {
                const businessName = document.getElementById('businessName').value;
                const businessAddress = document.getElementById('businessAddress').value;
                const businessEmail = document.getElementById('businessEmail').value;
                const businessPhone = document.getElementById('businessPhone').value;
                
                const clientName = document.getElementById('clientName').value;
                const clientAddress = document.getElementById('clientAddress').value;
                const clientEmail = document.getElementById('clientEmail').value;
                const clientPhone = document.getElementById('clientPhone').value;
                
                const invoiceNumber = document.getElementById('invoiceNumber').value;
                const invoiceDate = document.getElementById('invoiceDate').value;
                const dueDate = document.getElementById('dueDate').value;
                const notes = document.getElementById('notes').value;
                
                const currencySymbol = this.getCurrencySymbol();
                const subtotal = document.getElementById('subtotal').textContent;
                const taxAmount = document.getElementById('taxAmount').textContent;
                const total = document.getElementById('total').textContent;
                
                let itemsHTML = '';
                document.querySelectorAll('.item-row').forEach(row => {
                    const description = row.querySelector('input[type="text"]').value;
                    const quantity = row.querySelector('.quantity').value;
                    const price = row.querySelector('.price').value;
                    const itemTotal = row.querySelector('.item-total').value;
                    
                    itemsHTML += `
                        <tr>
                            <td>${description}</td>
                            <td class="text-center">${quantity}</td>
                            <td class="text-end">${currencySymbol}${parseFloat(price).toFixed(2)}</td>
                            <td class="text-end">${currencySymbol}${itemTotal}</td>
                        </tr>
                    `;
                });
                
                const previewContent = `
                    <div class="container">
                        <div class="row mb-4">
                            <div class="col-md-6">
                                <h2>${businessName}</h2>
                                <p>${businessAddress.replace(/\n/g, '<br>')}</p>
                                <p>Email: ${businessEmail}<br>Phone: ${businessPhone}</p>
                            </div>
                            <div class="col-md-6 text-end">
                                <h2 class="text-primary">INVOICE</h2>
                                <p><strong>Invoice Number:</strong> ${invoiceNumber}</p>
                                <p><strong>Invoice Date:</strong> ${new Date(invoiceDate).toLocaleDateString()}</p>
                                <p><strong>Due Date:</strong> ${new Date(dueDate).toLocaleDateString()}</p>
                            </div>
                        </div>
                        
                        <div class="row mb-4">
                            <div class="col-md-6">
                                <h4>Bill To:</h4>
                                <p>${clientName}<br>${clientAddress.replace(/\n/g, '<br>')}<br>Email: ${clientEmail}<br>Phone: ${clientPhone}</p>
                            </div>
                        </div>
                        
                        <table class="table table-bordered">
                            <thead class="table-light">
                                <tr>
                                    <th>Description</th>
                                    <th class="text-center">Quantity</th>
                                    <th class="text-end">Unit Price</th>
                                    <th class="text-end">Total</th>
                                </tr>
                            </thead>
                            <tbody>
                                ${itemsHTML}
                            </tbody>
                            <tfoot>
                                <tr>
                                    <td colspan="3" class="text-end"><strong>Subtotal:</strong></td>
                                    <td class="text-end"><strong>${subtotal}</strong></td>
                                </tr>
                                <tr>
                                    <td colspan="3" class="text-end"><strong>Tax:</strong></td>
                                    <td class="text-end"><strong>${taxAmount}</strong></td>
                                </tr>
                                <tr>
                                    <td colspan="3" class="text-end"><strong>Total:</strong></td>
                                    <td class="text-end"><strong>${total}</strong></td>
                                </tr>
                            </tfoot>
                        </table>
                        
                        <div class="mt-4">
                            <h5>Notes:</h5>
                            <p>${notes.replace(/\n/g, '<br>')}</p>
                        </div>
                    </div>
                `;
                
                document.getElementById('previewContent').innerHTML = previewContent;
            }
            
            downloadPdf() {
                if (!this.validateForm()) {
                    this.showToast('Please fill all required fields', 'error');
                    return;
                }
                
                this.showLoading('Generating PDF...');
                
                // Simulate PDF generation delay
                setTimeout(() => {
                    this.generatePDF();
                    this.hideLoading();
                    this.showToast('PDF downloaded successfully!');
                }, 1500);
            }
            
            generatePDF() {
                const businessName = document.getElementById('businessName').value;
                const businessAddress = document.getElementById('businessAddress').value;
                const businessEmail = document.getElementById('businessEmail').value;
                const businessPhone = document.getElementById('businessPhone').value;
                
                const clientName = document.getElementById('clientName').value;
                const clientAddress = document.getElementById('clientAddress').value;
                const clientEmail = document.getElementById('clientEmail').value;
                const clientPhone = document.getElementById('clientPhone').value;
                
                const invoiceNumber = document.getElementById('invoiceNumber').value;
                const invoiceDate = document.getElementById('invoiceDate').value;
                const dueDate = document.getElementById('dueDate').value;
                const notes = document.getElementById('notes').value;
                
                const currencySymbol = this.getCurrencySymbol();
                const subtotal = document.getElementById('subtotal').textContent;
                const taxAmount = document.getElementById('taxAmount').textContent;
                const total = document.getElementById('total').textContent;
                
                let items = [];
                document.querySelectorAll('.item-row').forEach(row => {
                    const description = row.querySelector('input[type="text"]').value;
                    const quantity = row.querySelector('.quantity').value;
                    const price = row.querySelector('.price').value;
                    const itemTotal = row.querySelector('.item-total').value;
                    
                    items.push([
                        description,
                        quantity,
                        `${currencySymbol}${parseFloat(price).toFixed(2)}`,
                        `${currencySymbol}${itemTotal}`
                    ]);
                });
                
                const docDefinition = {
                    content: [
                        { text: 'INVOICE', style: 'header' },
                        {
                            columns: [
                                {
                                    text: [
                                        { text: `${businessName}\n`, style: 'subheader' },
                                        `${businessAddress}\n`,
                                        `Email: ${businessEmail}\n`,
                                        `Phone: ${businessPhone}`
                                    ]
                                },
                                {
                                    text: [
                                        { text: `Invoice Number: ${invoiceNumber}\n`, alignment: 'right' },
                                        { text: `Invoice Date: ${new Date(invoiceDate).toLocaleDateString()}\n`, alignment: 'right' },
                                        { text: `Due Date: ${new Date(dueDate).toLocaleDateString()}`, alignment: 'right' }
                                    ],
                                    alignment: 'right'
                                }
                            ]
                        },
                        { text: '\n' },
                        {
                            text: [
                                { text: 'Bill To:\n', style: 'subheader' },
                                `${clientName}\n`,
                                `${clientAddress}\n`,
                                `Email: ${clientEmail}\n`,
                                `Phone: ${clientPhone}`
                            ]
                        },
                        { text: '\n' },
                        {
                            table: {
                                headerRows: 1,
                                widths: ['*', 'auto', 'auto', 'auto'],
                                body: [
                                    [
                                        { text: 'Description', style: 'tableHeader' },
                                        { text: 'Quantity', style: 'tableHeader' },
                                        { text: 'Unit Price', style: 'tableHeader' },
                                        { text: 'Total', style: 'tableHeader' }
                                    ],
                                    ...items,
                                    [
                                        { text: 'Subtotal:', colSpan: 3, alignment: 'right' },
                                        {},
                                        {},
                                        { text: subtotal, alignment: 'right' }
                                    ],
                                    [
                                        { text: 'Tax:', colSpan: 3, alignment: 'right' },
                                        {},
                                        {},
                                        { text: taxAmount, alignment: 'right' }
                                    ],
                                    [
                                        { text: 'Total:', colSpan: 3, alignment: 'right', style: 'tableTotal' },
                                        {},
                                        {},
                                        { text: total, alignment: 'right', style: 'tableTotal' }
                                    ]
                                ]
                            }
                        },
                        { text: '\n' },
                        {
                            text: [
                                { text: 'Notes:\n', style: 'subheader' },
                                notes
                            ]
                        }
                    ],
                    styles: {
                        header: {
                            fontSize: 18,
                            bold: true,
                            alignment: 'center',
                            margin: [0, 0, 0, 20]
                        },
                        subheader: {
                            fontSize: 14,
                            bold: true,
                            margin: [0, 10, 0, 5]
                        },
                        tableHeader: {
                            bold: true,
                            fontSize: 13,
                            color: 'black'
                        },
                        tableTotal: {
                            bold: true,
                            fontSize: 13
                        }
                    }
                };
                
                pdfMake.createPdf(docDefinition).download(`invoice-${invoiceNumber}.pdf`);
            }
            
            printInvoice() {
                if (!this.validateForm()) {
                    this.showToast('Please fill all required fields', 'error');
                    return;
                }
                
                this.generatePreview();
                document.getElementById('invoicePreview').style.display = 'block';
                
                setTimeout(() => {
                    window.print();
                }, 500);
            }
            
            saveInvoice() {
                if (!this.validateForm()) {
                    this.showToast('Please fill all required fields', 'error');
                    return;
                }
                
                const invoiceData = {
                    businessName: document.getElementById('businessName').value,
                    businessAddress: document.getElementById('businessAddress').value,
                    businessEmail: document.getElementById('businessEmail').value,
                    businessPhone: document.getElementById('businessPhone').value,
                    clientName: document.getElementById('clientName').value,
                    clientAddress: document.getElementById('clientAddress').value,
                    clientEmail: document.getElementById('clientEmail').value,
                    clientPhone: document.getElementById('clientPhone').value,
                    invoiceNumber: document.getElementById('invoiceNumber').value,
                    invoiceDate: document.getElementById('invoiceDate').value,
                    dueDate: document.getElementById('dueDate').value,
                    currency: document.getElementById('currency').value,
                    notes: document.getElementById('notes').value,
                    taxRate: document.getElementById('taxRate').value,
                    discount: document.getElementById('discount').value,
                    items: [],
                    subtotal: document.getElementById('subtotal').textContent,
                    taxAmount: document.getElementById('taxAmount').textContent,
                    total: document.getElementById('total').textContent,
                    createdAt: new Date().toISOString()
                };
                
                // Get items
                document.querySelectorAll('.item-row').forEach(row => {
                    const description = row.querySelector('input[type="text"]').value;
                    const quantity = row.querySelector('.quantity').value;
                    const price = row.querySelector('.price').value;
                    const itemTotal = row.querySelector('.item-total').value;
                    
                    invoiceData.items.push({
                        description,
                        quantity,
                        price,
                        itemTotal
                    });
                });
                
                // Check if we're updating an existing invoice
                const existingIndex = this.invoices.findIndex(inv => inv.invoiceNumber === invoiceData.invoiceNumber);
                
                if (existingIndex !== -1) {
                    this.invoices[existingIndex] = invoiceData;
                    this.showToast('Invoice updated successfully!');
                } else {
                    this.invoices.push(invoiceData);
                    this.showToast('Invoice saved successfully!');
                }
                
                // Save to localStorage
                localStorage.setItem('invoices', JSON.stringify(this.invoices));
                
                // Update stats
                this.updateStats();
            }
            
            updateStats() {
                const invoicesCreated = this.invoices.length;
                let totalRevenue = 0;
                
                this.invoices.forEach(invoice => {
                    // Extract numeric value from currency string
                    const totalValue = parseFloat(invoice.total.replace(/[^\d.]/g, ''));
                    totalRevenue += totalValue;
                });
                
                const paidInvoices = this.invoices.length > 0 ? 
                    Math.round((this.invoices.filter(inv => new Date(inv.dueDate) < new Date()).length / this.invoices.length) * 100) : 0;
                
                document.getElementById('invoicesCreated').textContent = invoicesCreated;
                document.getElementById('totalRevenue').textContent = `$${totalRevenue.toFixed(1)}K`;
                document.getElementById('paidInvoices').textContent = `${paidInvoices}%`;
            }
            
            showToast(message, type = 'success') {
                const toast = document.createElement('div');
                toast.className = `toast ${type === 'error' ? 'error' : ''}`;
                toast.innerHTML = `
                    <div class="toast-icon">
                        <i class="fas ${type === 'error' ? 'fa-exclamation-circle' : 'fa-check-circle'}"></i>
                    </div>
                    <div class="toast-message">${message}</div>
                `;
                
                document.getElementById('toastContainer').appendChild(toast);
                
                // Show toast
                setTimeout(() => {
                    toast.classList.add('show');
                }, 100);
                
                // Hide toast after 3 seconds
                setTimeout(() => {
                    toast.classList.remove('show');
                    setTimeout(() => {
                        toast.remove();
                    }, 300);
                }, 3000);
            }
            
            showLoading(message) {
                const loadingToast = document.createElement('div');
                loadingToast.className = 'toast';
                loadingToast.innerHTML = `
                    <div class="toast-icon">
                        <div class="spinner"></div>
                    </div>
                    <div class="toast-message">${message}</div>
                `;
                
                document.getElementById('toastContainer').appendChild(loadingToast);
                
                // Show loading
                setTimeout(() => {
                    loadingToast.classList.add('show');
                }, 100);
                
                return loadingToast;
            }
            
            hideLoading(loadingToast) {
                if (loadingToast) {
                    loadingToast.classList.remove('show');
                    setTimeout(() => {
                        loadingToast.remove();
                    }, 300);
                }
            }
        }

        // Initialize the invoice manager when the page loads
        document.addEventListener('DOMContentLoaded', () => {
            const invoiceManager = new InvoiceManager();
        });
    </script>
</body>
</html>
