<style>
    /* 1. Global Reset for consistency */
    .contact-showcase, .contact-showcase * {
        box-sizing: border-box;
    }

    .contact-showcase {
        display: flex;
        flex-wrap: wrap;
        gap: 30px;
        justify-content: center;
        padding: 40px 20px;
        font-family: 'Segoe UI', Roboto, sans-serif;
        background-color: #f4f7f6;
    }

    .contact-card {
        background: #ffffff;
        border-radius: 12px;
        box-shadow: 0 10px 25px rgba(0,0,0,0.08);
        padding: 24px;
        /* Fixed: Using flex-basis for better grid behavior */
        flex: 1 1 350px; 
        max-width: 450px;
        text-align: center;
        transition: transform 0.3s cubic-bezier(0.25, 0.46, 0.45, 0.94);
    }

    .contact-card:hover {
        transform: translateY(-8px);
    }

    .contact-card h1 {
        font-size: 1.4rem;
        color: #2d3436;
        margin: 0 0 20px 0; /* Fixed: Removed top margin */
        font-weight: 700;
        line-height: 1.2;
    }

    .contact-card img {
        width: 100%;
        height: 200px; /* Fixed: Forces uniform height for card alignment */
        object-fit: cover; /* Fixed: Prevents image stretching */
        border-radius: 8px;
        margin-bottom: 20px;
        border: 1px solid #eee;
        display: block;
    }

    .btn-view {
        display: inline-block;
        padding: 14px 28px;
        background-color: #0984e3;
        color: #ffffff !important; /* Fixed: Ensures text stays white */
        text-decoration: none;
        border-radius: 8px;
        font-weight: 600;
        transition: all 0.2s ease;
        width: 100%; /* Fixed: Full width button looks better on cards */
    }

    .btn-view:hover {
        background-color: #0773c5;
        box-shadow: 0 4px 12px rgba(9, 132, 227, 0.3);
    }

    /* Premium specific styling */
    .premium-card {
        border: 2px solid #6c5ce7; /* Subtle highlight for premium */
    }

    .premium-card .btn-view {
        background-color: #6c5ce7;
    }
    
    .premium-card .btn-view:hover {
        background-color: #5b4bc4;
        box-shadow: 0 4px 12px rgba(108, 92, 231, 0.3);
    }

    /* Mobile optimization */
    @media (max-width: 480px) {
        .contact-card {
            flex-basis: 100%;
        }
    }
</style>

<div class="contact-showcase">
    <div class="contact-card">
        <h1>Custom Modern Contact Page</h1>
        <img src="./Images/contact page mordern.png" alt="Modern Contact Preview">
        <a href="./custom-modern-contact-page/custom-modern-contact.liquid" class="btn-view">
            See This Section
        </a>
    </div>

<div class="contact-card">
        <h1>Premium Contact Page</h1>
        <img src="./Images/premium contact page.png" alt="Premium Contact Preview">
        <a href="./premium-contact-page/Premium-contact_page.liquid" class="btn-view">
            See This Section
        </a>
       </div>

<div class="contact-card">
        <h1>Elit About US page</h1>
        <img src="./Images/Elit About us page.png" alt="Elit About US page<">
        <a href="./premium contact page/Elite About us page/" class="btn-view">
            See This Section
        </a>
    </div>

<div class="contact-card">
        <h1>Premium testimonial</h1>
        <img src="./Images/premium testimonial.png" alt="premium testimonial<">
        <a href="./Premium Testimonial/premium-testimonial.liquid" class="btn-view">
            See This Section
        </a>
    </div>
</div>