:root {
  --blue: #22438a;
  --white: #ffffff;
  --background: #ffffff;
  --text: #17305f;
  --muted: #667085;
  --header-height: 86px;
  --transition: 220ms ease;
}

/* Reset simple */
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
  background: var(--background);
  color: var(--text);
  font-family: Georgia, "Times New Roman", serif;
}

a {
  color: inherit;
  text-decoration: none;
}

img {
  max-width: 100%;
  display: block;
}

body {
  font-family: 'Cabinet Grotesk', sans-serif;
  font-weight: 400;
}

h1 {
  font-family: 'Cabinet Grotesk', sans-serif;
  font-weight: 800;
  letter-spacing: -0.04em;
}

h2, h3 {
  font-family: 'Cabinet Grotesk', sans-serif;
  font-weight: 700;
  letter-spacing: -0.03em;
}

p {
  font-weight: 400;
  letter-spacing: -0.01em;
}

.navbar a,
.btn,
button {
  font-weight: 500;
  letter-spacing: -0.01em;
}

/* HEADER */

.site-header {
  position: fixed;
  top: 0;
  left: 0;
  z-index: 1000;
  width: 100%;
  height: var(--header-height);

  background: transparent;
  color: var(--white);

  transition:
    background-color var(--transition),
    color var(--transition),
    box-shadow var(--transition),
    backdrop-filter var(--transition);
}

/* HEADER TRANSPARENT */
.site-header.is-transparent {
  background: transparent;
  color: var(--white);
  box-shadow: none;
}

/* HEADER BLANC AU SCROLL */
.site-header.is-solid {
  background: rgba(255, 255, 255, 0.96);
  backdrop-filter: blur(12px);
  color: var(--blue);

  box-shadow:
    0 10px 30px rgba(34, 67, 138, 0.08);
}

.navbar {
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 clamp(20px, 5vw, 72px);
}

.nav-left,
.nav-right {
  display: flex;
  align-items: center;
  gap: 14px;
}

.logo-link {
  padding: 0;
  margin-right: 18px;
}

.logo {
  width: 62px;
  height: 62px;
  object-fit: contain;
}

.nav-link {
  position: relative;
  border-radius: 4px;
  padding: 11px 15px;
  font-size: 15px;
  font-weight: 700;
  letter-spacing: 0.02em;
  transition:
    color var(--transition),
    background-color var(--transition),
    transform var(--transition);
}

/* Hover uniquement quand le header est transparent */
.site-header.is-transparent .nav-link:not(.logo-link):hover,
.site-header.is-transparent .nav-link:not(.logo-link).is-active {
  background: var(--white);
  color: var(--blue) !important;
}

/* Quand le header est blanc : pas de carré au hover */
.site-header.is-solid .nav-link:hover,
.site-header.is-solid .nav-link.is-active {
  background: transparent;
  color: var(--blue) !important;
}

.nav-contact,
.site-header.is-transparent .nav-contact,
.site-header.is-solid .nav-contact,
.site-header.is-transparent .nav-contact:hover,
.site-header.is-solid .nav-contact:hover {
  background: var(--blue);
  color: var(--white) !important;
}

.nav-contact:hover {
  transform: translateY(-1px);
}

/* LIENS HEADER TRANSPARENT */
.site-header.is-transparent .nav-link {
  color: var(--white);
}

/* LIENS HEADER BLANC */
.site-header.is-solid .nav-link {
  color: var(--blue);
}

/* PAGES */
/* 
  Toutes les pages sont masquées par défaut.
  Une seule page est affichée :
  - soit via JS avec .active
  - soit immédiatement via l’URL avec :target
  - soit accueil par défaut quand il n’y a pas de hash
*/
.page {
  display: none;
  min-height: 100vh;
}

.page.active,
.page:target {
  display: block;
}

html:not(.has-hash) #accueil {
  display: block;
}
/* HERO ACCUEIL */
.hero {
  position: relative;
  min-height: 100vh;
  overflow: hidden;
}

.hero-home {
  background-image: url("../assets/hero-home.png");
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
}

.hero-overlay {
  position: absolute;
  inset: 0;
  background: linear-gradient(
    90deg,
    rgba(0, 0, 0, 0.62) 0%,
    rgba(0, 0, 0, 0.36) 42%,
    rgba(0, 0, 0, 0.2) 100%
  );
}

.hero-content {
  position: absolute;
  z-index: 2;
  left: 5%;
  bottom: 10%;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
}

.hero-content h1 {
  color: var(--white);
  font-size: clamp(48px, 8vw, 112px);
  line-height: 0.92;
  letter-spacing: 0.04em;
  font-weight: 700;
  text-transform: uppercase;
  animation: fadeUp 700ms ease both;
}

/* RÉCAP ACCUEIL */
.home-summary {
  padding: clamp(64px, 8vw, 110px) clamp(20px, 6vw, 86px);
  display: grid;
  gap: clamp(56px, 7vw, 96px);
}

.summary-block {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: clamp(32px, 5vw, 72px);
  align-items: center;
}

.summary-block.reverse .summary-image {
  order: 2;
}

.summary-block.reverse .summary-text {
  order: 1;
}

.summary-image {
  min-height: 360px;
  border-radius: 22px;
  overflow: hidden;
}

.placeholder-image,
.placeholder-banner {
  display: flex;
  align-items: center;
  justify-content: center;
  background:
    linear-gradient(135deg, rgba(34, 67, 138, 0.16), rgba(34, 67, 138, 0.04)),
    #f3f6fc;
  color: var(--blue);
  border: 1px dashed rgba(34, 67, 138, 0.35);
  font-weight: 700;
}

.summary-text {
  max-width: 590px;
}

.section-label {
  margin-bottom: 14px;
  color: var(--blue);
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 0.12em;
  font-size: 13px;
}

.summary-text h2 {
  margin-bottom: 18px;
  font-size: clamp(30px, 4vw, 52px);
  line-height: 1.04;
  color: var(--blue);
}

.summary-text p {
  margin-bottom: 24px;
  color: var(--muted);
  font-size: 18px;
  line-height: 1.7;
}

.button-primary {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  min-height: 46px;
  padding: 0 22px;
  border-radius: 4px;
  background: var(--blue);
  color: var(--white);
  font-weight: 700;
  transition:
    transform var(--transition),
    box-shadow var(--transition);
}

.button-primary:hover {
  transform: translateY(-2px);
  box-shadow: 0 12px 26px rgba(34, 67, 138, 0.22);
}

/* BANNIÈRES DES AUTRES PAGES */
.page-banner {
  min-height: 62vh;
  padding-top: var(--header-height);
}

.page-banner h1 {
  font-size: clamp(46px, 7vw, 92px);
  color: var(--blue);
  text-align: center;
}

/* ANIMATIONS */
@keyframes fadeUp {
  from {
    opacity: 0;
    transform: translateY(24px);
  }

  to {
    opacity: 1;
    transform: translateY(0);
  }
}

/* RESPONSIVE */
@media (max-width: 920px) {
  :root {
    --header-height: 76px;
  }

  .navbar {
    padding: 0 18px;
  }

  .nav-left,
  .nav-right {
    gap: 6px;
  }

  .nav-link {
    font-size: 13px;
    padding: 9px 10px;
  }

  .logo {
    width: 52px;
    height: 52px;
  }

  .summary-block,
  .summary-block.reverse {
    grid-template-columns: 1fr;
  }

  .summary-block.reverse .summary-image,
  .summary-block.reverse .summary-text {
    order: initial;
  }
}

@media (max-width: 720px) {
  .site-header {
    height: auto;
    min-height: var(--header-height);
  }

  .navbar {
    flex-direction: column;
    align-items: stretch;
    gap: 10px;
    padding-top: 10px;
    padding-bottom: 10px;
  }

  .nav-left,
  .nav-right {
    justify-content: center;
    flex-wrap: wrap;
  }

  .logo-link {
    width: 100%;
    display: flex;
    justify-content: center;
    margin-right: 0;
  }

.hero-content {
  left: 6%;
  right: 6%;
  bottom: 8%;
}

  .hero-content h1 {
    font-size: clamp(42px, 15vw, 72px);
  }
}

@media (prefers-reduced-motion: reduce) {
  html {
    scroll-behavior: auto;
  }

  *,
  *::before,
  *::after {
    animation: none !important;
    transition: none !important;
  }
}


.site-header.is-transparent .nav-contact,
.site-header.is-solid .nav-contact,
.site-header.is-transparent .nav-contact:hover,
.site-header.is-solid .nav-contact:hover {
  background: var(--blue);
  color: var(--white) !important;
}

.logo-link:hover,
.logo-link.is-active {
  background: transparent !important;
}

.navbar a {
  font-size: 1.1rem;
}

.hero-subtitle-top {
  color: white;
  font-size: 1rem;
  font-weight: 500;
  letter-spacing: 0.15em;
  text-transform: uppercase;
  margin-bottom: 1rem;
}

.hero-btn-secondary {
  margin-top: 2rem;
  margin-left: 210px;
  padding: 14px 32px;
  background: white;
  color: #0A3D91;
  border-radius: 999px;
  text-decoration: none;
  font-weight: 700;
  transition: all 0.3s ease;
}

.hero-btn-secondary:hover {
  transform: translateY(-2px);
}

.scroll-indicator {
  position: absolute;
  bottom: 28px;
  left: 50%;
  transform: translateX(-50%);
  z-index: 3;

  width: 42px;
  height: 42px;

  display: flex;
  align-items: center;
  justify-content: center;

  animation: bounce 2s infinite;
}

.scroll-indicator span {
  width: 24px;
  height: 24px;

  border-right: 4px solid white;
  border-bottom: 4px solid white;

  transform: rotate(45deg);
}

@keyframes bounce {
  0%, 100% {
    transform: translateX(-50%) translateY(0);
  }

  50% {
    transform: translateX(-50%) translateY(10px);
  }
}
.summary-image {
  width: 100%;
  height: 420px;
  border-radius: 22px;
  overflow: hidden;
}

/* Images réelles */
.summary-image img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
}

/* NEWSLETTER COMPACTE */
.newsletter {
  background: var(--blue);
  color: var(--white);
  padding: 38px clamp(24px, 6vw, 90px);
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 32px;
}

.newsletter h2 {
  max-width: 520px;
  font-size: clamp(28px, 3.6vw, 48px);
  line-height: 1;
  font-style: italic;
  color: var(--white);
}

.newsletter-form {
  display: flex;
  width: min(100%, 560px);
}

.newsletter-form input {
  flex: 1;
  min-height: 48px;
  padding: 0 18px;
  border: 1px solid var(--white);
  background: transparent;
  color: var(--white);
  font: inherit;
  outline: none;
}

.newsletter-form input::placeholder {
  color: rgba(255, 255, 255, 0.7);
}

.newsletter-form button {
  min-height: 48px;
  padding: 0 22px;
  border: 1px solid var(--white);
  background: var(--white);
  color: var(--blue);
  font: inherit;
  font-weight: 700;
  cursor: pointer;
}

/* FOOTER COMPACT */
.site-footer {
  background: var(--blue);
  color: var(--white);
  padding: 34px clamp(24px, 6vw, 90px) 24px;
}

.footer-grid {
  display: grid;
  grid-template-columns: 1.4fr 1.2fr 0.8fr 0.8fr 0.9fr;
  gap: 28px;
  align-items: start;
}

.footer-column {
  display: flex;
  flex-direction: column;
  gap: 8px;
}

.footer-column h3 {
  margin-bottom: 8px;
  font-size: 22px;
  line-height: 1;
  font-style: italic;
  color: var(--white);
}

.footer-column p,
.footer-column a {
  color: var(--white);
  font-size: 14px;
  line-height: 1.45;
}

.footer-column a {
  text-decoration: underline;
  text-underline-offset: 3px;
}

.footer-column iframe {
  width: 100%;
  height: 150px;
  border: 1px solid rgba(255, 255, 255, 0.35);
  border-radius: 12px;
}

.footer-bottom {
  margin-top: 28px;
  padding-top: 18px;
  border-top: 1px solid rgba(255, 255, 255, 0.22);
}

.footer-bottom p {
  color: var(--white);
  font-size: 13px;
  font-weight: 700;
  letter-spacing: 0.04em;
}

/* RESPONSIVE */
@media (max-width: 980px) {
  .newsletter {
    flex-direction: column;
    align-items: flex-start;
  }

  .newsletter-form {
    width: 100%;
  }

  .footer-grid {
    grid-template-columns: 1fr 1fr;
  }
}

@media (max-width: 620px) {
  .newsletter-form {
    flex-direction: column;
  }

  .footer-grid {
    grid-template-columns: 1fr;
  }
}

/* PAGE QUI SOMMES-NOUS */
.about-hero {
  position: relative;
  min-height: 67vh;
  background-image: url("../assets/photogroup.png");
  background-size: cover;
  background-position: center;
  border-radius: 0 0 18px 18px;
  overflow: hidden;
}

.about-hero-overlay {
  position: absolute;
  inset: 0;
  background: rgba(0, 0, 0, 0.52);
}

.about-hero-content {
  position: relative;
  z-index: 1;
  min-height: 67vh;
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  max-width: 860px;
  padding: var(--header-height) clamp(24px, 7vw, 96px) 80px;
  color: var(--white);
}

.about-kicker {
  margin-bottom: 16px;
  font-weight: 700;
  letter-spacing: 0.08em;
  text-transform: uppercase;
}

.about-hero h1 {
  margin-bottom: 22px;
  font-size: clamp(48px, 7vw, 88px);
  line-height: 0.95;
}

.about-hero p {
  font-size: clamp(18px, 2vw, 26px);
  line-height: 1.45;
}

.about-content {
  padding: clamp(70px, 8vw, 120px) clamp(24px, 7vw, 120px);
}

.about-text {
  max-width: 920px;
  margin: 0 auto;
}

.about-text h2 {
  margin-bottom: 28px;
  color: var(--blue);
  font-size: clamp(36px, 5vw, 68px);
  line-height: 1;
}

.about-text p {
  margin-bottom: 22px;
  color: var(--text);
  font-size: 19px;
  line-height: 1.8;
}

/* SECTIONS ÉQUIPE */
.team-section {
  padding: clamp(70px, 8vw, 120px) clamp(24px, 7vw, 120px);
}

.team-office {
  background: var(--blue);
  color: var(--white);
}

.team-poles {
  background: var(--white);
  color: var(--blue);
}

.section-heading {
  max-width: 850px;
  margin-bottom: 48px;
}

.section-heading h2 {
  margin-bottom: 18px;
  font-size: clamp(42px, 6vw, 76px);
  line-height: 0.95;
  font-style: italic;
}

.section-heading p {
  font-size: 18px;
  line-height: 1.7;
}

.section-label-light {
  margin-bottom: 14px;
  color: var(--white);
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 0.12em;
  font-size: 13px;
}

.team-global-photo {
  height: 360px;
  margin-bottom: 42px;
  border: 1px dashed rgba(255, 255, 255, 0.5);
  border-radius: 22px;
  display: flex;
  align-items: center;
  justify-content: center;
  color: var(--white);
  font-weight: 700;
}

.team-grid,
.poles-grid {
  display: grid;
  gap: 28px;
}

.team-grid {
  grid-template-columns: repeat(3, 1fr);
}

.poles-grid {
  grid-template-columns: repeat(3, 1fr);
}

.team-card,
.pole-card {
  display: flex;
  flex-direction: column;
  gap: 12px;
}

.team-photo,
.pole-photo {
  height: 300px;
  border-radius: 18px;
  overflow: hidden;
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: 700;
}

.team-photo {
  border: 1px dashed rgba(255, 255, 255, 0.5);
  color: var(--white);
}

.pole-photo {
  background: #f3f6fc;
  border: 1px dashed rgba(34, 67, 138, 0.35);
  color: var(--blue);
}

.team-photo img,
.pole-photo img,
.team-global-photo img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.team-card h3,
.pole-card h3 {
  margin-top: 10px;
  font-size: 26px;
  line-height: 1.1;
}

.team-card p,
.pole-card p {
  font-size: 17px;
  line-height: 1.5;
}

@media (max-width: 920px) {
  .team-grid,
  .poles-grid {
    grid-template-columns: 1fr 1fr;
  }
}

@media (max-width: 620px) {
  .team-grid,
  .poles-grid {
    grid-template-columns: 1fr;
  }

  .team-global-photo,
  .team-photo,
  .pole-photo {
    height: 260px;
  }
}

/* PAGE NOS MISSIONS */
.missions-hero {
  position: relative;
  min-height: 58vh;
  background-image: url("../assets/photogrouperasmus.png");
  background-size: cover;
  background-position: center;
  border-radius: 0 0 18px 18px;
  overflow: hidden;
}

.missions-hero-overlay {
  position: absolute;
  inset: 0;
  background: rgba(0, 0, 0, 0.52);
}

.missions-hero-content {
  position: relative;
  z-index: 1;
  min-height: 58vh;
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  width: 100%;
  max-width: 1400px;
  padding: var(--header-height) clamp(24px, 7vw, 96px) 70px;
  color: var(--white);
}

.missions-hero h1 {
  margin-bottom: 22px;
  max-width: 1200px;
  font-size: clamp(52px, 7vw, 104px);
  line-height: 0.92;
}

.missions-hero p {
  font-size: clamp(18px, 2vw, 25px);
  line-height: 1.45;
}

.missions-content,
.missions-gallery {
  padding: clamp(70px, 8vw, 120px) clamp(24px, 7vw, 120px);
}

.missions-intro {
  max-width: 980px;
  margin-bottom: 54px;
}

.missions-intro h2 {
  margin-bottom: 26px;
  color: var(--blue);
  font-size: clamp(38px, 5vw, 70px);
  line-height: 1;
}

.missions-intro p {
  margin-bottom: 20px;
  color: var(--text);
  font-size: 19px;
  line-height: 1.8;
}

.missions-image-row {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 36px;
  margin-bottom: 90px;
}

.missions-image-row img {
  width: 100%;
  height: 380px;
  object-fit: cover;
  border-radius: 22px;
}

.missions-grid-text {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 60px;
}

.missions-grid-text h3 {
  margin-bottom: 14px;
  color: var(--blue);
  font-size: 30px;
  font-style: italic;
}

.missions-grid-text p {
  color: var(--text);
  font-size: 17px;
  line-height: 1.75;
}

.missions-events {
  background: var(--blue);
  color: var(--white);
  padding: clamp(70px, 8vw, 120px) clamp(24px, 7vw, 120px);
}

.event-highlight {
  max-width: 900px;
  padding: 48px 0;
}

.event-highlight:last-child {
  border-bottom: 1px solid rgba(255, 255, 255, 0.25);
}

.event-highlight h3 {
  margin-bottom: 12px;
  font-size: clamp(30px, 4vw, 52px);
  font-style: italic;
  color: var(--white);
}

.event-highlight p {
  font-size: 18px;
  line-height: 1.75;
}

.gallery-featured {
  margin-bottom: 26px;
}

.gallery-featured img {
  width: 100%;
  height: 560px;
  object-fit: cover;
  border-radius: 24px;
}

.gallery-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 18px;
}

.gallery-grid img {
  width: 100%;
  height: 220px;
  object-fit: cover;
  border-radius: 16px;
}

@media (max-width: 920px) {
  .missions-image-row,
  .missions-grid-text {
    grid-template-columns: 1fr;
  }

  .gallery-grid {
    grid-template-columns: repeat(2, 1fr);
  }

  .gallery-featured img {
    height: 420px;
  }
}

@media (max-width: 620px) {
  .gallery-grid {
    grid-template-columns: 1fr;
  }

  .gallery-grid img,
  .missions-image-row img {
    height: 260px;
  }

  .gallery-featured img {
    height: 320px;
  }
}

.missions-events-layout {
  display: grid;
  grid-template-columns: 1.1fr 0.9fr;
  gap: clamp(40px, 6vw, 90px);
  align-items: start;
}

.missions-events-image img {
  width: 100%;
  height: 100%;
  min-height: 720px;
  object-fit: cover;
  border-radius: 24px;
}

@media (max-width: 920px) {
  .missions-events-layout {
    grid-template-columns: 1fr;
  }

  .missions-events-image img {
    min-height: 420px;
  }
}

.missions-intro {
  max-width: 920px;
  margin: 0 auto 90px;
  text-align: left;
}

.missions-intro h2 {
  margin-bottom: 36px;
  font-size: clamp(38px, 5vw, 70px);
  line-height: 1;
  color: var(--blue);
}

.missions-intro p {
  margin-bottom: 28px;
  color: var(--text);
  font-size: 19px;
  line-height: 1.8;
}

.missions-intro-inner {
  max-width: 920px;
}
/* PAGE ACTU */
.actu-hero {
  position: relative;
  min-height: 58vh;
  background-image: url("../assets/bateau.png");
  background-size: cover;
  background-position: center;
  color: var(--white);
  border-radius: 0 0 18px 18px;
  overflow: hidden;
}

.actu-hero::before {
  content: "";
  position: absolute;
  inset: 0;
  background: rgba(0, 0, 0, 0.52);
}

.actu-hero-content {
  position: relative;
  z-index: 1;
  min-height: 58vh;
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  max-width: 1100px;
  padding: var(--header-height) clamp(24px, 7vw, 96px) 70px;
}

.actu-hero h1 {
  margin-bottom: 22px;
  font-size: clamp(52px, 7vw, 104px);
  line-height: 0.92;
}

.actu-hero p {
  font-size: clamp(18px, 2vw, 25px);
  line-height: 1.45;
}

.next-events {
  padding: clamp(44px, 5vw, 70px) clamp(24px, 7vw, 120px);
}

.news-feed,
.instagram-live {
  padding: clamp(70px, 8vw, 120px) clamp(24px, 7vw, 120px);
}



.events-countdown-card {
  margin-bottom: 24px;
  padding: 22px 26px;
  background: var(--blue);
  color: var(--white);
  border-radius: 18px;
}

.events-countdown-card p {
  margin-bottom: 10px;
  opacity: 0.8;
  text-transform: uppercase;
  letter-spacing: 0.12em;
  font-size: 13px;
}

.countdown {
  font-size: clamp(28px, 4vw, 52px);
  font-weight: 800;
  line-height: 1;
}

.next-events-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 28px;
}

.next-event-card {
  padding: 24px;
  border: 1px solid rgba(34, 67, 138, 0.18);
  border-radius: 18px;
  background: #f3f6fc;
}

.event-date {
  margin-bottom: 14px;
  color: var(--blue);
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 0.12em;
  font-size: 13px;
}

.next-event-card h3,
.news-card h3 {
  margin-bottom: 14px;
  color: var(--blue);
  font-size: clamp(26px, 3vw, 42px);
  line-height: 1;
  font-style: italic;
}

.next-event-card p,
.news-card p {
  margin-bottom: 18px;
  color: var(--text);
  font-size: 18px;
  line-height: 1.7;
}

.next-event-card span {
  color: var(--blue);
  font-weight: 700;
}

.news-feed {
  background: var(--white);
}

.news-card {
  display: grid;
  grid-template-columns: 0.9fr 1.1fr;
  gap: clamp(36px, 6vw, 90px);
  align-items: center;
  padding: 56px 0;
  border-top: 1px solid rgba(34, 67, 138, 0.16);
}

.news-card.reverse .news-text {
  order: 2;
}

.news-card.reverse .instagram-embed {
  order: 1;
}

.news-text {
  max-width: 620px;
}

.instagram-embed {
  display: flex;
  justify-content: center;
  overflow: hidden;
}

.instagram-media {
  max-width: 540px !important;
  width: 100% !important;
  min-width: 280px !important;
}

.instagram-live {
  background: var(--blue);
  color: var(--white);
  text-align: center;
}

.instagram-live h2 {
  margin: 0 auto 18px;
  max-width: 900px;
  font-size: clamp(38px, 5vw, 72px);
  line-height: 1;
  font-style: italic;
  color: var(--white);
}

.instagram-live p {
  margin-bottom: 28px;
  font-size: 22px;
  font-weight: 700;
}

.instagram-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  min-height: 48px;
  padding: 0 24px;
  border-radius: 999px;
  background: var(--white);
  color: var(--blue);
  font-weight: 700;
}

@media (max-width: 920px) {
  .next-events-grid,
  .news-card {
    grid-template-columns: 1fr;
  }

  .news-card.reverse .news-text,
  .news-card.reverse .instagram-embed {
    order: initial;
  }
}

.instagram-live {
  background: var(--white);
  color: var(--blue);
  text-align: center;
  padding: clamp(70px, 8vw, 120px) clamp(24px, 7vw, 120px);
}

.instagram-live h2 {
  margin: 0 auto 18px;
  max-width: 980px;
  font-size: clamp(42px, 6vw, 82px);
  line-height: 1;
  font-style: italic;
  color: var(--blue);
}

.instagram-live p {
  margin-bottom: 30px;
  font-size: 24px;
  font-weight: 800;
  color: var(--blue);
}

.instagram-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  min-height: 50px;
  padding: 0 26px;
  border-radius: 999px;
  background: var(--blue);
  color: var(--white);
  font-weight: 700;
}

/* PAGE CONTACT */
.contact-hero {
  background: var(--blue);
  color: var(--white);
  border-radius: 0 0 18px 18px;
}

.contact-hero-content {
  min-height: 52vh;
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  max-width: 1100px;
  padding: var(--header-height) clamp(24px, 7vw, 96px) 70px;
}

.contact-hero h1 {
  margin-bottom: 22px;
  font-size: clamp(52px, 7vw, 104px);
  line-height: 0.92;
}

.contact-hero p {
  font-size: clamp(18px, 2vw, 25px);
  line-height: 1.45;
}

.contact-section {
  padding: clamp(70px, 8vw, 120px) clamp(24px, 7vw, 120px);
}

.contact-intro {
  max-width: 920px;
  margin: 0 auto 60px;
}

.contact-intro h2 {
  margin-bottom: 28px;
  color: var(--blue);
  font-size: clamp(38px, 5vw, 70px);
  line-height: 1;
}

.contact-intro p {
  color: var(--text);
  font-size: 19px;
  line-height: 1.8;
}

.contact-layout {
  display: flex;
  justify-content: center;
}

.contact-form {
  padding: 36px;
  background: #f3f6fc;
  border-radius: 24px;
  display: grid;
  gap: 22px;
}

.form-row {
  display: grid;
  gap: 8px;
}

.form-row label {
  color: var(--blue);
  font-weight: 700;
}

.form-row input,
.form-row textarea {
  width: 100%;
  border: 1px solid rgba(34, 67, 138, 0.22);
  border-radius: 12px;
  padding: 15px 16px;
  color: var(--text);
  font: inherit;
  outline: none;
  background: var(--white);
}

.form-row textarea {
  resize: vertical;
}

.contact-form button {
  min-height: 52px;
  border: none;
  border-radius: 999px;
  background: var(--blue);
  color: var(--white);
  font: inherit;
  font-weight: 700;
  cursor: pointer;
}

.form-note {
  color: var(--muted);
  font-size: 14px;
}

.contact-card {
  padding: 36px;
  background: var(--blue);
  color: var(--white);
  border-radius: 24px;
  display: grid;
  gap: 28px;
}

.contact-card h3 {
  font-size: clamp(30px, 4vw, 48px);
  line-height: 1;
  font-style: italic;
}

.contact-info-block {
  display: grid;
  gap: 6px;
}

.contact-info-block p {
  font-size: 13px;
  text-transform: uppercase;
  letter-spacing: 0.12em;
  opacity: 0.75;
}

.contact-info-block span,
.contact-info-block a {
  color: var(--white);
  font-size: 18px;
  line-height: 1.5;
}

.contact-info-block a {
  text-decoration: underline;
  text-underline-offset: 4px;
}

.contact-form {
  width: min(100%, 760px);
  margin: 0 auto;
  padding: 36px;
  background: #f3f6fc;
  border-radius: 24px;
  display: grid;
  gap: 22px;
}

/* PAGES SIMPLES : BOUTIQUE + BILLETTERIE */
.simple-page {
  min-height: 70vh;
  padding: var(--header-height) clamp(24px, 7vw, 120px) 80px;
  display: flex;
  align-items: center;
  justify-content: center;
  background: #f3f6fc;
}

.simple-page-content {
  max-width: 900px;
  text-align: center;
}

.simple-page-content h1 {
  margin-bottom: 22px;
  color: var(--blue);
  font-size: clamp(52px, 7vw, 104px);
  line-height: 0.92;
}

.simple-page-content p:last-child {
  color: var(--text);
  font-size: clamp(20px, 2vw, 28px);
  line-height: 1.5;
}

/* MENU MOBILE */
.menu-toggle {
  display: none;
}

@media (max-width: 820px) {
  .site-header {
    height: var(--header-height);
  }

  .navbar {
    height: 100%;
    padding: 0 22px;
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  .menu-toggle {
    display: flex;
    flex-direction: column;
    justify-content: center;
    gap: 5px;

    width: 44px;
    height: 44px;

    background: transparent;
    border: none;
    cursor: pointer;

    color: currentColor;
    z-index: 1400;
  }

  .menu-toggle span {
    width: 28px;
    height: 2px;
    background: currentColor;
    border-radius: 99px;
    transition: transform 220ms ease, opacity 220ms ease;
  }

  body.menu-open .menu-toggle span:nth-child(1) {
    transform: translateY(7px) rotate(45deg);
  }

  body.menu-open .menu-toggle span:nth-child(2) {
    opacity: 0;
  }

  body.menu-open .menu-toggle span:nth-child(3) {
    transform: translateY(-7px) rotate(-45deg);
  }

  .nav-left,
  .nav-right {
    display: flex;
    align-items: center;
  }

  .nav-left .nav-link:not(.logo-link),
  .nav-right {
    display: none;
  }

  .logo-link {
    margin-right: 0;
    padding: 0;
    z-index: 1400;
  }

  .logo {
    width: 54px;
    height: 54px;
  }

  body.menu-open::before {
    content: "";
    position: fixed;
    inset: 0;
    background: rgba(0, 0, 0, 0.38);
    z-index: 1050;
  }

  body.menu-open .nav-left,
  body.menu-open .nav-right {
    position: fixed;
    right: 0;
    width: min(82vw, 360px);

    background: var(--blue);
    color: var(--white);

    z-index: 1200;

    display: flex;
    flex-direction: column;
    align-items: flex-start;

    padding-left: 28px;
    padding-right: 28px;
  }

  body.menu-open .nav-left {
    top: 0;
    height: 330px;
    padding-top: 110px;
    gap: 18px;
  }

  body.menu-open .nav-right {
    top: 330px;
    bottom: 0;
    gap: 18px;
  }

  body.menu-open .nav-left .nav-link:not(.logo-link),
  body.menu-open .nav-right {
    display: flex;
  }

  body.menu-open .nav-link {
    color: var(--white) !important;
    font-size: 20px;
    padding: 8px 0;
    background: transparent !important;
  }

  body.menu-open .nav-contact {
    margin-top: 8px;
    padding: 12px 18px;
    background: var(--white) !important;
    color: var(--blue) !important;
  }

  body.menu-open .logo-link {
    position: fixed;
    top: 18px;
    right: calc(min(82vw, 360px) - 82px);
  }
}

/* CORRECTION MENU MOBILE */
@media (max-width: 820px) {
  .navbar {
    position: relative;
    height: var(--header-height);
    padding: 0 22px;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .menu-toggle {
    position: absolute;
    left: 22px;
    top: 50%;
    transform: translateY(-50%);
    display: flex;
    width: 44px;
    height: 44px;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    gap: 5px;
    z-index: 3000;
  }

  .menu-toggle span {
    width: 28px;
    height: 2px;
    background: currentColor;
  }

  .logo-link {
    width: auto !important;
    margin: 0 !important;
    padding: 0 !important;
  }

  .nav-left {
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .nav-left .nav-link:not(.logo-link),
  .nav-right {
    display: none;
  }

  body.menu-open .nav-left,
  body.menu-open .nav-right {
    position: fixed;
    right: 0;
    width: min(82vw, 360px);
    background: var(--blue);
    z-index: 2500;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    padding-left: 28px;
    padding-right: 28px;
  }

  body.menu-open .nav-left {
    top: 0;
    height: 310px;
    padding-top: 105px;
    gap: 18px;
  }

  body.menu-open .nav-right {
    top: 310px;
    bottom: 0;
    gap: 18px;
  }

  body.menu-open .nav-left .nav-link:not(.logo-link),
  body.menu-open .nav-right {
    display: flex;
  }

  body.menu-open .logo-link {
    position: fixed;
    top: 22px;
    right: calc(min(82vw, 360px) / 2 - 27px);
    z-index: 3000;
  }

  body.menu-open .nav-link {
    color: white !important;
    background: transparent !important;
    font-size: 18px;
  }

  body.menu-open .nav-contact {
    background: white !important;
    color: var(--blue) !important;
    padding: 12px 18px;
  }
}
