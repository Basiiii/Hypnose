# Hypnose

Hypnose is a nightclub that plays hypnotic trance music. I created their branding (logo, font choice, color palette, etc.) along with the Home Page for their website. This repository will showcase the code for the website.

## Languages & technologies used

HTML, CSS, JavaScript and GSAP/ Three js.

## Code Snipet

Script for animations.

```javascript
var hoverAnimation = new hoverEffect({
        parent: document.querySelector('.image'),
        intensity: 0.3,
        image1: '/img/hypnose1.jpg',
        image2: '/img/hypnose2.jpg',
        displacementImage: '/img/diss.png',
        imagesRatio: 4 / 3

    });


    // animate
    gsap.from('.heading__item', {opacity: 0, duration: 1, delay : 1, stagger: 0.1, y: -30});
    gsap.from('.title', {opacity: 0, duration: 1.2, delay : 1.5, y: -30});
    gsap.from('.image__container', {opacity: 0, duration: 1.2, delay : 1.7, y: -50});
    gsap.from('.more-details', {opacity: 0, duration: 1.2, delay : 1.7, y: -50});

    // click on the hamburger menu
    var hamburger = document.getElementById('menu-toggle');
    var logo = document.querySelector('.brand');

    hamburger.addEventListener('click', function(){
        var navMenu = document.getElementById('nav-menu');
        navMenu.style.display = 'flex';
        logo.style.transform = null;
        gsap.from('.nav__item', { opacity: 0, duration: 1, stagger:0.2, y: -50 })

    });

    var close = document.getElementById('nav-close');
    close.addEventListener('click', function(){

        var navMenu = document.getElementById('nav-menu');
        navMenu.style.display = 'none';
    })
```

## Additional Information
Primary font used: ```Proxima Nova Regular.```
Credit for green photo in Home page to [NITISH GOSWAMI.](https://unsplash.com/@nitishgoswami)
  
