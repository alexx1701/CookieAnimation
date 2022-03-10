
# CookieAnimation


<img width="576" alt="Screen Shot 2022-02-17 at 2 05 36 PM" src="https://user-images.githubusercontent.com/92756383/154562415-ab02ae4b-b967-4cfe-b093-2864824518b0.png">
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->



<!-- ABOUT THE PROJECT -->
## About The Project


A cookie popup animation using GSAP! Nothing too complicated, but another way to add life and character to a webpage.

### Built With

* HTML
* CSS
* JavaScript
* GSAP


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

<!-- CONTACT -->
## Contact

Alexandra Christopher - [My Portfolio Site](https://alexmchris.com/) - alexandra.christopher@outlook.com

Live Link: [Click here for the live version!](https://cookieanim.netlify.app/)

<p align="right">(<a href="#top">back to top</a>)</p>




<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/github_username/repo_name.svg?style=for-the-badge
[contributors-url]: https://github.com/github_username/repo_name/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/github_username/repo_name.svg?style=for-the-badge
[forks-url]: https://github.com/github_username/repo_name/network/members
[stars-shield]: https://img.shields.io/github/stars/github_username/repo_name.svg?style=for-the-badge
[stars-url]: https://github.com/github_username/repo_name/stargazers
[issues-shield]: https://img.shields.io/github/issues/github_username/repo_name.svg?style=for-the-badge
[issues-url]: https://github.com/github_username/repo_name/issues
[license-shield]: https://img.shields.io/github/license/github_username/repo_name.svg?style=for-the-badge
[license-url]: https://github.com/github_username/repo_name/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/linkedin_username
[product-screenshot]: images/screenshot.png

