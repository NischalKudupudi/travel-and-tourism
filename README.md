:root {
  --primary-color: #0a0d14;
  --primary-color-light: #20242f;
  --secondary-color: #f49e09;
  --extra-light: rgba(255, 255, 255, 0.5);
  --white: #ffffff;
  --max-width: 1200px;
  --header-font: "Lisu Bosa", serif;
}

{
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

.section__container {
  max-width: var(--max-width);
  margin: auto;
  padding: 5rem 1rem;
}

.section__header {
  margin-bottom: 2rem;
  font-size: 3rem;
  font-weight: 800;
  font-family: var(--header-font);
  text-align: center;
}

.section__subheader {
  max-width: 600px;
  margin: auto;
  text-align: center;
}

.btn {
  padding: 0.75rem 1.5rem;
  outline: none;
  border: none;
  font-size: 1rem;
  color: var(--primary-color);
  background-color: var(--secondary-color);
  cursor: pointer;
}

img {
  width: 100%;
  display: flex;
}

a {
  text-decoration: none;
}

html,
body {
  scroll-behavior: smooth;
}

body {
  font-family: "Poppins", sans-serif;
  color: var(--white);
  background-color: var(--primary-color);
}

header {
  background-image: linear-gradient(to top, var(--primary-color), transparent),
    url("mountain.jpg");
  background-position: center center;
  background-size: cover;
  background-repeat: no-repeat;
}

nav {
  background-color: rgba(231, 119, 119, 0.5);
  border-bottom: 1px solid var(--extra-light);
}

.nav__bar {
  max-width: var(--max-width);
  margin: auto;
  padding: 1.5rem 1rem;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 2rem;
}

.nav__logo a {
  font-size: 1.2rem;
  font-weight: 600;
  color: var(--white);
}

.nav__links {
  list-style: none;
  display: flex;
  align-items: center;
  gap: 2rem;
}

.link a {
  padding: 1.5rem 5px;
  font-weight: 500;
  color: var(--white);
  transition: 0.3s;
}

.link a:hover {
  color: var(--secondary-color);
  border-bottom: 2px solid var(--secondary-color);
}

.link span {
  padding: 1rem 0;
  color: var(--white);
  cursor: pointer;
}

.header__container {
  padding: 12rem 1rem;
}

.header__container h1 {
  margin-bottom: 1rem;
  max-width: 700px;
  font-size: 4rem;
  font-family: var(--header-font);
}

.header__container h4 {
  position: relative;
  margin-left: 3rem;
  margin-bottom: 2rem;
  font-size: 1rem;
  font-weight: 500;
}

.header__container h4::after {
  position: absolute;
  content: "";
  left: -3rem;
  top: 50%;
  transform: translateY(-50%);
  height: 2px;
  width: 2rem;
  background-color: var(--white);
}

.about__container {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 2rem;
  align-items: center;
}

.about_container :is(.sectionheader, .section_subheader) {
  text-align: left;
}

.about__flex {
  margin: 2rem 0;
  padding: 2rem 1rem;
  display: flex;
  align-items: center;
  gap: 1rem;
  flex-wrap: wrap;
  background-color: var(--primary-color-light);
}

.about__card {
  flex: 1 1 150px;
  text-align: center;
  border-right: 2px solid var(--primary-color);
}

.about__card:last-child {
  border: none;
}

.about__card h4 {
  margin-bottom: 5px;
  font-size: 3rem;
  font-weight: 600;
  font-family: var(--header-font);
}

.about__card p {
  font-size: 0.9rem;
}

.about__image img {
  max-width: 450px;
  margin: auto;
}

.discover {
  background-image: linear-gradient(
    to bottom,
    rgba(255, 255, 255, 0.05),
    transparent
  );
}

.discover__grid {
  margin-top: 4rem;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 2rem;
}

.discover__card {
  max-width: 320px;
  margin: auto;
}

.discover__card:nth-child(2) {
  transform: translateY(5rem);
}

.discover__image {
  position: relative;
}

.discover__image::after {
  position: absolute;
  content: "";
  width: 100%;
  height: 50%;
  left: 0;
  bottom: 0;
  background-image: linear-gradient(to top, var(--primary-color), transparent);
}

.discover_card_content {
  padding: 0 2rem;
  transform: translateY(-50%);
}

.discover_card_content h4 {
  margin-bottom: 1rem;
  font-size: 2rem;
  font-weight: 800;
  font-family: var(--header-font);
  color: var(--secondary-color);
}

.discover_card_content p {
  margin-bottom: 2rem;
}

.discover__btn {
  padding: 0.75rem 1rem;
  outline: none;
  font-size: 1rem;
  color: var(--white);
  background-color: transparent;
  border: 1px solid var(--white);
  cursor: pointer;
}

.blogs__container {
  padding: 5rem 0;
}

.blogs__grid {
  margin-top: 4rem;
  display: grid;
  grid-template-columns: repeat(4, 1fr);
}

.blogs__card {
  position: relative;
}

.blogs__card::after {
  position: absolute;
  content: "";
  width: 100%;
  height: 100%;
  left: 0;
  top: 0;
  background-image: linear-gradient(to top, var(--primary-color), transparent);
}

.blogs__content {
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  padding: 2rem;
  font-size: 1.2rem;
  font-weight: 500;
  z-index: 1;
}

.journals__grid {
  margin-top: 4rem;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 2rem;
}

.journals__content {
  padding: 2rem;
  background-color: var(--primary-color-light);
}

.journals__author {
  margin-bottom: 1rem;
  display: flex;
  align-items: center;
  gap: 1rem;
}

.journals__author img {
  max-width: 30px;
  border-radius: 100%;
}

.journals__author p {
  font-size: 0.9rem;
  opacity: 0.75;
}

.journals__content h4 {
  margin-bottom: 0.5rem;
  font-size: 1.1rem;
  font-weight: 600;
}

.journals__footer {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 2rem;
}

.journals__footer p {
  font-size: 0.9rem;
  opacity: 0.5;
}

.journals__footer span a {
  font-size: 1.5rem;
  color: var(--white);
  opacity: 0.75;
}

.journals__btn {
  margin-top: 4rem;
  text-align: center;
}

.hero__container p {
  text-align: center;
  font-size: 12rem;
  font-weight: 700;
  background-image: url("banner.jpg");
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  -webkit-text-stroke: 1px var(--extra-light);
}

.gallery__container {
  padding: 5rem 1rem;
}

.gallery__grid {
  margin-top: 4rem;
  display: grid;
  grid-template-columns: repeat(5, 1fr);
  gap: 1rem;
}

.gallery__card {
  position: relative;
  overflow: hidden;
}

.gallery__content {
  position: absolute;
  left: 50%;
  bottom: -8rem;
  transform: translateX(-50%);
  width: 100%;
  padding: 2rem 1rem;
  transition: 0.3s;
  text-align: center;
  background-image: linear-gradient(to top, var(--primary-color), transparent);
}

.gallery__content h4 {
  margin-bottom: 1rem;
  font-size: 2rem;
  font-weight: 800;
  font-family: var(--header-font);
}

.gallery_card:hover .gallery_content {
  bottom: 0;
}

.contact {
  background-image: linear-gradient(
    to top,
    rgba(255, 255, 255, 0.05),
    transparent
  );
}

.contact__container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 2rem;
  align-items: center;
}

.contact__card {
  max-width: 250px;
  margin: auto;
  aspect-ratio: 1;
  display: grid;
  place-content: center;
  text-align: center;
  border: 1px solid var(--extra-light);
  border-radius: 100%;
  cursor: pointer;
}

.contact__card span {
  margin-bottom: 1rem;
  font-size: 2rem;
  transition: 0.3s;
}

.contact__card:hover span {
  color: var(--secondary-color);
}

.contact__col h4 {
  margin-bottom: 1rem;
  font-size: 2.5rem;
  font-weight: 800;
  font-family: var(--header-font);
}

.contact__col h5 {
  margin-bottom: 0.5rem;
  font-size: 1.5rem;
  font-weight: 600;
  font-family: var(--header-font);
}

.footer__container {
  text-align: center;
}

.footer__container h4 {
  margin-bottom: 1rem;
  font-size: 1.5rem;
  font-weight: 600;
}

.footer__socials {
  margin-bottom: 2rem;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 2rem;
}

.footer__socials span a {
  font-size: 1.5rem;
  color: var(--white);
  cursor: pointer;
  transition: 0.3s;
}

.footer__socials span a:hover {
  color: var(--secondary-color);
}

.footer__container p {
  max-width: 600px;
  margin: auto;
  margin-bottom: 4rem;
}

.footer__nav {
  list-style: none;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-wrap: wrap;
  gap: 2rem;
}

.footer__link a {
  font-weight: 500;
  color: var(--white);
}

.footer__link a:hover {
  color: var(--secondary-color);
}

.footer__bar {
  padding: 1rem;
  text-align: center;
  font-size: 0.8rem;
  border-top: 1px solid var(--extra-light);
}

@media (width < 900px) {
  .link:not(.search) {
    display: none;
  }

  .about__container {
    grid-template-columns: repeat(1, 1fr);
    text-align: center;
  }

  .about_container :is(.sectionheader, .section_subheader) {
    text-align: center;
  }

  .about__image {
    grid-area: 1/1/2/2;
  }

  .discover__grid {
    grid-template-columns: repeat(2, 1fr);
  }

  .blogs__grid {
    grid-template-columns: repeat(2, 1fr);
  }

  .journals__grid {
    grid-template-columns: repeat(2, 1fr);
    gap: 1rem;
  }

  .hero__container p {
    font-size: 10rem;
  }

  .gallery__grid {
    grid-template-columns: repeat(3, 1fr);
  }

  .contact__container {
    grid-template-columns: repeat(2, 1fr);
  }

  .contact__col:first-child {
    grid-area: 1/1/2/3;
    text-align: center;
  }
}

@media (width < 600px) {
  .header__container {
    text-align: center;
  }

  .header__container h4 {
    margin-left: 0;
  }

  .about__card {
    border: none;
  }

  .discover__grid {
    grid-template-columns: repeat(1, 1fr);
  }

  .discover__card:nth-child(2) {
    transform: translateY(0);
  }

  .blogs__grid {
    grid-template-columns: repeat(1, 1fr);
  }

  .journals__grid {
    grid-template-columns: repeat(1, 1fr);
  }

  .hero__container p {
    font-size: 6rem;
  }

  .gallery__grid {
    grid-template-columns: repeat(2, 1fr);
  }

  .contact__container {
    grid-template-columns: repeat(1, 1fr);
  }

  .contact__col:first-child {
    grid-area: unset;
  }
}
