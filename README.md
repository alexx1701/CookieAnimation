<img width="576" alt="Screen Shot 2022-02-17 at 2 05 36 PM" src="https://user-images.githubusercontent.com/92756383/154562415-ab02ae4b-b967-4cfe-b093-2864824518b0.png">

# CookieAnimation

You can find the hosted animation [here!](https://cookieanim.netlify.app/)

A quick overview of the javascript code:
```
tl = gsap.timeline({defaults: {duration: 0.75, ease: "power1.out"}})

tl.fromTo('.cookie-container', {scale:0}, {scale:1, ease: "elastic.out(1, 0.75)"})
tl.fromTo('.cookie', {opacity:0, x:-50, rotation: '-45deg'}, {opacity:1, x:0, rotation: '0deg'})
tl.fromTo('.text', {x:30, opacity:0}, {x:0, opacity:1}, '<')

tl.fromTo('.cookie', {y:0, rotation: '0deg'}, {y: -15, yoyo: true, repeat: -1, rotation: '-20deg'})
tl.fromTo('#crumbs', {y:0}, {y: -5, yoyo: true, repeat: -1}, '<')


//fade out button
const button = document.querySelector('button');
button.addEventListener('click', () => {
    gsap.to('.cookie-container', {opacity: 0, y:100, duration:0.75, ease:'power1.out'})
})

```

