<!DOCTYPE html>
<html lang="sv">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>SyExperten | Skräddarsydd Elegans i Linköping</title>
  <meta name="description" content="SyExperten - Din adress för skräddarsydd lyx i Linköping. Vi förvandlar textil till konstverk med exceptionell hantverksskicklighet.">
  <script src="https://cdn.tailwindcss.com"></script>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  <script>
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            primary: '#0A0A0A', // Deepest black
            secondary: '#D4AF37', // Premium gold
            accent: '#2A2520', // Rich charcoal
            light: '#F5F3F0', // Cream white
            dark: '#1A1715', // Dark charcoal
            beige: '#E8E1D9', // Soft beige
            goldlight: '#F5E6C8' // Light gold accent
          },
          fontFamily: {
            sans: ['"Montserrat"', 'sans-serif'],
            heading: ['"Cormorant Garamond"', 'serif'],
            elegant: ['"Playfair Display"', 'serif'],
            decorative: ['"Bodoni Moda"', 'serif']
          },
          animation: {
            'pulse-slow': 'pulse 4s infinite',
            'float': 'float 6s ease-in-out infinite',
            'fade-in': 'fadeIn 1.5s ease-in',
            'text-glow': 'textGlow 3s ease-in-out infinite alternate'
          },
          keyframes: {
            float: {
              '0%, 100%': { transform: 'translateY(0)' },
              '50%': { transform: 'translateY(-12px)' }
            },
            fadeIn: {
              '0%': { opacity: '0' },
              '100%': { opacity: '1' }
            },
            textGlow: {
              '0%': { 'text-shadow': '0 0 5px rgba(212,175,55,0.3)' },
              '100%': { 'text-shadow': '0 0 15px rgba(212,175,55,0.6)' }
            }
          }
        }
      }
    }
  </script>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@500;600;700&family=Playfair+Display:wght@500;600;700&family=Montserrat:wght@300;400;500&family=Bodoni+Moda:wght@500;600&display=swap');
    
    body {
      background-color: #0A0A0A;
      color: #F5F3F0;
      scroll-behavior: smooth;
    }
    
    .luxury-card {
      transition: all 0.5s cubic-bezier(0.22, 1, 0.36, 1);
      position: relative;
      overflow: hidden;
      border: 1px solid rgba(212, 175, 55, 0.2);
    }
    
    .luxury-card::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: linear-gradient(135deg, rgba(10,10,10,0.7) 0%, rgba(10,10,10,0.3) 100%);
      z-index: 1;
    }
    
    .luxury-card:hover {
      transform: translateY(-10px);
      box-shadow: 0 25px 50px -12px rgba(212, 175, 55, 0.3);
      border-color: rgba(212, 175, 55, 0.4);
    }
    
    .service-content {
      position: relative;
      z-index: 2;
    }
    
    .hero-text {
      text-shadow: 2px 2px 10px rgba(0, 0, 0, 0.5);
    }
    
    .nav-link {
      position: relative;
    }
    
    .nav-link::after {
      content: '';
      position: absolute;
      width: 0;
      height: 1px;
      bottom: -2px;
      left: 0;
      background-color: #D4AF37;
      transition: width 0.4s ease;
    }
    
    .nav-link:hover::after {
      width: 100%;
    }
    
    .gold-divider {
      height: 1px;
      background: linear-gradient(90deg, transparent, #D4AF37, transparent);
    }
    
    .logo-container {
      max-width: 420px;
      margin: 0 auto;
      animation: float 6s ease-in-out infinite;
      filter: drop-shadow(0 4px 12px rgba(0,0,0,0.3));
    }
    
    .bg-luxury-pattern {
      background-image: url("data:image/svg+xml,%3Csvg width='100' height='100' viewBox='0 0 100 100' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M0 0h100v100H0V0zm10 10h80v80H10V10zM20 20h60v60H20V20zM30 30h40v40H30V30zM40 40h20v20H40V40z' fill='%23D4AF37' fill-opacity='0.05' fill-rule='evenodd'/%3E%3C/svg%3E");
    }
    
    .testimonial-card {
      background: linear-gradient(135deg, #1A1715 0%, #0A0A0A 100%);
      border: 1px solid rgba(212, 175, 55, 0.2);
      transition: all 0.4s ease;
    }
    
    .testimonial-card:hover {
      transform: translateY(-5px);
      box-shadow: 0 15px 30px -10px rgba(212, 175, 55, 0.2);
      border-color: rgba(212, 175, 55, 0.4);
    }
    
    .floating-btn {
      box-shadow: 0 8px 32px rgba(212, 175, 55, 0.4);
      transition: all 0.3s ease;
    }
    
    .floating-btn:hover {
      transform: scale(1.1) rotate(10deg);
    }
    
    .scroll-indicator {
      animation: bounce 3s infinite;
    }
    
    @keyframes bounce {
      0%, 20%, 50%, 80%, 100% {transform: translateY(0);}
      40% {transform: translateY(-20px);}
      60% {transform: translateY(-10px);}
    }
    
    .text-glow {
      text-shadow: 0 0 8px rgba(212, 175, 55, 0.4);
    }
    
    .border-gold {
      border-color: rgba(212, 175, 55, 0.3);
    }
    
    .embossed-text {
      text-shadow: 1px 1px 1px rgba(0,0,0,0.3), 
                  0 0 0 rgba(212,175,55,0.8),
                  1px 1px 1px rgba(0,0,0,0.3);
      letter-spacing: 0.05em;
    }
    
    .stitch-effect {
      position: relative;
    }
    
    .stitch-effect::after {
      content: '';
      position: absolute;
      bottom: -10px;
      left: 0;
      width: 100%;
      height: 2px;
      background: linear-gradient(90deg, transparent, #D4AF37, transparent);
      background-size: 10px 2px;
      background-image: linear-gradient(90deg, transparent 0%, transparent 50%, #D4AF37 50%, #D4AF37 100%);
    }
    
    .fabric-texture {
      background-image: url("data:image/svg+xml,%3Csvg width='100' height='100' viewBox='0 0 100 100' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M0 0h100v100H0V0zm10 10h80v80H10V10zM20 20h60v60H20V20zM30 30h40v40H30V30zM40 40h20v20H40V40z' fill='%23D4AF37' fill-opacity='0.02' fill-rule='evenodd'/%3E%3C/svg%3E");
    }

    .golden-underline {
      position: relative;
      display: inline-block;
    }
    
    .golden-underline::after {
      content: '';
      position: absolute;
      bottom: -5px;
      left: 0;
      width: 100%;
      height: 1px;
      background: linear-gradient(90deg, #D4AF37, #F5E6C8, #D4AF37);
      transform: scaleX(0);
      transform-origin: right;
      transition: transform 0.4s ease;
    }
    
    .golden-underline:hover::after {
      transform: scaleX(1);
      transform-origin: left;
    }
    
    .luxury-btn {
      position: relative;
      overflow: hidden;
      z-index: 1;
    }
    
    .luxury-btn::before {
      content: '';
      position: absolute;
      top: 0;
      left: -100%;
      width: 100%;
      height: 100%;
      background: linear-gradient(90deg, transparent, rgba(212, 175, 55, 0.2), transparent);
      transition: all 0.6s ease;
      z-index: -1;
    }
    
    .luxury-btn:hover::before {
      left: 100%;
    }
  </style>
</head>

<!-- Add this script before </body> -->
<script>
  // Function to fetch Google reviews (using a proxy service)
  async function fetchGoogleReviews() {
    try {
      // In a real implementation, you would use:
      // 1. Google Places API (requires API key)
      // 2. A third-party service like Elfsight, Grade.us, etc.
      // 3. Or a simple proxy server to avoid CORS issues
      
      // For demonstration, we'll simulate fetching real reviews
      const reviewsContainer = document.getElementById('google-reviews');
      
      // Simulate API delay
      await new Promise(resolve => setTimeout(resolve, 1000));
      
      // Sample reviews (in a real implementation, these would come from API)
      const sampleReviews = [
        {
          author: "Emma Karlsson",
          rating: 5,
          text: "Fantastisk service! Fattho fixade min favoritklänning som var trasig på ett osynligt sätt. Kommer definitivt tillbaka.",
          date: "2 veckor sedan",
          photo: "https://randomuser.me/api/portraits/women/43.jpg"
        },
        {
          author: "Anders Berg",
          rating: 5,
          text: "Bästa skräddaren i Linköping. Har anpassat flera kostymer åt mig och resultatet är alltid perfekt.",
          date: "1 månad sedan",
          photo: "https://randomuser.me/api/portraits/men/32.jpg"
        },
        {
          author: "Lisa Nordström",
          rating: 5,
          text: "Min bröllopsklänning blev precis som jag drömt om. Professionell service och hög kvalité.",
          date: "3 månader sedan",
          photo: "https://randomuser.me/api/portraits/women/65.jpg"
        }
      ];
      
      // Clear loading skeletons
      reviewsContainer.innerHTML = '';
      
      // Add real reviews
      sampleReviews.forEach(review => {
        const stars = Array.from({length: 5}, (_, i) => 
          `<i class="fas fa-star${i < review.rating ? '' : (i === Math.floor(review.rating) && review.rating % 1 >= 0.5 ? '-half-alt' : '')}"></i>`
        ).join('');
        
        const reviewElement = document.createElement('div');
        reviewElement.className = 'testimonial-card rounded-sm p-10 animate-fade-in';
        reviewElement.innerHTML = `
          <div class="flex items-center mb-4">
            <div class="text-secondary text-xl mr-2">
              ${stars}
            </div>
            <span class="text-sm text-light/60 ml-auto">${review.date}</span>
          </div>
          <p class="text-light/80 mb-6 italic">"${review.text}"</p>
          <div class="flex items-center">
            <div class="w-14 h-14 rounded-full bg-accent overflow-hidden mr-4 border-2 border-secondary">
              <img src="${review.photo}" alt="${review.author}" class="w-full h-full object-cover">
            </div>
            <div>
              <h4 class="font-bold text-light">${review.author}</h4>
              <p class="text-sm text-light/60">Google Recension</p>
            </div>
          </div>
        `;
        
        reviewsContainer.appendChild(reviewElement);
      });
      
    } catch (error) {
      console.error('Error fetching reviews:', error);
      // Fallback to static reviews if API fails
      document.getElementById('google-reviews').innerHTML = `
        <div class="col-span-3 text-center py-10">
          <p class="text-light/80 mb-6">Vi kunde inte ladda recensioner just nu. Besök vår <a href="https://g.co/kgs/m63w7z2" target="_blank" class="text-secondary hover:underline">Google sida</a> för att läsa vad våra kunder säger.</p>
        </div>
      `;
    }
  }

  // Fetch reviews when page loads
  document.addEventListener('DOMContentLoaded', fetchGoogleReviews);
</script>

<body class="font-sans thread-cursor">

  <!-- Navigationsmeny -->
  <nav class="fixed top-0 w-full bg-primary/95 backdrop-blur-md z-50 border-b border-gold transition-all duration-500">
    <div class="container mx-auto px-6 py-5 flex flex-col md:flex-row justify-between items-center">
      <div class="flex items-center gap-6">
        <div class="text-3xl font-heading font-bold text-light tracking-tight">SYEXPERTEN</div>
        <div class="hidden md:block h-12 border-r border-gold"></div>
        <div class="hidden md:block">
          <img src="SyExpertenVecWhite.svg" alt="SyExperten" class="h-16 transition duration-500 hover:scale-105">
        </div>
      </div>
      
      <div class="flex flex-wrap justify-center gap-10 text-base mt-6 md:mt-0">
        <a href="#tjanster" class="nav-link text-light/90 hover:text-secondary font-medium transition duration-300 flex items-center gap-2">
          <i class="fas fa-scissors text-secondary"></i> Tjänster
        </a>
        <a href="#omoss" class="nav-link text-light/90 hover:text-secondary font-medium transition duration-300 flex items-center gap-2">
          <i class="fas fa-store text-secondary"></i> Om oss
        </a>
        <a href="#oppettider" class="nav-link text-light/90 hover:text-secondary font-medium transition duration-300 flex items-center gap-2">
          <i class="far fa-clock text-secondary"></i> Öppettider
        </a>
        <a href="#kontakt" class="nav-link text-light/90 hover:text-secondary font-medium transition duration-300 flex items-center gap-2">
          <i class="fas fa-map-marker-alt text-secondary"></i> Kontakt
        </a>
      </div>
      
      <div class="hidden md:block">
        <a href="tel:013127200" class="luxury-btn bg-transparent border-2 border-secondary hover:bg-secondary/10 text-secondary font-medium px-6 py-3 rounded-sm transition duration-300 flex items-center gap-3 group">
          <i class="fas fa-phone transform group-hover:scale-110 transition"></i> 
          <span class="transform group-hover:translate-x-1 transition">013-12 72 00</span>
        </a>
      </div>
    </div>
  </nav>

  <!-- Hero-bild -->
  <div class="relative h-screen max-h-[90vh] overflow-hidden bg-luxury-pattern">
    <!-- Background image with enhanced filters -->
    <div class="absolute inset-0">
      <img src="SyExperten.jpeg" alt="SyExperten" class="w-full h-full object-cover object-center">
      <div class="absolute inset-0 bg-gradient-to-b from-primary/90 via-primary/60 to-primary/90"></div>
      <div class="absolute inset-0 bg-gradient-to-r from-primary/70 to-primary/30"></div>
    </div>
  
    <!-- Content overlay -->
    <div class="absolute inset-0 z-20 flex flex-col items-center justify-center px-4 text-center">
      <!-- Logo with enhanced visibility -->
      <div class="logo-container mb-12 transform transition-all duration-500 hover:scale-105">
        <img src="SyExpertenVecGold.svg" alt="SyExperten Logo" class="w-full h-auto">
      </div>
      
      <!-- Headline with decorative elements -->
      <div class="relative mb-8">
        <h1 class="text-4xl md:text-6xl lg:text-7xl font-heading font-bold text-light max-w-4xl mb-8 leading-tight hero-text animate-fade-in">
          <span class="embossed-text">Skräddarsydd Elegans</span>
        </h1>
        <div class="absolute -bottom-4 left-1/2 transform -translate-x-1/2 w-32 h-1 bg-secondary"></div>
      </div>
      
      <!-- Subheading with golden animation -->
      <p class="text-2xl text-light max-w-2xl mb-12 font-elegant italic animate-text-glow">
        Perfektion i varje stygn sedan 2005
      </p>
      
      <!-- Buttons with luxury effects -->
      <div class="flex flex-wrap gap-6 justify-center">
        <a href="#kontakt" class="luxury-btn bg-secondary hover:bg-opacity-90 text-dark font-bold py-4 px-10 rounded-sm transition duration-300 flex items-center gap-3 group relative overflow-hidden">
          <span class="transform group-hover:translate-x-1 transition">Boka Konsultation</span>
          <i class="fas fa-gem transform group-hover:scale-110 transition"></i>
        </a>
        <a href="#tjanster" class="luxury-btn bg-transparent border-2 border-secondary hover:bg-secondary/10 text-secondary font-bold py-4 px-10 rounded-sm transition duration-300 flex items-center gap-3 group">
          <span class="transform group-hover:translate-x-1 transition">Våra Tjänster</span>
          <i class="fas fa-chevron-down transform group-hover:scale-110 transition"></i>
        </a>
      </div>
      
      <!-- Scroll indicator -->
      <div class="absolute bottom-12 left-1/2 transform -translate-x-1/2">
        <a href="#content-start" class="text-secondary text-2xl scroll-indicator">
          <i class="fas fa-chevron-down"></i>
        </a>
      </div>
    </div>
  </div>

  <!-- Main content anchor -->
  <div id="content-start" class="pt-2"></div>

  <!-- Huvudinnehåll -->
  <main class="max-w-7xl mx-auto px-6 py-20">

    <!-- Välkomsttext -->
    <section class="mb-28 text-center max-w-5xl mx-auto">
      <span class="inline-block text-secondary text-sm font-semibold mb-6 tracking-widest">
        HANDGJORD LYX
      </span>
      <h2 class="text-5xl md:text-6xl font-heading font-bold mb-10 leading-tight text-light">Välkommen till SyExperten</h2>
      <div class="gold-divider max-w-2xl mx-auto my-10"></div>
      <p class="text-xl text-light/80 mb-12 leading-relaxed max-w-4xl mx-auto">
        I hjärtat av Linköping skapar vi skräddarsydda mästerverk som kombinerar tidlös elegans med modern komfort. 
        Varje plagg som lämnar vår ateljé bär på en historia av exceptionellt hantverk och oöverträffad kvalitet.
      </p>
      <div class="flex justify-center">
        <a href="#omoss" class="inline-flex items-center text-secondary font-medium group golden-underline">
          Upptäck vår historia
          <i class="fas fa-arrow-right ml-3 transform group-hover:translate-x-2 transition duration-300"></i>
        </a>
      </div>
    </section>

    <!-- Tjänster -->
    <section id="tjanster" class="mb-32">
      <div class="text-center mb-20">
        <span class="inline-block text-secondary text-sm font-semibold mb-6 tracking-widest">
          VÅRT HANTVERK
        </span>
        <h2 class="text-5xl md:text-6xl font-heading font-bold mb-8 leading-tight text-light stitch-effect">Tjänster</h2>
        <div class="gold-divider max-w-xl mx-auto my-10"></div>
        <p class="text-xl text-light/70 max-w-3xl mx-auto">
          Från diskreta anpassningar till spektakulära specialbeställningar - vi förverkligar dina textildrömmar
        </p>
      </div>
      
      <div class="grid grid-cols-1 lg:grid-cols-3 gap-8">
        <!-- Tjänst 1 - Skräddarsytt arbete -->
        <div class="luxury-card rounded-sm overflow-hidden h-[600px] relative">
          <div class="absolute inset-0 overflow-hidden">
            <img src="https://images.unsplash.com/photo-1598033129183-c4f50c736f10?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1200&q=80" 
                alt="Skräddarsytt arbete" class="w-full h-full object-cover transition duration-700 hover:scale-105">
          </div>
          <div class="absolute bottom-0 left-0 right-0 p-10 text-light service-content">
            <span class="inline-block bg-secondary text-dark px-4 py-2 rounded-sm text-xs font-bold mb-4 tracking-widest">
              MÄTTAGNING
            </span>
            <h3 class="text-3xl font-heading font-bold mb-4">Skräddarsytt Arbete</h3>
            <p class="text-light/80 mb-6">Perfekt anpassning efter dina unika mått och stilpreferenser.</p>
            <a href="#kontakt" class="inline-flex items-center text-secondary font-medium group golden-underline">
              Boka Mätning
              <i class="fas fa-arrow-right ml-3 transform group-hover:translate-x-2 transition duration-300"></i>
            </a>
          </div>
        </div>
        
        <!-- Tjänst 2 - Reparation & Lagning -->
        <div class="luxury-card rounded-sm overflow-hidden h-[600px] relative">
          <div class="absolute inset-0 overflow-hidden">
            <img src="https://images.unsplash.com/photo-1607346256330-dee7af15f7c5?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1200&q=80" 
                alt="Reparationer" class="w-full h-full object-cover transition duration-700 hover:scale-105">
          </div>
          <div class="absolute bottom-0 left-0 right-0 p-10 text-light service-content">
            <span class="inline-block bg-secondary text-dark px-4 py-2 rounded-sm text-xs font-bold mb-4 tracking-widest">
              RESTAURERING
            </span>
            <h3 class="text-3xl font-heading font-bold mb-4">Reparation & Lagning</h3>
            <p class="text-light/80 mb-6">Expertis som ger dina favoritplagg nytt liv med osynliga ingrepp.</p>
            <a href="#kontakt" class="inline-flex items-center text-secondary font-medium group golden-underline">
              Få Kostnadsförslag
              <i class="fas fa-arrow-right ml-3 transform group-hover:translate-x-2 transition duration-300"></i>
            </a>
          </div>
        </div>
        
        <!-- Tjänst 3 - Specialarbeten -->
        <div class="luxury-card rounded-sm overflow-hidden h-[600px] relative">
          <div class="absolute inset-0 overflow-hidden">
            <img src="https://images.unsplash.com/photo-1539109136881-3be0616acf4b?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1200&q=80" 
                alt="Specialarbeten" class="w-full h-full object-cover transition duration-700 hover:scale-105">
          </div>
          <div class="absolute bottom-0 left-0 right-0 p-10 text-light service-content">
            <span class="inline-block bg-secondary text-dark px-4 py-2 rounded-sm text-xs font-bold mb-4 tracking-widest">
              HAUTE COUTURE
            </span>
            <h3 class="text-3xl font-heading font-bold mb-4">Specialarbeten</h3>
            <p class="text-light/80 mb-6">Unika kreationer för bröllop, galor och speciella tillfällen.</p>
            <a href="#kontakt" class="inline-flex items-center text-secondary font-medium group golden-underline">
              Boka Konsultation
              <i class="fas fa-arrow-right ml-3 transform group-hover:translate-x-2 transition duration-300"></i>
            </a>
          </div>
        </div>
      </div>
    </section>

    <!-- Om oss -->
    <section id="omoss" class="mb-32 py-24 bg-accent relative overflow-hidden">
      <!-- Sophisticated grain texture (almost invisible but adds depth) -->
      <div class="absolute inset-0 bg-[url('data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxMDAiIGhlaWdodD0iMTAwIiB2aWV3Qm94PSIwIDAgMTAwIDEwMCI+PGRlZnM+PGZpbHRlciBpZD0ibm9pc2UiIHg9IjAiIHk9IjAiIHdpZHRoPSIxMDAlIiBoZWlnaHQ9IjEwMCUiPjxmZVR1cmJ1bGVuY2UgdHlwZT0iZnJhY3RhbE5vaXNlIiBiYXNlRnJlcXVlbmN5PSIwLjA1IiBudW1PY3RhdmVzPSIzIiBzdGl0Y2hUaWxlcz0ic3RpdGNoIi8+PGZlQ29sb3JNYXRyaXggdHlwZT0ic2F0dXJhdGUiIHZhbHVlcz0iMCIvPjwvZmlsdGVyPjwvZGVmcz48cmVjdCB3aWR0aD0iMTAwJSIgaGVpZ2h0PSIxMDAlIiBmaWx0ZXI9InVybCgjbm9pc2UpIiBvcGFjaXR5PSIwLjAzIi8+PC9zdmc+')] opacity-10"></div>
      
      <div class="max-w-7xl mx-auto px-6 relative z-10">
        <div class="grid grid-cols-1 lg:grid-cols-2 gap-16 items-center">
          <div class="order-2 lg:order-1">
            <span class="inline-block text-secondary text-sm font-semibold mb-6 tracking-widest">
              VÅR FILOSOFI
            </span>
            <h2 class="text-5xl md:text-6xl font-heading font-bold mb-10 leading-tight text-light stitch-effect">Konsten Att Skapa</h2>
            <div class="gold-divider max-w-md my-10"></div>
            <div class="space-y-6 text-lg text-light/80">
              <p>Sedan vår grundande har vi dedikerat oss till att bevara och utveckla det äkta skräddarhantverket. Varje plagg som lämnar vår ateljé bär på en historia av noggrannhet och passion.</p>
              <p>Vår vision sträcker sig bortom vanlig skräddarsydd - vi skapar kläder som inte bara passar perfekt, men som också förmedlar en känsla av unik elegans och självförtroende.</p>
              <p>Med en kombination av traditionella tekniker och moderna innovationer säkerställer vi att varje detalj är perfekt.</p>
            </div>
            <div class="flex flex-wrap gap-4 mt-12">
              <span class="inline-flex items-center gap-3 bg-primary/30 px-6 py-3 rounded-sm text-sm font-medium border border-gold hover:bg-secondary/10 hover:border-secondary/50 transition">
                <i class="fas fa-check-circle text-secondary text-glow"></i> Expertis sedan 2005
              </span>
              <span class="inline-flex items-center gap-3 bg-primary/30 px-6 py-3 rounded-sm text-sm font-medium border border-gold hover:bg-secondary/10 hover:border-secondary/50 transition">
                <i class="fas fa-check-circle text-secondary text-glow"></i> Exklusiva Material
              </span>
              <span class="inline-flex items-center gap-3 bg-primary/30 px-6 py-3 rounded-sm text-sm font-medium border border-gold hover:bg-secondary/10 hover:border-secondary/50 transition">
                <i class="fas fa-check-circle text-secondary text-glow"></i> Personlig Service
              </span>
            </div>
          </div>
          <div class="order-1 lg:order-2 relative rounded-sm overflow-hidden shadow-2xl h-[700px] border border-gold">
            <div class="absolute inset-0 bg-gradient-to-t from-dark/70 via-dark/30 to-transparent z-10"></div>
            <img src="https://images.unsplash.com/photo-1597677208174-68347ef1e7dc?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1200&q=80" 
                  alt="Vår verkstad" class="w-full h-full object-cover">
            <div class="absolute bottom-0 left-0 right-0 p-10 z-20">
              <div class="bg-primary/90 backdrop-blur-sm border border-gold text-light p-8 max-w-md">
                <h3 class="font-heading text-3xl font-bold mb-3">Möt Vår Mästerskräddare</h3>
                <p class="mb-6 text-light/80">Fattho Abdul Ahad, med över 20 års erfarenhet av högklassig skräddarsydd, leder vårt team av hantverkare.</p>
                <a href="#kontakt" class="inline-flex items-center text-secondary font-medium group golden-underline">
                  Boka Rådgivning
                  <i class="fas fa-arrow-right ml-3 transform group-hover:translate-x-2 transition duration-300"></i>
                </a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Replace the Testimonials section with this code -->
    <section class="mb-32">
      <div class="max-w-7xl mx-auto px-6">
        <div class="text-center mb-20">
          <span class="inline-block text-secondary text-sm font-semibold mb-6 tracking-widest">
            VÅRA KUNDERS RÖSTER
          </span>
          <h2 class="text-5xl md:text-6xl font-heading font-bold mb-8 leading-tight text-light stitch-effect">Kundrecensioner</h2>
          <div class="gold-divider max-w-xl mx-auto my-10"></div>
          <p class="text-xl text-light/70 max-w-3xl mx-auto">
            Vad våra nöjda kunder säger om oss
          </p>
        </div>
        
        <!-- Reviews Container -->
        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
          <!-- Review 1 -->
          <div class="testimonial-card rounded-sm p-10">
            <div class="flex items-center mb-4">
              <div class="text-secondary text-xl mr-2">
                <i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i>
              </div>
              <span class="text-sm text-light/60 ml-auto">2 veckor sedan</span>
            </div>
            <p class="text-light/80 mb-6 italic">"Fantastisk service! Fattho fixade min favoritklänning som var trasig på ett osynligt sätt. Kommer definitivt tillbaka."</p>
            <div class="flex items-center">
              <div class="w-14 h-14 rounded-full bg-accent overflow-hidden mr-4 border-2 border-secondary">
                <img src="https://randomuser.me/api/portraits/women/43.jpg" alt="Emma Karlsson" class="w-full h-full object-cover">
              </div>
              <div>
                <h4 class="font-bold text-light">Emma Karlsson</h4>
                <p class="text-sm text-light/60">Nöjd kund</p>
              </div>
            </div>
          </div>
          
          <!-- Review 2 -->
          <div class="testimonial-card rounded-sm p-10">
            <div class="flex items-center mb-4">
              <div class="text-secondary text-xl mr-2">
                <i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i>
              </div>
              <span class="text-sm text-light/60 ml-auto">1 månad sedan</span>
            </div>
            <p class="text-light/80 mb-6 italic">"Bästa skräddaren i Linköping. Har anpassat flera kostymer åt mig och resultatet är alltid perfekt."</p>
            <div class="flex items-center">
              <div class="w-14 h-14 rounded-full bg-accent overflow-hidden mr-4 border-2 border-secondary">
                <img src="https://randomuser.me/api/portraits/men/32.jpg" alt="Anders Berg" class="w-full h-full object-cover">
              </div>
              <div>
                <h4 class="font-bold text-light">Anders Berg</h4>
                <p class="text-sm text-light/60">Återkommande kund</p>
              </div>
            </div>
          </div>
          
          <!-- Review 3 -->
          <div class="testimonial-card rounded-sm p-10">
            <div class="flex items-center mb-4">
              <div class="text-secondary text-xl mr-2">
                <i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i>
              </div>
              <span class="text-sm text-light/60 ml-auto">3 månader sedan</span>
            </div>
            <p class="text-light/80 mb-6 italic">"Min bröllopsklänning blev precis som jag drömt om. Professionell service och hög kvalité."</p>
            <div class="flex items-center">
              <div class="w-14 h-14 rounded-full bg-accent overflow-hidden mr-4 border-2 border-secondary">
                <img src="https://randomuser.me/api/portraits/women/65.jpg" alt="Lisa Nordström" class="w-full h-full object-cover">
              </div>
              <div>
                <h4 class="font-bold text-light">Lisa Nordström</h4>
                <p class="text-sm text-light/60">Bröllopskund</p>
              </div>
            </div>
          </div>
        </div>
        
        <!-- Google Badge Link -->
        <div class="text-center mt-16">
          <a href="https://www.google.com/maps/place/Syexperten+I+Linköping/@58.4091145,15.6150206,16z/data=!4m8!3m7!1s0x46596f2327695555:0xd35278e54bd45255!8m2!3d58.4078106!4d15.617338!9m1!1b1!16s%2Fg%2F11fmvl3gff?hl=sv&entry=ttu&g_ep=EgoyMDI1MDQwOS4wIKXMDSoJLDEwMjExNDUzSAFQAw%3D%3D" 
            target="_blank" 
            class="inline-flex items-center bg-primary hover:bg-opacity-90 border border-gold text-light font-bold py-4 px-8 rounded-sm transition duration-300 group">
            <i class="fab fa-google mr-3 text-secondary"></i>
            <span>Lämna en recension på Google</span>
            <i class="fas fa-arrow-right ml-3 transform group-hover:translate-x-2 transition"></i>
          </a>
        </div>
      </div>
    </section>

    <!-- Öppettider -->
    <section id="oppettider" class="mb-32 bg-primary/50 rounded-sm border border-gold p-12 md:p-16 backdrop-blur-sm">
      <div class="max-w-6xl mx-auto">
        <div class="text-center mb-16">
          <h2 class="text-5xl md:text-6xl font-heading font-bold mb-8 leading-tight text-light stitch-effect">Besök Vår Ateljé</h2>
          <div class="gold-divider max-w-xl mx-auto my-10"></div>
          <p class="text-xl text-light/70 max-w-3xl mx-auto">
            Vår exklusiva verkstad i Linköpings fina innerstad
          </p>
        </div>
        
        <div class="grid grid-cols-1 lg:grid-cols-2 gap-16">
          <div>
            <h3 class="text-3xl font-heading font-bold mb-8 text-light">Öppettider</h3>
            <ul class="space-y-6">
              <li class="flex justify-between items-center pb-4 border-b border-gold">
                <span class="font-medium text-light">Måndag - Fredag</span>
                <span class="font-semibold text-secondary">10:00 - 18:00</span>
              </li>
              <li class="flex justify-between items-center pb-4 border-b border-gold">
                <span class="font-medium text-light">Lördag</span>
                <span class="font-semibold text-light/40">Stängt</span>
              </li>
              <li class="flex justify-between items-center pb-4 border-b border-gold">
                <span class="font-medium text-light">Söndag</span>
                <span class="font-semibold text-light/40">Stängt</span>
              </li>
            </ul>
            
            <div class="mt-12 bg-secondary/5 border border-secondary/20 rounded-sm p-8">
              <p class="font-medium text-secondary"><i class="fas fa-info-circle mr-3"></i> För bästa service rekommenderar vi att boka tid i förväg via vår bokningsfunktion</p>
            </div>
          </div>
          
          <div>
            <h3 class="text-3xl font-heading font-bold mb-8 text-light">Kontaktinformation</h3>
            <div class="space-y-8">
              <div class="flex items-start gap-6">
                <div class="w-14 h-14 bg-accent text-secondary rounded-full flex items-center justify-center mt-1 border border-gold">
                  <i class="fas fa-map-marker-alt text-xl"></i>
                </div>
                <div>
                  <h4 class="font-bold text-xl text-light mb-2">Ateljé</h4>
                  <p class="text-light/70 mb-3">Elsa Brändströms gata 1<br>582 27 Linköping</p>
                  <a href="https://maps.google.com" target="_blank" class="inline-flex items-center text-secondary font-medium group golden-underline">
                    Visa på karta
                    <i class="fas fa-external-link-alt ml-3 text-xs transform group-hover:translate-x-1 transition"></i>
                  </a>
                </div>
              </div>
              
              <div class="flex items-start gap-6">
                <div class="w-14 h-14 bg-accent text-secondary rounded-full flex items-center justify-center mt-1 border border-gold">
                  <i class="fas fa-phone-alt text-xl"></i>
                </div>
                <div>
                  <h4 class="font-bold text-xl text-light mb-2">Telefon</h4>
                  <p class="text-light/70 mb-4">013-12 72 00</p>
                  <a href="tel:013127200" class="inline-flex bg-secondary text-dark px-6 py-3 rounded-sm font-medium hover:bg-opacity-90 transition items-center gap-3 luxury-btn">
                    <i class="fas fa-phone"></i> 
                    Ring oss direkt
                  </a>
                </div>
              </div>
              
              <div class="flex items-start gap-6">
                <div class="w-14 h-14 bg-accent text-secondary rounded-full flex items-center justify-center mt-1 border border-gold">
                  <i class="fas fa-envelope text-xl"></i>
                </div>
                <div>
                  <h4 class="font-bold text-xl text-light mb-2">E-post</h4>
                  <p class="text-light/70 mb-4">info@syexperten.se</p>
                  <a href="mailto:info@syexperten.se" class="inline-flex bg-primary text-light px-6 py-3 rounded-sm font-medium hover:bg-opacity-90 transition items-center gap-3 border border-gold luxury-btn">
                    <i class="fas fa-envelope"></i> 
                    Skicka meddelande
                  </a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Kontakt -->
    <section id="kontakt" class="mb-32">
      <div class="grid grid-cols-1 lg:grid-cols-2 gap-16 items-center">
        <div class="order-2 lg:order-1">
          <span class="inline-block text-secondary text-sm font-semibold mb-6 tracking-widest">
            BOKNING
          </span>
          <h2 class="text-5xl md:text-6xl font-heading font-bold mb-8 leading-tight text-light stitch-effect">Boka En Privat Konsultation</h2>
          <div class="gold-divider max-w-md my-10"></div>
          <p class="text-xl text-light/70 mb-10">
            Berätta om ditt projekt så återkommer vi med en exklusiv tid och detaljerat kostnadsförslag.
          </p>
          
          <form class="space-y-8">
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
              <div>
                <label for="name" class="block text-sm font-medium text-light/80 mb-2">Namn *</label>
                <input type="text" id="name" name="name" required class="w-full px-5 py-4 bg-primary/30 border border-gold rounded-sm focus:ring-2 focus:ring-secondary focus:border-transparent text-light placeholder-light/30">
              </div>
              <div>
                <label for="email" class="block text-sm font-medium text-light/80 mb-2">E-post *</label>
                <input type="email" id="email" name="email" required class="w-full px-5 py-4 bg-primary/30 border border-gold rounded-sm focus:ring-2 focus:ring-secondary focus:border-transparent text-light placeholder-light/30">
              </div>
            </div>
            
            <div>
              <label for="phone" class="block text-sm font-medium text-light/80 mb-2">Telefon</label>
              <input type="tel" id="phone" name="phone" class="w-full px-5 py-4 bg-primary/30 border border-gold rounded-sm focus:ring-2 focus:ring-secondary focus:border-transparent text-light placeholder-light/30">
            </div>
            
            <div>
              <label for="service" class="block text-sm font-medium text-light/80 mb-2">Tjänst *</label>
              <select id="service" name="service" required class="w-full px-5 py-4 bg-primary/30 border border-gold rounded-sm focus:ring-2 focus:ring-secondary focus:border-transparent text-light">
                <option value="" class="bg-primary">Välj tjänst</option>
                <option value="tailoring" class="bg-primary">Skräddarsytt arbete</option>
                <option value="repair" class="bg-primary">Reparation & lagning</option>
                <option value="special" class="bg-primary">Specialarbeten</option>
                <option value="other" class="bg-primary">Privat rådgivning</option>
              </select>
            </div>
            
            <div>
              <label for="message" class="block text-sm font-medium text-light/80 mb-2">Beskriv ditt projekt *</label>
              <textarea id="message" name="message" rows="5" required class="w-full px-5 py-4 bg-primary/30 border border-gold rounded-sm focus:ring-2 focus:ring-secondary focus:border-transparent text-light placeholder-light/30"></textarea>
            </div>
            
            <button type="submit" class="w-full bg-secondary hover:bg-opacity-90 text-dark font-bold py-5 px-8 rounded-sm transition duration-300 flex items-center justify-center gap-4 group luxury-btn">
              <span class="transform group-hover:translate-x-2 transition">Skicka Förfrågan</span>
              <i class="fas fa-paper-plane transform group-hover:scale-125 transition"></i>
            </button>
          </form>
        </div>
        
        <div class="order-1 lg:order-2 rounded-sm overflow-hidden shadow-2xl h-[700px] border border-gold">
          <iframe 
            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2079.869403873527!2d15.6012223159287!3d58.41090038124695!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x46596bc8b3b8e6d5%3A0x3e8a0d7c8a7a7a7a!2sElsa%20Br%C3%A4ndstr%C3%B6ms%20gata%201%2C%20582%2027%20Link%C3%B6ping!5e0!3m2!1ssv!2sse!4v1620000000000!5m2!1ssv!2sse" 
            width="100%" 
            height="100%" 
            style="border:0;" 
            allowfullscreen="" 
            loading="lazy"
            class="min-h-[400px]"
          ></iframe>
          <div class="absolute bottom-0 left-0 right-0 h-20 bg-gradient-to-t from-primary to-transparent"></div>
        </div>
      </div>
    </section>
  </main>

  <!-- Footer -->
  <footer class="bg-primary text-light pt-24 pb-16 relative border-t border-gold">
    <div class="absolute top-0 left-0 right-0 h-24 bg-gradient-to-b from-secondary/10 to-transparent"></div>
    <div class="max-w-7xl mx-auto px-6 relative z-10">
      <div class="grid grid-cols-1 md:grid-cols-4 gap-12 mb-16">
        <div>
          <div class="flex items-center gap-4 mb-6">
            <div class="text-3xl font-heading font-bold text-light">SYEXPERTEN</div>
            <div class="h-10 border-r border-gold"></div>
            <img src="SyExpertenVecWhite.svg" alt="SyExperten" class="h-10">
          </div>
          <p class="text-light/60 mb-6">Exklusiv skräddarservice i Linköping sedan 2005.</p>
          <div class="flex gap-4">
            <a href="#" class="w-12 h-12 bg-accent hover:bg-secondary rounded-full flex items-center justify-center transition border border-gold text-secondary hover:text-dark">
              <i class="fab fa-facebook-f text-lg"></i>
            </a>
            <a href="#" class="w-12 h-12 bg-accent hover:bg-secondary rounded-full flex items-center justify-center transition border border-gold text-secondary hover:text-dark">
              <i class="fab fa-instagram text-lg"></i>
            </a>
          </div>
        </div>
        
        <div>
          <h3 class="text-lg font-bold mb-6 uppercase tracking-wider text-light">Tjänster</h3>
          <ul class="space-y-3">
            <li><a href="#" class="text-light/60 hover:text-secondary transition flex items-center gap-3">
              <i class="fas fa-chevron-right text-xs text-secondary"></i> Skräddarsytt arbete
            </a></li>
            <li><a href="#" class="text-light/60 hover:text-secondary transition flex items-center gap-3">
              <i class="fas fa-chevron-right text-xs text-secondary"></i> Reparation & lagning
            </a></li>
            <li><a href="#" class="text-light/60 hover:text-secondary transition flex items-center gap-3">
              <i class="fas fa-chevron-right text-xs text-secondary"></i> Specialarbeten
            </a></li>
            <li><a href="#" class="text-light/60 hover:text-secondary transition flex items-center gap-3">
              <i class="fas fa-chevron-right text-xs text-secondary"></i> Bröllopsklänningar
            </a></li>
            <li><a href="#" class="text-light/60 hover:text-secondary transition flex items-center gap-3">
              <i class="fas fa-chevron-right text-xs text-secondary"></i> Kostymanpassning
            </a></li>
          </ul>
        </div>
        
        <div>
          <h3 class="text-lg font-bold mb-6 uppercase tracking-wider text-light">Kontakt</h3>
          <ul class="space-y-4 text-light/60">
            <li class="flex items-start gap-4">
              <i class="fas fa-map-marker-alt mt-1 text-secondary"></i> 
              <span>Elsa Brändströms gata 1<br>582 27 Linköping</span>
            </li>
            <li class="flex items-center gap-4">
              <i class="fas fa-phone-alt text-secondary"></i> 
              <span>013-12 72 00</span>
            </li>
            <li class="flex items-center gap-4">
              <i class="fas fa-envelope text-secondary"></i> 
              <span>info@syexperten.se</span>
            </li>
          </ul>
        </div>
        
        <div>
          <h3 class="text-lg font-bold mb-6 uppercase tracking-wider text-light">Nyhetsbrev</h3>
          <p class="text-light/60 mb-6">Prenumerera för exklusiva erbjudanden och stylingtips.</p>
          <form class="flex">
            <input type="email" placeholder="Din e-post" class="px-5 py-3 w-full rounded-l-sm bg-accent text-light border border-gold focus:ring-2 focus:ring-secondary focus:border-transparent placeholder-light/30">
            <button type="submit" class="bg-secondary text-dark px-5 rounded-r-sm hover:bg-opacity-90 transition border border-secondary">
              <i class="fas fa-paper-plane"></i>
            </button>
          </form>
        </div>
      </div>
      
      <div class="pt-8 border-t border-gold flex flex-col md:flex-row justify-between items-center">
        <p class="text-light/40 text-sm mb-4 md:mb-0">
          &copy; <span id="current-year">2025</span> SyExperten. Alla rättigheter förbehållna.
        </p>
        <div class="flex gap-6">
          <a href="#" class="text-light/40 hover:text-secondary text-sm transition golden-underline">Integritetspolicy</a>
          <a href="#" class="text-light/40 hover:text-secondary text-sm transition golden-underline">Villkor</a>
          <a href="#" class="text-light/40 hover:text-secondary text-sm transition golden-underline">Cookies</a>
        </div>
      </div>
    </div>
  </footer>

  <!-- Floating action button -->
  <a href="#kontakt" class="fixed bottom-8 right-8 w-16 h-16 bg-secondary text-dark rounded-full flex items-center justify-center shadow-2xl hover:bg-opacity-90 transition z-50 floating-btn group">
    <i class="fas fa-calendar-alt text-xl transform group-hover:scale-125 transition"></i>
  </a>

  <script>
    // Add current year to footer
    document.getElementById('current-year').textContent = new Date().getFullYear();
    
    // Smooth scrolling for anchor links
    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
      anchor.addEventListener('click', function (e) {
        e.preventDefault();
        
        document.querySelector(this.getAttribute('href')).scrollIntoView({
          behavior: 'smooth'
        });
      });
    });
    
    // Animate elements when they come into view
    const animateOnScroll = () => {
      const elements = document.querySelectorAll('.luxury-card, .testimonial-card, .golden-underline');
      
      elements.forEach(element => {
        const elementPosition = element.getBoundingClientRect().top;
        const screenPosition = window.innerHeight / 1.3;
        
        if(elementPosition < screenPosition) {
          element.classList.add('animate-fade-in');
        }
      });
    };
    
    window.addEventListener('scroll', animateOnScroll);
    window.addEventListener('load', animateOnScroll);
  </script>

</body>
</html>
