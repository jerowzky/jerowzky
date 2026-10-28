
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Jeruh Fornal's developer profile and tech stack.">
    <title>Jeruh Fornal | Developer Profile</title>
</head>
<style>
  
/* ================================
   GLOBAL STYLES
================================ */

:root {
    --bg: #080d0b;
    --surface: #101713;
    --surface-hover: #151f19;
    --accent: #03a271;
    --accent-light: #4fd9a8;
    --text: #f1f5f2;
    --muted: #9aa79f;
    --border: rgba(79, 217, 168, 0.16);
}

* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

html {
    scroll-behavior: smooth;
}

body {
    min-height: 100vh;
    background:
        radial-gradient(
            ellipse at 50% 0%,
            rgba(3, 162, 113, 0.14),
            transparent 50%
        ),
        var(--bg);
    color: var(--text);
    font-family: Arial, Helvetica, sans-serif;
    line-height: 1.7;
}

a {
    color: inherit;
    text-decoration: none;
}

.container {
    width: min(100% - 40px, 1000px);
    margin: 0 auto;
}

/* ================================
   HERO
================================ */

.hero {
    padding: 100px 0 80px;
    text-align: center;
    border-bottom: 1px solid var(--border);
}

.eyebrow {
    display: inline-block;
    margin-bottom: 18px;
    color: var(--accent-light);
    font-size: 0.75rem;
    font-weight: 700;
    letter-spacing: 4px;
}

.hero h1 {
    font-size: clamp(2.5rem, 8vw, 5.5rem);
    font-weight: 900;
    line-height: 1.15;
    letter-spacing: -3px;
}

.hero h1 span {
    color: var(--accent-light);
}

.subtitle {
    margin-top: 20px;
    color: var(--muted);
    font-size: 1rem;
}

.hero-tags,
.social-links,
.tags {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 10px;
}

.hero-tags {
    margin-top: 28px;
}

.hero-tags span,
.tags span {
    padding: 6px 12px;
    border: 1px solid var(--border);
    border-radius: 8px;
    background: rgba(16, 23, 19, 0.8);
    color: var(--accent-light);
    font-size: 0.8rem;
}

.social-links {
    margin-top: 32px;
}

.social-links a {
    padding: 9px 17px;
    border: 1px solid var(--border);
    border-radius: 8px;
    font-size: 0.85rem;
    transition: 0.2s ease;
}

.social-links a:hover {
    border-color: var(--accent);
    background: rgba(3, 162, 113, 0.12);
    color: var(--accent-light);
}

/* ================================
   SECTIONS
================================ */

.section {
    padding: 55px 0 10px;
}

.section-heading {
    display: flex;
    align-items: center;
    gap: 14px;
    margin-bottom: 22px;
}

.section-number {
    color: var(--accent-light);
    font-size: 0.8rem;
    font-weight: 700;
    letter-spacing: 2px;
}

.section-heading h2 {
    font-size: clamp(1.4rem, 4vw, 2rem);
    letter-spacing: -0.5px;
}

/* ================================
   CARDS
================================ */

.card {
    border: 1px solid var(--border);
    border-radius: 16px;
    background: linear-gradient(
        145deg,
        rgba(16, 23, 19, 0.95),
        rgba(10, 16, 12, 0.95)
    );
}

.about-card {
    padding: 28px;
}

.about-card p {
    color: var(--muted);
}

.about-card p + p {
    margin-top: 16px;
}

.about-card strong {
    color: var(--text);
}

.skills-grid {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 16px;
}

.skill-card {
    padding: 24px;
}

.skill-card h3 {
    margin-bottom: 18px;
    font-size: 1rem;
}

.tags {
    justify-content: flex-start;
    gap: 8px;
}

.tags span {
    color: var(--text);
    font-size: 0.78rem;
}

.skill-card:hover {
    border-color: rgba(79, 217, 168, 0.4);
}

/* ================================
   CONTACT
================================ */

.contact-card {
    padding: 30px;
    text-align: center;
}

.contact-card p {
    margin-bottom: 22px;
    color: var(--muted);
}

.contact-button {
    display: inline-flex;
    align-items: center;
    gap: 12px;
    padding: 12px 22px;
    border-radius: 9px;
    background: var(--accent);
    color: #04110b;
    font-weight: 700;
    transition: 0.2s ease;
}

.contact-button:hover {
    background: var(--accent-light);
    transform: translateY(-2px);
}

/* ================================
   FOOTER
================================ */

footer {
    display: flex;
    justify-content: space-between;
    gap: 16px;
    margin-top: 75px;
    padding: 25px 0 35px;
    border-top: 1px solid var(--border);
    color: var(--muted);
    font-size: 0.8rem;
}

footer a {
    color: var(--accent-light);
}

/* ================================
   RESPONSIVE
================================ */

@media (max-width: 600px) {
    .container {
        width: min(100% - 28px, 1000px);
    }

    .hero {
        padding: 70px 0 55px;
    }

    .hero h1 {
        letter-spacing: -1.5px;
    }

    .subtitle {
        font-size: 0.9rem;
    }

    .skills-grid {
        grid-template-columns: 1fr;
    }

    .about-card,
    .skill-card,
    .contact-card {
        padding: 20px;
    }

    footer {
        flex-direction: column;
        text-align: center;
    }
}

@media (prefers-reduced-motion: reduce) {
    *,
    *::before,
    *::after {
        scroll-behavior: auto !important;
        transition-duration: 0.01ms !important;
    }
}

</style>
<body>


    <main class="container">

        <header class="hero">
            <span class="eyebrow">WELCOME TO MY PROFILE</span>
            <h1>JERUH <span>FORNAL</span></h1>
            <p class="subtitle">
                Web Development · UI/UX Design · Quality Assurance
            </p>

            <div class="hero-tags">
                <span>Frontend Development</span>
                <span>UI/UX Design</span>
                <span>BSIT · PUP</span>
            </div>

            <div class="social-links">
                <a href="mailto:jeruhasis@gmail.com">Email</a>
                <a href="https://www.linkedin.com/in/jeruh-fornal">LinkedIn</a>
                <a href="https://github.com/jerowzky">GitHub</a>
                <a href="https://www.instagram.com/its_jeyuh">Instagram</a>
            </div>
        </header>

        <section class="section">
            <div class="section-heading">
                <span class="section-number">01</span>
                <h2>About Me</h2>
            </div>

            <div class="card about-card">
                <p>
                    I'm a passionate <strong>Web Developer</strong> focused on
                    <strong>Frontend Development</strong> and
                    <strong>UI/UX Design</strong>. Currently, I'm a fourth-year
                    BS Information Technology student at the
                    <strong>Polytechnic University of the Philippines</strong>.
                </p>
                <p>
                    I enjoy building websites, exploring creative design
                    solutions, and improving user experiences while continuing
                    to develop my technical skills.
                </p>
            </div>
        </section>

        <section class="section">
            <div class="section-heading">
                <span class="section-number">02</span>
                <h2>Tech Stack & Skills</h2>
            </div>

            <div class="skills-grid">

                <article class="card skill-card">
                    <h3>Languages</h3>
                    <div class="tags">
                        <span>HTML5</span>
                        <span>CSS3</span>
                        <span>JavaScript</span>
                        <span>PHP</span>
                        <span>Python</span>
                        <span>Java</span>
                    </div>
                </article>

                <article class="card skill-card">
                    <h3>Frameworks & Libraries</h3>
                    <div class="tags">
                        <span>Tailwind CSS</span>
                        <span>jQuery</span>
                    </div>
                </article>

                <article class="card skill-card">
                    <h3>Databases</h3>
                    <div class="tags">
                        <span>MySQL</span>
                        <span>SQLite</span>
                    </div>
                </article>

                <article class="card skill-card">
                    <h3>Tools & Platforms</h3>
                    <div class="tags">
                        <span>GitHub</span>
                        <span>VS Code</span>
                        <span>Figma</span>
                        <span>Canva</span>
                    </div>
                </article>

            </div>
        </section>

        <section class="section">
            <div class="section-heading">
                <span class="section-number">03</span>
                <h2>Let's Connect</h2>
            </div>

            <div class="card contact-card">
                <p>Have a project or opportunity in mind? Let's connect.</p>
                <a class="contact-button"
                   href="mailto:jeruhasis@gmail.com">
                    Get in Touch <span aria-hidden="true">↗</span>
                </a>
            </div>
        </section>

        <footer>
            <p>Designed & built with care by Jeruh Fornal.</p>
            <a href="https://github.com/jerowzky">GitHub Profile ↗</a>
        </footer>

    </main>

</body>
</html>
