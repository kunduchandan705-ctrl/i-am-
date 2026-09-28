* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    color: #222;
    background: #f7f8fc;
}


/* Navigation */

header {
    position: sticky;
    top: 0;
    z-index: 1000;
    background: #111827;
}

.navbar {
    max-width: 1100px;
    margin: auto;
    padding: 18px 20px;

    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    color: #ffffff;
    font-size: 25px;
}

.nav-links {
    list-style: none;
    display: flex;
    gap: 25px;
}

.nav-links a {
    color: white;
    text-decoration: none;
    font-weight: 500;
    transition: 0.3s;
}

.nav-links a:hover {
    color: #38bdf8;
}


/* Hero */

.hero {
    min-height: 90vh;

    display: flex;
    justify-content: center;
    align-items: center;

    text-align: center;

    background:
        linear-gradient(135deg, #111827, #1e3a8a);
    
    color: white;
    padding: 40px 20px;
}

.hero-content {
    max-width: 750px;
}

.intro {
    font-size: 20px;
    color: #38bdf8;
}

.hero h1 {
    font-size: 60px;
    margin: 10px 0;
}

.hero h3 {
    font-size: 28px;
    margin-bottom: 20px;
}

.hero p {
    font-size: 18px;
}


/* Buttons */

.btn {
    display: inline-block;

    margin-top: 25px;
    padding: 12px 28px;

    background: #38bdf8;
    color: #082f49;

    border: none;
    border-radius: 30px;

    font-weight: bold;
    text-decoration: none;

    cursor: pointer;

    transition: 0.3s;
}

.btn:hover {
    transform: translateY(-3px);
    background: #7dd3fc;
}


/* Common Sections */

.section {
    padding: 90px 20px;
}

.container {
    max-width: 1100px;
    margin: auto;
}

.section h2 {
    text-align: center;
    font-size: 36px;
    margin-bottom: 30px;
}


/* About */

#about {
    background: white;
}

#about p {
    max-width: 750px;
    margin: auto;
    text-align: center;
    font-size: 18px;
}

.skills {
    margin-top: 35px;

    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 12px;
}

.skills span {
    background: #e0f2fe;
    color: #0369a1;

    padding: 10px 18px;
    border-radius: 20px;

    font-weight: bold;
}


/* Projects */

.projects-section {
    background: #f1f5f9;
}

.project-grid {
    display: grid;

    grid-template-columns:
        repeat(3, 1fr);

    gap: 25px;
}

.project-card {
    background: white;

    padding: 30px;

    border-radius: 15px;

    box-shadow:
        0 10px 30px rgba(0, 0, 0, 0.08);

    transition: 0.3s;
}

.project-card:hover {
    transform: translateY(-8px);
}

.project-card h3 {
    margin-bottom: 15px;
    font-size: 22px;
}

.project-card p {
    color: #555;
}

.project-btn {
    display: inline-block;

    margin-top: 20px;

    color: #0369a1;
    text-decoration: none;

    font-weight: bold;
}


/* Contact */

#contact {
    background: white;
}

.contact-text {
    text-align: center;
    margin-bottom: 30px;
}

form {
    max-width: 650px;
    margin: auto;

    display: flex;
    flex-direction: column;

    gap: 15px;
}

input,
textarea {
    width: 100%;

    padding: 15px;

    border: 1px solid #d1d5db;
    border-radius: 8px;

    font-size: 16px;

    outline: none;
}

input:focus,
textarea:focus {
    border-color: #38bdf8;
}

textarea {
    resize: vertical;
}


/* Footer */

footer {
    background: #111827;
    color: white;

    text-align: center;

    padding: 25px;
}


/* Responsive Design */

@media (max-width: 768px) {

    .navbar {
        flex-direction: column;
        gap: 15px;
    }

    .nav-links {
        gap: 15px;
        flex-wrap: wrap;
        justify-content: center;
    }

    .hero h1 {
        font-size: 42px;
    }

    .hero h3 {
        font-size: 22px;
    }

    .project-grid {
        grid-template-columns: 1fr;
    }

    .section {
        padding: 65px 20px;
    }
}
