<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>RR Legal Solutions</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;500;700&family=Inter:wght@300;400;600&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
  <style>
    /* CSS Variables for easier theme management - Black and White Palette */
    :root {
      --color-primary-dark: #0A0A0A; /* Near Black */
      --color-secondary-dark: #1A1A1A; /* Deep Charcoal */
      --color-accent-dark: #333333; /* Dark Grey for accents */
      --color-accent-light: #BBBBBB; /* Light Grey for accents */
      --color-white: #FDFDFD; /* Soft White */
      --color-off-white: #F5F5F5; /* Subtle background */
      --color-light-grey: #DDDDDD;
      --color-dark-text: #222222; /* Darker text for contrast on light backgrounds */
      --color-medium-text: #444444;
    }

    /* Base Styles */
    body {
      margin: 0;
      font-family: 'Inter', sans-serif;
      background-color: var(--color-off-white);
      color: var(--color-dark-text);
      line-height: 1.8; /* Increased line height for elegance */
      scroll-behavior: smooth;
      /* Subtle, almost imperceptible geometric background pattern */
      background-image: url('data:image/svg+xml,%3Csvg width="60" height="60" viewBox="0 0 60 60" xmlns="http://www.w3.org/2000/svg"%3E%3Cg fill="none" fill-rule="evenodd"%3E%3Cg fill="%23e0e0e0" fill-opacity="0.08"%3E%3Cpath d="M36 34v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zm0 20v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zM6 4h-.995V2h1.001V1.1h-.006V0H4.995v1.1h.006V2H4V4h-.005v1.1h.006V6H2.995v-1.1h.006V4H2V2h-.005V1.1h.006V0H.995v1.1H1V2H0V4h-.005v1.1h.006V6H.995v-1.1h.006V4h1.005v1.1h-.006V6H4v-1.1h-.005V4h1.005v1.1h-.006V6H6v-1.1h-.005V4zm0 20h-.995V22h1.001v-1.1h-.006V20H4.995v1.1h.006V22H4V24h-.005v1.1h.006V26H2.995v-1.1h.006V24H2V22h-.005v1.1h.006V20H.995v1.1H1V22H0V24h-.005v1.1h.006V26H.995v-1.1h.006V24h1.005v1.1h-.006V26H4v-1.1h-.005V24h1.005v1.1h-.006V26H6v-1.1h-.005V24zM24 4h-.995V2h1.001v-1.1h-.006V0H22.995v1.1h.006V2H22V4h-.005v1.1h.006V6H20.995v-1.1h.006V4H20V2h-.005V1.1h.006V0H18.995v1.1H19V2H18V4h-.005v1.1h.006V6H18.995v-1.1h.006V4h1.005v1.1h-.006V6H22v-1.1h-.005V4h1.005v1.1h-.006V6H24v-1.1h-.005V4zm0 20h-.995V22h1.001v-1.1h-.006V20H22.995v1.1h.006V22H22V24h-.005v1.1h.006V26H20.995v-1.1h.006V24H20V22h-.005v1.1h.006V20H18.995v1.1H19V22H18V24h-.005v1.1h.006V26H18.995v-1.1h.006V24h1.005v1.1h-.006V26H22v-1.1h-.005V24h1.005v1.1h-.006V26H24v-1.1h-.005V24zM42 4h-.995V2h1.001v-1.1h-.006V0H40.995v1.1h.006V2H40V4h-.005v1.1h.006V6H38.995v-1.1h.006V4H38V2h-.005V1.1h.006V0H36.995v1.1H37V2H36V4h-.005v1.1h.006V6H36.995v-1.1h.006V4h1.005v1.1h-.006V6H40v-1.1h-.005V4h1.005v1.1h-.006V6H42v-1.1h-.005V4zm0 20h-.995V22h1.001v-1.1h-.006V20H40.995v1.1h.006V22H40V24h-.005v1.1h.006V26H38.995v-1.1h.006V24H38V22h-.005v1.1h.006V20H36.995v1.1H37V22H36V24h-.005v1.1h.006V26H36.995v-1.1h.006V24h1.005v1.1h-.006V26H40v-1.1h-.005V24h1.005v1.1h-.006V26H42v-1.1h-.005V24zM24 34v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zm0 20v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zM48 4h-.995V2h1.001v-1.1h-.006V0H46.995v1.1h.006V2H46V4h-.005v1.1h.006V6H44.995v-1.1h.006V4H44V2h-.005V1.1h.006V0H42.995v1.1H43V2H42V4h-.005v1.1h.006V6H42.995v-1.1h.006V4h1.005v1.1h-.006V6H46v-1.1h-.005V4h1.005v1.1h-.006V6H48v-1.1h-.005V4zm0 20h-.995V22h1.001v-1.1h-.006V20H46.995v1.1h.006V22H46V24h-.005v1.1h.006V26H44.995v-1.1h.006V24H44V22h-.005v1.1h.006V20H42.995v1.1H43V22H42V24h-.005v1.1h.006V26H42.995v-1.1h.006V24h1.005v1.1h-.006V26H46v-1.1h-.005V24h1.005v1.1h-.006V26H48v-1.1h-.005V24zm0 30h-.995V52h1.001v-1.1h-.006V50H46.995v1.1h.006V52H46V54h-.005v1.1h.006V56H44.995v-1.1h.006V54H44V52h-.005v1.1h.006V50H42.995v1.1H43V52H42V54h-.005v1.1h.006V56H42.995v-1.1h.006V54h1.005v1.1h-.006V56H46v-1.1h-.005V54h1.005v1.1h-.006V56H48v-1.1h-.005V54zM6 34v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zm0 20v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zM30 4h-.995V2h1.001v-1.1h-.006V0H28.995v1.1h.006V2H28V4h-.005v1.1h.006V6H26.995v-1.1h.006V4H26V2h-.005V1.1h.006V0H24.995v1.1H25V2H24V4h-.005v1.1h.006V6H24.995v-1.1h.006V4h1.005v1.1h-.006V6H28v-1.1h-.005V4h1.005v1.1h-.006V6H30v-1.1h-.005V4zM30 24h-.995V22h1.001v-1.1h-.006V20H28.995v1.1h.006V22H28V24h-.005v1.1h.006V26H26.995v-1.1h.006V24H26V22h-.005v1.1h.006V20H24.995v1.1H25V22H24V24h-.005v1.1h.006V26H24.995v-1.1h.006V24h1.005v1.1h-.006V26H28v-1.1h-.005V24h1.005v1.1h-.006V26H30v-1.1h-.005V24zM30 30v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zm0 20v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zM6 48h-.995V46h1.001v-1.1h-.006V44H4.995v1.1h.006V46H4V48h-.005v1.1h.006V50H2.995v-1.1h.006V48H2V46h-.005v1.1h.006V44H.995v1.1H1V46H0V48h-.005v1.1h.006V50H.995v-1.1h.006V48h1.005v1.1h-.006V50H4v-1.1h-.005V48h1.005v1.1h-.006V50H6v-1.1h-.005V48zm0 10h-.995V56h1.001v-1.1h-.006V54H4.995v1.1h.006V56H4V58h-.005v1.1h.006V60H2.995v-1.1h.006V58H2V56h-.005v1.1h.006V54H.995v1.1H1V56H0V58h-.005v1.1h.006V60H.995v-1.1h.006V58h1.005v1.1h-.006V60H4v-1.1h-.005V58h1.005v1.1h-.006V60H6v-1.1h-.005V58zM24 48h-.995V46h1.001v-1.1h-.006V44H22.995v1.1h.006V46H22V48h-.005v1.1h.006V50H20.995v-1.1h.006V48H20V46h-.005v1.1h.006V44H18.995v1.1H19V46H18V48h-.005v1.1h.006V50H18.995v-1.1h.006V48h1.005v1.1h-.006V50H22v-1.1h-.005V48h1.005v1.1h-.006V50H24v-1.1h-.005V48zm0 10h-.995V56h1.001v-1.1h-.006V54H22.995v1.1h.006V56H22V58h-.005v1.1h.006V60H20.995v-1.1h.006V58H20V56h-.005v1.1h.006V54H18.995v1.1H19V56H18V58h-.005v1.1h.006V60H18.995v-1.1h.006V58h1.005v1.1h-.006V60H22v-1.1h-.005V58h1.005v1.1h-.006V60H24v-1.1h-.005V58zM42 48h-.995V46h1.001v-1.1h-.006V44H40.995v1.1h.006V46H40V48h-.005v1.1h.006V50H38.995v-1.1h.006V48H38V46h-.005v1.1h.006V44H36.995v1.1H37V46H36V48h-.005v1.1h.006V50H36.995v-1.1h.006V48h1.005v1.1h-.006V50H40v-1.1h-.005V48h1.005v1.1h-.006V50H42v-1.1h-.005V48zm0 10h-.995V56h1.001v-1.1h-.006V54H40.995v1.1h.006V56H40V58h-.005v1.1h.006V60H38.995v-1.1h.006V58H38V56h-.005v1.1h.006V54H36.995v1.1H37V56H36V58h-.005v1.1h.006V60H36.995v-1.1h.006V58h1.005v1.1h-.006V60H40v-1.1h-.005V58h1.005v1.1h-.006V60H42v-1.1h-.005V58zM54 34v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zm0 20v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zM54 4h-.995V2h1.001v-1.1h-.006V0H52.995v1.1h.006V2H52V4h-.005v1.1h.006V6H50.995v-1.1h.006V4H50V2h-.005V1.1h.006V0H48.995v1.1H49V2H48V4h-.005v1.1h.006V6H48.995v-1.1h.006V4h1.005v1.1h-.006V6H52v-1.1h-.005V4h1.005v1.1h-.006V6H54v-1.1h-.005V4zm0 20h-.995V22h1.001v-1.1h-.006V20H52.995v1.1h.006V22H52V24h-.005v1.1h.006V26H50.995v-1.1h.006V24H50V22h-.005v1.1h.006V20H48.995v1.1H49V22H48V24h-.005v1.1h.006V26H48.995v-1.1h.006V24h1.005v1.1h-.006V26H52v-1.1h-.005V24h1.005v1.1h-.006V26H54v-1.1h-.005V24zM54 48h-.995V46h1.001v-1.1h-.006V44H52.995v1.1h.006V46H52V48h-.005v1.1h.006V50H50.995v-1.1h.006V48H50V46h-.005v1.1h.006V44H48.995v1.1H49V46H48V48h-.005v1.1h.006V50H48.995v-1.1h.006V48h1.005v1.1h-.006V50H52v-1.1h-.005V48h1.005v1.1h-.006V50H54v-1.1h-.005V48zm0 10h-.995V56h1.001v-1.1h-.006V54H52.995v1.1h.006V56H52V58h-.005v1.1h.006V60H50.995v-1.1h.006V58H50V56h-.005v1.1h.006V54H48.995v1.1H49V56H48V58h-.005v1.1h.006V60H48.995v-1.1h.006V58h1.005v1.1h-.006V60H52v-1.1h-.005V58h1.005v1.1h-.006V60H54v-1.1h-.005V58zM30 48h-.995V46h1.001v-1.1h-.006V44H28.995v1.1h.006V46H28V48h-.005v1.1h.006V50H26.995v-1.1h.006V48H26V46h-.005v1.1h.006V44H24.995v1.1H25V46H24V48h-.005v1.1h.006V50H24.995v-1.1h.006V48h1.005v1.1h-.006V50H28v-1.1h-.005V48h1.005v1.1h-.006V50H30v-1.1h-.005V48zM30 58h-.995V56h1.001v-1.1h-.006V54H28.995v1.1h.006V56H28V58h-.005v1.1h.006V60H26.995v-1.1h.006V58H26V56h-.005v1.1h.006V54H24.995v1.1H25V56H24V58h-.005v1.1h.006V60H24.995v-1.1h.006V58h1.005v1.1h-.006V60H28v-1.1h-.005V58h1.005v1.1h-.006V60H30v-1.1h-.005V58z"%3E%3C/path%3E%3C/g%3E%3C/g%3E%3C/svg%3E');
      background-attachment: fixed;
    }

    h1, h2, h3, h4, h5, h6 {
      font-family: 'Playfair Display', serif;
      color: var(--color-primary-dark);
      margin-bottom: 1rem;
      letter-spacing: 0.8px; /* Slightly more letter spacing for elegance */
    }

    p {
      margin-bottom: 1rem;
    }

    .container {
      max-width: 1200px;
      margin: 0 auto;
      padding: 4rem 2.5rem; /* Increased padding for more breathing room */
    }

    .section-title {
      text-align: center;
      font-size: 4rem; /* Even larger for more impact */
      margin-bottom: 5rem; /* More space below title */
      color: var(--color-primary-dark);
      position: relative;
      padding-bottom: 2rem; /* More space for the underline */
      font-weight: 700;
      text-transform: uppercase; /* Uppercase for titles */
      letter-spacing: 2px;
    }

    .section-title::after {
      content: '';
      position: absolute;
      left: 50%;
      bottom: 0;
      transform: translateX(-50%);
      width: 150px; /* Longer underline */
      height: 5px; /* Thicker underline */
      background: linear-gradient(to right, var(--color-accent-dark), var(--color-accent-light)); /* Black/White gradient underline */
      border-radius: 5px;
      box-shadow: 0 3px 10px rgba(0, 0, 0, 0.3); /* Stronger glow */
    }

    /* Header */
    header {
      background: linear-gradient(to right, var(--color-secondary-dark), var(--color-primary-dark));
      color: var(--color-white);
      padding: 3.5rem 0; /* More vertical padding */
      text-align: center;
      box-shadow: 0 8px 25px rgba(0, 0, 0, 0.4); /* Deeper shadow */
    }

    header h1 {
      font-size: 5.5rem; /* Even larger firm name */
      margin: 0;
      color: var(--color-white); /* White for firm name */
      letter-spacing: 4px; /* More prominent letter spacing */
      text-shadow: 4px 4px 8px rgba(0, 0, 0, 0.7);
    }

    header p {
      font-size: 1.5rem; /* Larger tagline */
      margin-top: 1rem;
      color: var(--color-light-grey);
      font-weight: 300;
      font-style: italic;
      letter-spacing: 1px;
    }

    /* Navigation */
    nav {
      background-color: var(--color-secondary-dark);
      border-top: 1px solid var(--color-accent-dark);
      border-bottom: 1px solid var(--color-accent-dark);
      display: flex;
      justify-content: center;
      padding: 1.2rem 0; /* More padding */
      flex-wrap: wrap;
      position: sticky;
      top: 0;
      z-index: 1000;
      box-shadow: 0 3px 15px rgba(0, 0, 0, 0.3);
    }

    nav a {
      color: var(--color-light-grey); /* Lighter grey for nav links */
      padding: 1.2rem 2.5rem; /* More padding */
      text-decoration: none;
      font-weight: 600;
      letter-spacing: 1px; /* More prominent letter spacing */
      transition: background-color 0.4s ease, color 0.4s ease, transform 0.3s ease;
      position: relative;
      overflow: hidden;
      font-size: 1.2rem;
      text-transform: uppercase;
    }

    nav a::before {
      content: '';
      position: absolute;
      bottom: 0;
      left: 0;
      width: 100%;
      height: 4px; /* Thicker hover underline */
      background: linear-gradient(to right, var(--color-accent-dark), var(--color-accent-light)); /* Black/White gradient */
      transform: translateX(-100%);
      transition: transform 0.4s ease-out;
    }

    nav a:hover::before {
      transform: translateX(0);
    }

    nav a:hover {
      background-color: var(--color-accent-dark); /* Darker black on hover */
      color: var(--color-white);
      transform: translateY(-3px); /* More pronounced lift effect */
    }

    /* Hero Section */
    .hero {
      background: linear-gradient(rgba(0, 0, 0, 0.75), rgba(0, 0, 0, 0.75)), url('https://placehold.co/1920x1000/1A1A1A/FDFDFD?text=Justice+in+Black+and+White') no-repeat center center/cover; /* Updated placeholder */
      color: var(--color-white);
      text-align: center;
      padding: 12rem 2.5rem; /* More vertical padding */
      min-height: 700px; /* Taller hero section */
      display: flex;
      align-items: center;
      justify-content: center;
      position: relative;
      overflow: hidden;
    }

    .hero-content {
      max-width: 1000px;
      position: relative;
      z-index: 1;
    }

    .hero h2 {
      font-size: 5.5rem; /* Even larger hero heading */
      margin-bottom: 2rem;
      color: var(--color-white); /* White for hero heading */
      text-shadow: 5px 5px 10px rgba(0, 0, 0, 0.8);
      line-height: 1.1;
      letter-spacing: 2px;
    }

    .hero p {
      font-size: 1.8rem; /* Even larger hero text */
      font-weight: 300;
      line-height: 1.9;
      color: var(--color-light-grey);
      text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.6);
      max-width: 800px;
      margin: 0 auto;
    }

    /* About Us Section */
    #about {
      padding: 6rem 0; /* More padding */
      background-color: var(--color-white);
      position: relative;
      z-index: 1;
    }

    #about p {
      font-size: 1.2rem; /* Slightly larger text */
      line-height: 2; /* More line height for elegance */
      text-align: justify;
      max-width: 1000px;
      margin: 0 auto 2rem auto;
      color: var(--color-dark-text);
    }

    /* Team Section */
    #team {
      padding: 6rem 0;
      background-color: var(--color-off-white);
      position: relative;
      z-index: 1;
    }

    .team-intro {
      text-align: center;
      margin-bottom: 5rem; /* More space */
      font-size: 1.2rem;
      max-width: 1000px;
      margin: 0 auto 5rem auto;
      color: var(--color-medium-text);
      line-height: 1.9;
    }

    .partner-card-container {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 4rem; /* Increased gap */
      margin-top: 4rem;
    }

    .partner-card {
      background-color: var(--color-white);
      border: 1px solid #eeeeee;
      border-radius: 15px; /* More rounded */
      box-shadow: 0 15px 40px rgba(0, 0, 0, 0.15); /* Deeper shadow */
      padding: 3rem; /* More padding */
      max-width: 520px; /* Wider cards */
      text-align: center;
      transition: transform 0.5s ease, box-shadow 0.5s ease;
      position: relative;
      overflow: hidden;
      z-index: 0;
    }

    .partner-card::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 8px; /* Thicker accent border */
      background: linear-gradient(to right, var(--color-accent-dark), var(--color-accent-light)); /* Black/White gradient */
      transform: translateY(-100%);
      transition: transform 0.5s ease-out;
    }

    .partner-card:hover::before {
      transform: translateY(0);
    }

    .partner-card:hover {
      transform: translateY(-15px); /* More pronounced lift */
      box-shadow: 0 25px 50px rgba(0, 0, 0, 0.25); /* Even deeper shadow on hover */
    }

    .partner-card img {
      width: 200px; /* Larger images */
      height: 200px;
      border-radius: 50%;
      object-fit: cover;
      border: 6px solid var(--color-accent-dark); /* Thicker accent border */
      margin-bottom: 2.5rem; /* More space */
      box-shadow: 0 0 25px rgba(0, 0, 0, 0.4); /* Stronger glow (black) */
      transition: transform 0.4s ease;
    }

    .partner-card:hover img {
      transform: scale(1.07); /* More subtle zoom on image */
    }

    .partner-card h3 {
      font-size: 2.5rem; /* Larger name */
      color: var(--color-primary-dark);
      margin-bottom: 1rem;
      font-weight: 700;
      letter-spacing: 1px;
    }

    .partner-card h4 {
      font-size: 1.4rem; /* Larger title */
      color: var(--color-medium-text);
      margin-bottom: 2rem;
      font-weight: 500; /* Slightly bolder */
      font-style: italic;
    }

    .partner-card p {
      font-size: 1.1rem; /* Slightly larger text */
      text-align: justify;
      line-height: 1.9;
      color: var(--color-dark-text);
    }

    /* Practice Areas Section */
    #practice-areas {
      padding: 6rem 0;
      background-color: var(--color-white);
      position: relative;
      z-index: 1;
    }

    .practice-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(350px, 1fr)); /* Wider min-width */
      gap: 3rem; /* Increased gap */
      margin-top: 5rem;
    }

    .practice-item {
      background-color: var(--color-white);
      border: 1px solid #eeeeee;
      border-radius: 15px;
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1); /* Deeper shadow */
      padding: 3rem; /* More padding */
      text-align: center;
      transition: transform 0.5s ease, box-shadow 0.5s ease, background-color 0.5s ease;
      position: relative;
      overflow: hidden;
    }

    .practice-item::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 6px;
      background: linear-gradient(to right, var(--color-accent-dark), var(--color-accent-light)); /* Black/White gradient */
      transform: translateY(-100%);
      transition: transform 0.5s ease-out;
    }

    .practice-item:hover::before {
      transform: translateY(0);
    }

    .practice-item:hover {
      transform: translateY(-10px);
      box-shadow: 0 15px 40px rgba(0, 0, 0, 0.2);
      background-color: var(--color-off-white);
    }

    .practice-item i {
      font-size: 4rem; /* Larger icons */
      color: var(--color-accent-dark); /* Dark accent for icons */
      margin-bottom: 2.5rem; /* More space */
      transition: color 0.4s ease;
    }

    .practice-item:hover i {
      color: var(--color-accent-light); /* Light accent on hover */
    }

    .practice-item h3 {
      font-size: 2rem; /* Larger heading */
      color: var(--color-primary-dark);
      margin-bottom: 1.5rem;
      font-weight: 700;
      letter-spacing: 0.8px;
    }

    .practice-item p {
      font-size: 1.05rem;
      color: var(--color-medium-text);
      line-height: 1.8;
    }

    /* Contact Section */
    #contact {
      padding: 6rem 0;
      background-color: var(--color-off-white);
      position: relative;
      z-index: 1;
    }

    .contact-content {
      display: flex;
      flex-wrap: wrap;
      gap: 4rem; /* Increased gap */
      justify-content: center;
    }

    .contact-info, .contact-form-container {
      flex: 1;
      min-width: 400px; /* Wider min-width for better form layout */
      background-color: var(--color-white);
      padding: 3.5rem; /* More padding */
      border-radius: 15px;
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
    }

    .contact-info h3, .contact-form-container h3 {
      font-size: 2.8rem; /* Larger heading */
      color: var(--color-primary-dark);
      margin-bottom: 2.5rem; /* More space */
      text-align: center;
      font-weight: 700;
    }

    .contact-info p {
      margin-bottom: 1.5rem;
      font-size: 1.2rem; /* Larger text */
      display: flex;
      align-items: flex-start;
      color: var(--color-dark-text);
    }

    .contact-info p i {
      color: var(--color-accent-dark); /* Dark accent for icons */
      margin-right: 20px; /* More space for icon */
      font-size: 1.6rem; /* Larger icon */
      flex-shrink: 0;
      padding-top: 0.2rem;
    }

    .contact-form label {
      display: block;
      margin-bottom: 1rem; /* More space */
      font-weight: 600;
      color: var(--color-dark-text);
      font-size: 1.1rem;
    }

    .contact-form input,
    .contact-form textarea {
      width: calc(100% - 28px); /* Account for padding */
      padding: 14px; /* More padding */
      margin-bottom: 1.8rem; /* More space */
      border: 1px solid #cccccc;
      border-radius: 10px; /* More rounded */
      font-family: 'Inter', sans-serif;
      font-size: 1.1rem;
      transition: border-color 0.3s ease, box-shadow 0.3s ease;
    }

    .contact-form input:focus,
    .contact-form textarea:focus {
      border-color: var(--color-accent-dark); /* Dark accent focus glow */
      box-shadow: 0 0 0 4px rgba(0, 0, 0, 0.2); /* Stronger glow */
      outline: none;
    }

    .contact-form textarea {
      resize: vertical;
      min-height: 150px; /* Taller textarea */
    }

    .contact-form button {
      background: linear-gradient(to right, var(--color-accent-dark), var(--color-accent-light));
      color: var(--color-white);
      padding: 16px 35px; /* More padding */
      border: none;
      border-radius: 10px; /* More rounded */
      font-size: 1.3rem; /* Larger text */
      font-weight: 700;
      cursor: pointer;
      transition: background-color 0.4s ease, transform 0.4s ease, box-shadow 0.4s ease;
      box-shadow: 0 8px 20px rgba(0, 0, 0, 0.4); /* Stronger shadow */
      letter-spacing: 0.8px;
      display: block;
      width: 100%;
      max-width: 350px;
      margin: 0 auto 2rem auto;
    }

    .contact-form button:hover {
      background: linear-gradient(to left, var(--color-accent-dark), var(--color-accent-light));
      transform: translateY(-5px); /* More pronounced lift */
      box-shadow: 0 12px 25px rgba(0, 0, 0, 0.5);
    }

    .google-map {
      width: 100%;
      height: 500px; /* Taller map */
      border-radius: 15px;
      overflow: hidden;
      margin-top: 4rem;
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
      border: 1px solid #eee;
    }

    .google-map iframe {
      width: 100%;
      height: 100%;
      border: 0;
    }

    /* Blog Section (Placeholder) */
    #blog {
      padding: 6rem 0;
      background-color: var(--color-white);
      text-align: center;
      position: relative;
      z-index: 1;
    }

    #blog > p {
      max-width: 1000px;
      margin: 0 auto 4rem auto;
      font-size: 1.2rem;
      color: var(--color-medium-text);
      line-height: 1.9;
    }

    /* LLM Feature Containers */
    .llm-feature-container {
      background-color: var(--color-off-white);
      border-radius: 15px;
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
      padding: 3.5rem;
      margin: 5rem auto 0 auto; /* Top margin to separate from blog intro */
      max-width: 900px;
      text-align: left;
      border: 1px solid #eee;
      position: relative;
      overflow: hidden;
    }

    .llm-feature-container::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 8px; /* Accent top border */
      background: linear-gradient(to right, var(--color-accent-dark), var(--color-accent-light));
      border-radius: 15px 15px 0 0;
    }

    .llm-feature-container h3 {
      font-size: 2.8rem;
      color: var(--color-primary-dark);
      margin-bottom: 2rem;
      text-align: center;
      position: relative;
      padding-bottom: 0.8rem;
      font-weight: 700;
      letter-spacing: 1px;
    }

    .llm-feature-container h3::after {
      content: '';
      position: absolute;
      left: 50%;
      bottom: 0;
      transform: translateX(-50%);
      width: 80px;
      height: 3px;
      background-color: var(--color-accent-dark);
      border-radius: 5px;
    }

    .llm-feature-container textarea {
      width: calc(100% - 28px);
      padding: 14px;
      margin-bottom: 2rem;
      border: 1px solid #cccccc;
      border-radius: 10px;
      font-family: 'Inter', sans-serif;
      font-size: 1.1rem;
      min-height: 120px;
      resize: vertical;
      transition: border-color 0.3s ease, box-shadow 0.3s ease;
    }

    .llm-feature-container textarea:focus {
      border-color: var(--color-accent-dark);
      box-shadow: 0 0 0 4px rgba(0, 0, 0, 0.2);
      outline: none;
    }

    .llm-feature-container button {
      background: linear-gradient(to right, var(--color-accent-dark), var(--color-accent-light));
      color: var(--color-white);
      padding: 14px 30px;
      border: none;
      border-radius: 10px;
      font-size: 1.2rem;
      font-weight: 700;
      cursor: pointer;
      transition: background-color 0.4s ease, transform 0.4s ease, box-shadow 0.4s ease;
      box-shadow: 0 6px 15px rgba(0, 0, 0, 0.3);
      letter-spacing: 0.5px;
      display: block;
      width: 100%;
      max-width: 350px;
      margin: 0 auto 2rem auto;
    }

    .llm-feature-container button:hover {
      background: linear-gradient(to left, var(--color-accent-dark), var(--color-accent-light));
      transform: translateY(-3px);
      box-shadow: 0 8px 20px rgba(0, 0, 0, 0.4);
    }

    .llm-output-area {
      background-color: var(--color-white);
      border: 1px solid #e0e0e0;
      border-radius: 10px;
      padding: 2rem;
      min-height: 150px;
      margin-top: 2rem;
      font-size: 1.05rem;
      line-height: 1.8;
      color: var(--color-dark-text);
      text-align: justify;
      box-shadow: inset 0 3px 10px rgba(0, 0, 0, 0.08);
      position: relative;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column; /* For loader and text */
    }

    .loader {
      border: 8px solid #f3f3f3;
      border-top: 8px solid var(--color-accent-dark); /* Dark accent for loader */
      border-radius: 50%;
      width: 60px;
      height: 60px;
      animation: spin 1.2s linear infinite;
      display: none;
      margin-bottom: 1rem; /* Space below loader */
    }

    .llm-output-area.loading .loader {
      display: block;
    }

    .llm-output-area.loading #output-text,
    .llm-output-area.loading #term-output-text { /* Hide text when loading */
        display: none;
    }

    @keyframes spin {
      0% { transform: rotate(0deg); }
      100% { transform: rotate(360deg); }
    }

    .disclaimer {
      font-size: 0.9rem;
      color: #777;
      margin-top: 2.5rem;
      text-align: center;
      font-style: italic;
      padding: 0 1.5rem;
      line-height: 1.6;
    }

    /* Footer */
    footer {
      background: linear-gradient(to right, var(--color-primary-dark), var(--color-secondary-dark));
      color: var(--color-light-grey);
      text-align: center;
      padding: 3.5rem 0; /* More padding */
      font-size: 1rem;
      border-top: 1px solid var(--color-accent-dark); /* Dark accent border */
      box-shadow: 0 -6px 20px rgba(0, 0, 0, 0.3);
    }

    footer .footer-links {
      margin-bottom: 1.8rem; /* More space */
    }

    footer .footer-links a {
      color: var(--color-light-grey); /* Lighter grey for footer links */
      text-decoration: none;
      margin: 0 18px; /* More spacing between links */
      transition: color 0.3s ease, transform 0.3s ease;
      font-weight: 600;
      letter-spacing: 0.5px;
    }

    footer .footer-links a:hover {
      color: var(--color-white);
      transform: translateY(-3px);
    }

    /* Responsive Adjustments */
    @media (max-width: 1200px) {
        .container {
            padding: 3rem 1.5rem;
        }
        .section-title {
            font-size: 3.5rem;
        }
        .hero h2 {
            font-size: 4.5rem;
        }
        .hero p {
            font-size: 1.6rem;
        }
    }

    @media (max-width: 992px) {
      .section-title {
        font-size: 3rem;
        margin-bottom: 4rem;
      }
      .hero h2 {
        font-size: 3.8rem;
        margin-bottom: 1.5rem;
      }
      .hero p {
        font-size: 1.4rem;
      }
      .partner-card {
        max-width: 48%;
      }
      .contact-info, .contact-form-container {
        min-width: 48%;
      }
      .llm-feature-container {
        max-width: 80%;
      }
    }

    @media (max-width: 768px) {
      header h1 {
        font-size: 3.2rem;
        letter-spacing: 2px;
      }
      header p {
        font-size: 1rem;
      }
      nav a {
        padding: 0.8rem 1.2rem;
        font-size: 1rem;
        letter-spacing: 0.5px;
      }
      .hero {
        padding: 8rem 1.5rem;
        min-height: 500px;
      }
      .hero h2 {
        font-size: 2.8rem;
        letter-spacing: 1px;
      }
      .hero p {
        font-size: 1.1rem;
      }
      .section-title {
        font-size: 2.5rem;
        margin-bottom: 3rem;
        padding-bottom: 1.5rem;
      }
      .section-title::after {
        width: 100px;
        height: 4px;
      }
      #about, #team, #practice-areas, #contact, #blog {
        padding: 4rem 0;
      }
      #about p, .team-intro, #blog > p {
        font-size: 1.05rem;
        line-height: 1.8;
      }
      .partner-card-container {
        flex-direction: column;
        align-items: center;
        gap: 2.5rem;
      }
      .partner-card {
        max-width: 90%;
        padding: 2.5rem;
      }
      .partner-card img {
        width: 150px;
        height: 150px;
        margin-bottom: 2rem;
      }
      .partner-card h3 {
        font-size: 2rem;
      }
      .partner-card h4 {
        font-size: 1.2rem;
      }
      .partner-card p {
        font-size: 1rem;
      }
      .practice-grid {
        grid-template-columns: 1fr;
        gap: 2rem;
        margin-top: 3rem;
      }
      .practice-item {
        padding: 2.5rem;
      }
      .practice-item i {
        font-size: 3.5rem;
        margin-bottom: 2rem;
      }
      .practice-item h3 {
        font-size: 1.8rem;
      }
      .contact-content {
        flex-direction: column;
        gap: 2.5rem;
      }
      .contact-info, .contact-form-container {
        min-width: 90%;
        padding: 2.5rem;
      }
      .contact-info h3, .contact-form-container h3 {
        font-size: 2.2rem;
        margin-bottom: 1.8rem;
      }
      .contact-info p {
        font-size: 1.05rem;
      }
      .contact-form label {
        font-size: 1rem;
      }
      .contact-form input, .contact-form textarea {
        padding: 12px;
        font-size: 1rem;
        margin-bottom: 1.5rem;
      }
      .contact-form button {
        padding: 12px 25px;
        font-size: 1.1rem;
        max-width: 250px;
      }
      .google-map {
        height: 350px;
        margin-top: 3rem;
      }
      .llm-feature-container {
        padding: 2.5rem;
        margin: 3rem auto 0 auto;
        max-width: 90%;
      }
      .llm-feature-container h3 {
        font-size: 2rem;
        margin-bottom: 1.5rem;
      }
      .llm-feature-container textarea {
        min-height: 100px;
      }
      .llm-feature-container button {
        max-width: 280px;
      }
      .llm-output-area {
        padding: 1.5rem;
        min-height: 100px;
      }
      .loader {
        width: 50px;
        height: 50px;
        border-width: 5px;
      }
      .disclaimer {
        font-size: 0.8rem;
        margin-top: 1.5rem;
      }
      footer {
        padding: 2.5rem 0;
      }
      footer .footer-links a {
        margin: 0 10px;
      }
    }

    @media (max-width: 480px) {
      header h1 {
        font-size: 2.5rem;
      }
      header p {
        font-size: 0.85rem;
      }
      .hero {
        padding: 6rem 1rem;
        min-height: 400px;
      }
      .hero h2 {
        font-size: 2.2rem;
      }
      .hero p {
        font-size: 0.95rem;
      }
      .section-title {
        font-size: 2rem;
        margin-bottom: 2.5rem;
      }
      .section-title::after {
        width: 80px;
      }
      .container {
        padding: 1.5rem;
      }
      nav {
        flex-direction: column;
        align-items: center;
      }
      nav a {
        width: 100%;
        text-align: center;
        border-bottom: 1px solid rgba(0, 0, 0, 0.1);
      }
      nav a:last-child {
        border-bottom: none;
      }
      .partner-card, .practice-item, .contact-info, .contact-form-container {
        padding: 1.5rem;
        border-radius: 10px;
      }
      .partner-card img {
        width: 100px;
        height: 100px;
        border-width: 4px;
      }
      .partner-card h3 {
        font-size: 1.6rem;
      }
      .partner-card h4 {
        font-size: 1.05rem;
      }
      .partner-card p {
        font-size: 0.9rem;
      }
      .practice-item i {
        font-size: 3rem;
      }
      .practice-item h3 {
        font-size: 1.6rem;
      }
      .contact-info h3, .contact-form-container h3 {
        font-size: 1.8rem;
      }
      .contact-info p {
        font-size: 0.95rem;
      }
      .contact-info p i {
        font-size: 1.2rem;
      }
      .contact-form input, .contact-form textarea {
        padding: 10px;
        font-size: 0.95rem;
      }
      .contact-form button {
        padding: 10px 20px;
        font-size: 1rem;
        max-width: 200px;
      }
      .google-map {
        height: 300px;
      }
      .llm-feature-container {
        padding: 1.8rem;
        margin: 2.5rem auto 0 auto;
      }
      .llm-feature-container h3 {
        font-size: 1.6rem;
      }
      .llm-feature-container textarea {
        min-height: 80px;
      }
      .llm-feature-container button {
        max-width: 220px;
      }
      .llm-output-area {
        padding: 1.2rem;
        min-height: 80px;
        font-size: 0.9rem;
      }
      .loader {
        width: 40px;
        height: 40px;
        border-width: 4px;
      }
    }
  </style>
</head>
<body>

  <header>
    <h1>RR LEGAL SOLUTIONS</h1>
    <p>VOX LEGIS, OPUS VICTORIAE</p>
  </header>

  <nav>
    <a href="#about">About Us</a>
    <a href="#team">Our Team</a>
    <a href="#practice-areas">Practice Areas</a>
    <a href="#contact">Contact Us</a>
    <a href="#blog">Insights</a>
  </nav>

  <section class="hero" id="home">
    <div class="hero-content">
      <h2>Where Legal Acumen Meets Definitive Resolution</h2>
      <p>Guiding you through complexity with strategic brilliance and an unwavering commitment to justice.</p>
    </div>
  </section>

  <section id="about" class="container">
    <h2 class="section-title">About RR Legal Solutions</h2>
    <p>RR Legal Solutions represents the zenith of legal advocacy, where profound experience converges with an audacious pursuit of justice. For over two decades, we have cultivated a reputation for transforming legal challenges into triumphs, operating with an unparalleled blend of sophistication and relentless dedication.</p>
    <p>We are masters of clarity amidst complexity. Our distinguished practice extends across the foundational pillars of Civil Law, with a highly specialized focus on the precise and potent strategies required for Debt Recovery. Our command of Company Law ensures comprehensive guidance through corporate governance, compliance, and growth. Crucially, our deep-seated proficiency in Alternative Dispute Resolution (ADR), particularly Arbitration, underscores our capacity to engineer swift, equitable, and definitive resolutions, offering judicious alternatives to protracted court battles.</p>
    <p>Our raison d'être is simple yet profound: to deliver expertly tailored solutions and to serve the unyielding tenets of justice. We approach each mandate with intellectual rigour and a client-centric ethos, ensuring that your interests are not merely represented, but decisively advanced. With RR Legal Solutions, expect not just legal service, but a partnership dedicated to achieving your optimal outcome.</p>
  </section>

  <section id="team" class="container">
    <h2 class="section-title">Our Visionary Partners</h2>
    <p class="team-intro">At the heart of RR Legal Solutions stands a formidable partnership, a dual force whose collective sagacity and strategic brilliance define the firm's unparalleled standing. Advocates Rajesh Sharma and Ravi Data are the professionals of landmark resolutions, guiding clients through the labyrinth of law with precision, power, and an unyielding commitment to justice. Their individual brilliance, synergistically combined, forms the very bedrock of the firm's distinguished legacy.</p>

    <div class="partner-card-container">
      <div class="partner-card">
        <img src="https://placehold.co/200x200/0A0A0A/FDFDFD?text=Rajesh+Sharma" alt="Advocate Rajesh Sharma">
        <h3>Advocate Rajesh Sharma</h3>
        <h4>Partner & Luminary of Legal Strategy</h4>
        <p>Mr. Sharma is widely revered as a preeminent authority in civil litigation, a legal luminary whose strategic brilliance and profound command of the law consistently define favorable legal landscapes. With a distinguished career spanning over two+ decades, Mr. Sharma possesses an extraordinary acumen for deconstructing intricate legal challenges, identifying pivotal leverage points, and meticulously crafting pathways to definitive resolution.</p>
        <p>His expertise is particularly vibrant in the dynamic arena of debt recovery, where his strategic foresight and rigorous application of civil law principles have consistently transformed complex financial disputes into meticulously secured outcomes. Beyond the courtroom, Advocate Sharma's true hallmark lies in his exceptional drafting prowess. He is celebrated for his ability to translate the most convoluted legal intricacies into documents of unparalleled clarity, precision, and persuasive power. Each pleading, contract, or legal instrument he crafts is a testament to his intellectual rigor and his meticulous attention to detail, designed not merely to articulate a position but to fundamentally shape the trajectory of a case. This skill ensures that the foundational legal arguments are not just sound, but powerfully articulated, setting the stage for success.</p>
        <p>Advocate Sharma's professional ethos is rooted in a steadfast commitment to client welfare and the uncompromising pursuit of justice, embodying the principle that intelligent legal strategy, precisely articulated, is the cornerstone of every triumph.</p>
      </div>

      <div class="partner-card">
        <img src="https://placehold.co/200x200/0A0A0A/FDFDFD?text=Ravi+Data" alt="Advocate Ravi Data">
        <h3>Advocate Ravi Data</h3>
        <h4>Partner & Virtuoso of Resolution</h4>
        <p>Mr. Data stands as a distinguished specialist in corporate jurisprudence and a pivotal force in the realm of ADR. Mr. Data's extensive experience, cultivated over many years, positions him as a trusted advisor capable of navigating the multifaceted challenges confronting modern enterprises. His profound experience in Civil Law extends beyond conventional compliance, encompassing sophisticated counsel on corporate governance, complex transactional frameworks, and strategic business expansion.</p>
        <p>A defining facet of Advocate Data's practice is his exceptional proficiency in Alternative Dispute Resolution, particularly his highly respected acumen in Arbitration. He is adept at steering parties toward pragmatic and equitable solutions, often pre-empting the protracted nature of traditional litigation. His approach is characterized by incisive legal analysis combined with a refined diplomatic sensibility, enabling the construction of definitive resolutions that are both legally sound and commercially advantageous. Advocate Data's commitment to expedited justice ensures that clients achieve efficient and effective outcomes, safeguarding their resources and facilitating their forward momentum.</p>
      </div>
    </div>
  </section>

  <section id="practice-areas" class="container">
    <h2 class="section-title">Our Areas of Expertise</h2>
    <div class="practice-grid">
      <div class="practice-item">
        <i class="fas fa-gavel"></i>
        <h3>Civil Law</h3>
        <p>Comprehensive representation in all civil disputes, ensuring your rights are protected and justice is served.</p>
      </div>
      <div class="practice-item">
        <i class="fas fa-coins"></i>
        <h3>Debt Recovery</h3>
        <p>Specialized strategies for efficient and effective recovery of outstanding debts, safeguarding your financial interests.</p>
      </div>
      <div class="practice-item">
        <i class="fas fa-building"></i>
        <h3>Company Law</h3>
        <p>Expert counsel on corporate governance, compliance, mergers, acquisitions, and strategic business expansion.</p>
      </div>
      <div class="practice-item">
        <i class="fas fa-handshake"></i>
        <h3>Alternative Dispute Resolution (ADR)</h3>
        <p>Skilled facilitation in mediation and arbitration to achieve swift, equitable, and definitive resolutions.</p>
      </div>
      <div class="practice-item">
        <i class="fas fa-file-contract"></i>
        <h3>Contract Law</h3>
        <p>Drafting, review, and enforcement of contracts to secure your agreements and mitigate risks.</p>
      </div>
      <div class="practice-item">
        <i class="fas fa-balance-scale"></i>
        <h3>General Legal Counsel</h3>
        <p>Proactive legal advice and strategic planning to prevent disputes and ensure long-term compliance.</p>
      </div>
    </div>
  </section>

  <section id="contact" class="container">
    <h2 class="section-title">Connect With Us</h2>
    <div class="contact-content">
      <div class="contact-info">
        <h3>Our Contact Details</h3>
        <p><i class="fas fa-phone-alt"></i> Phone: 011-41528050 / 9810223507 / 9810910916</p>
        <p><i class="fas fa-envelope"></i> Email: <a href="mailto:writetorrlegal@gmail.com" style="color: var(--color-dark-text); text-decoration: none;">writetorrlegal@gmail.com</a></p>
        <p><i class="fas fa-map-marker-alt"></i> Address: D-29, Jangpura Extension, New Delhi</p>
        <p><i class="fas fa-clock"></i> Hours: Monday - Friday, 9:00 AM - 6:00 PM</p>
      </div>
      <div class="contact-form-container">
        <h3>Send Us a Message</h3>
        <form class="contact-form">
          <label for="name">Name:</label>
          <input type="text" id="name" name="name" required>

          <label for="email">Email:</label>
          <input type="email" id="email" name="email" required>

          <label for="subject">Subject:</label>
          <input type="text" id="subject" name="subject">

          <label for="message">Message:</label>
          <textarea id="message" name="message" required></textarea>

          <button type="submit">Send Message</button>
        </form>
      </div>
    </div>
    <div class="google-map">
      <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3503.298242485573!2d77.2480608149174!3d28.58983048243685!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x390ce303d2b0e987%3A0x8f7c9e0a0d4c9e0!2sJangpura%20Extension%2C%20New%20Delhi%2C%20Delhi%20110014%2C%20India!5e0!3m2!1sen!2sus!4v1678901234567!5m2!1sen!2sus" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
    </div>
  </section>

  <section id="blog" class="container">
    <h2 class="section-title">Insights & Articles</h2>
    <p>Stay informed with our latest legal insights, analyses, and thought leadership. Our blog provides valuable perspectives on evolving legal landscapes and practical advice for navigating complex issues.</p>
    <p style="font-style: italic; color: var(--color-medium-text);">*(Content for blog posts will appear here. This section is ready for future updates.)*</p>

    <div id="llm-insight-generator" class="llm-feature-container">
      <h3>Legal Insight Generator ✨</h3>
      <p style="text-align: center; font-size: 1rem; color: var(--color-medium-text); margin-bottom: 2rem;">
        Ask a general legal question and get a concise overview.
      </p>
      <textarea id="legal-query-input" placeholder="e.g., What is the role of arbitration in commercial disputes?" rows="4"></textarea>
      <button id="generate-insight-button">Generate Insight ✨</button>
      <div class="llm-output-area" id="llm-output">
        <div class="loader"></div>
        <p id="output-text"></p>
      </div>
      <p class="disclaimer">
        *Disclaimer: This tool provides general informational insights only and does not constitute legal advice. For specific legal counsel, please contact RR Legal Solutions directly.*
      </p>
    </div>

    <div id="llm-terminology-explainer" class="llm-feature-container">
      <h3>Legal Terminology Explainer ✨</h3>
      <p style="text-align: center; font-size: 1rem; color: var(--color-medium-text); margin-bottom: 2rem;">
        Enter a legal term to get a simplified explanation.
      </p>
      <textarea id="legal-term-input" placeholder="e.g., What is 'Habeas Corpus'?" rows="2"></textarea>
      <button id="explain-term-button">Explain Term ✨</button>
      <div class="llm-output-area" id="llm-term-output">
        <div class="loader"></div>
        <p id="term-output-text"></p>
      </div>
      <p class="disclaimer">
        *Disclaimer: This tool provides general informational explanations only and does not constitute legal advice. For specific legal counsel, please contact RR Legal Solutions directly.*
      </p>
    </div>

  </section>

  <footer>
    <div class="container">
      <p>© 2025 RR Legal Solutions. All Rights Reserved.</p>
      <div class="footer-links">
        <a href="#about">About</a> |
        <a href="#team">Team</a> |
        <a href="#practice-areas">Services</a> |
        <a href="#contact">Contact</a>
      </div>
    </div>
  </footer>

  <script>
    document.addEventListener('DOMContentLoaded', () => {
      // --- Legal Insight Generator ---
      const queryInput = document.getElementById('legal-query-input');
      const generateButton = document.getElementById('generate-insight-button');
      const llmOutputArea = document.getElementById('llm-output');
      const outputText = document.getElementById('output-text');
      const loaderInsight = llmOutputArea.querySelector('.loader');

      generateButton.addEventListener('click', async () => {
        const prompt = queryInput.value.trim();
        if (!prompt) {
          outputText.textContent = "Please enter a legal question to generate an insight.";
          return;
        }

        // Show loading indicator
        llmOutputArea.classList.add('loading');
        loaderInsight.style.display = 'block';
        outputText.textContent = ''; // Clear previous output

        try {
          let chatHistory = [];
          chatHistory.push({ role: "user", parts: [{ text: `Provide a concise, high-level overview (max 150 words) on the following legal query, suitable for a general audience on a law firm's website. Focus on key concepts and avoid specific legal advice: "${prompt}"` }] });
          const payload = { contents: chatHistory };
          const apiKey = ""; // Leave as empty string; Canvas will provide at runtime.
          const apiUrl = `https://generativelanguage.googleapis.com/v1beta/models/gemini-2.0-flash:generateContent?key=${apiKey}`;

          const response = await fetch(apiUrl, {
            method: 'POST',
            headers: { 'Content-Type': 'application/json' },
            body: JSON.stringify(payload)
          });

          const result = await response.json();

          if (result.candidates && result.candidates.length > 0 &&
              result.candidates[0].content && result.candidates[0].content.parts &&
              result.candidates[0].content.parts.length > 0) {
            const text = result.candidates[0].content.parts[0].text;
            outputText.textContent = text;
          } else {
            outputText.textContent = "Sorry, I couldn't generate an insight for that query. Please try rephrasing.";
            console.error("Gemini API response structure unexpected:", result);
          }
        } catch (error) {
          outputText.textContent = "An error occurred while fetching the insight. Please try again later.";
          console.error("Error calling Gemini API:", error);
        } finally {
          // Hide loading indicator
          llmOutputArea.classList.remove('loading');
          loaderInsight.style.display = 'none';
        }
      });

      // --- Legal Terminology Explainer ---
      const termInput = document.getElementById('legal-term-input');
      const explainButton = document.getElementById('explain-term-button');
      const llmTermOutputArea = document.getElementById('llm-term-output');
      const termOutputText = document.getElementById('term-output-text');
      const loaderTerm = llmTermOutputArea.querySelector('.loader');

      explainButton.addEventListener('click', async () => {
        const term = termInput.value.trim();
        if (!term) {
          termOutputText.textContent = "Please enter a legal term to get an explanation.";
          return;
        }

        // Show loading indicator
        llmTermOutputArea.classList.add('loading');
        loaderTerm.style.display = 'block';
        termOutputText.textContent = ''; // Clear previous output

        try {
          let chatHistory = [];
          chatHistory.push({ role: "user", parts: [{ text: `Explain the legal term "${term}" concisely (max 100 words) in simple language suitable for a general audience on a law firm's website. Avoid jargon where possible and do not provide legal advice.` }] });
          const payload = { contents: chatHistory };
          const apiKey = ""; // Leave as empty string; Canvas will provide at runtime.
          const apiUrl = `https://generativelanguage.googleapis.com/v1beta/models/gemini-2.0-flash:generateContent?key=${apiKey}`;

          const response = await fetch(apiUrl, {
            method: 'POST',
            headers: { 'Content-Type': 'application/json' },
            body: JSON.stringify(payload)
          });

          const result = await response.json();

          if (result.candidates && result.candidates.length > 0 &&
              result.candidates[0].content && result.candidates[0].content.parts &&
              result.candidates[0].content.parts.length > 0) {
            const text = result.candidates[0].content.parts[0].text;
            termOutputText.textContent = text;
          } else {
            termOutputText.textContent = "Sorry, I couldn't explain that term. Please try a different one.";
            console.error("Gemini API response structure unexpected:", result);
          }
        } catch (error) {
          termOutputText.textContent = "An error occurred while fetching the explanation. Please try again later.";
          console.error("Error calling Gemini API:", error);
        } finally {
          // Hide loading indicator
          llmTermOutputArea.classList.remove('loading');
          loaderTerm.style.display = 'none';
        }
      });
    });
  </script>

</body>
</html>
