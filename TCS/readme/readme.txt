LICENSE
The template is created by Inovatik and is offered for free use under the open source MIT license for any type and any number of projects.


FILE STRUCTURE
- index.html holds the entire content
- css/styles.css custom css styling
- js/scripts.js custom js code
- images folder contains all the images
- The rest are files specific to different frameworks and dependencies


FRAMEWORKS & DEPENDENCIES
- Bootstrap https://getbootstrap.com/
- Isotope Filterable Grid https://isotope.metafizzy.co/
- Purecounter https://www.cssscript.com/scroll-triggered-counter/
- Swiper https://swiperjs.com/
- Font Awesome for icons https://fontawesome.com/


IMAGES
All images are included in the download package and can be reused in your projects. The ones mentioned below come for outside resources. The ones not mentioned come from inside resources like created by Inovatik or purchased special license from authors. Either way you can use them for free in your project if you want.
- Header self hosted video https://www.videvo.net/video/coloured-smoke-on-black-15/4685/
- Details https://www.pexels.com/photo/people-inside-building-3184455/
- Services 1 https://www.pexels.com/photo/photo-of-man-near-computer-3184653/
- Services 2 https://www.pexels.com/photo/people-working-in-front-of-the-computer-3184357/
- Services 3 https://www.pexels.com/photo/man-and-woman-holding-green-bubble-text-board-3184403/
- Projects https://www.pexels.com/photo/person-in-black-pants-and-black-and-white-nike-sneakers-sitting-in-front-of-macbook-pro-4763075/
- Projects https://www.pexels.com/photo/black-headphones-black-and-silver-laptop-computer-black-headphones-black-headphones-black-headphones-black-headphones-black-4763077/
- Contact https://www.pexels.com/photo/shallow-focus-photography-of-gray-asphalt-floor-34090/
- Testimonials: https://www.pexels.com/photo/photo-of-people-standing-near-blackboard-3184393/
- Article details image large: https://www.pexels.com/photo/photo-of-imac-near-macbook-1029757/ 
- Article details image small: https://www.pexels.com/photo/apple-office-internet-ipad-38544/


CREDITS
- Video by Videvo: https://www.videvo.net/
- Images by Pexels: https://www.pexels.com/


-----------------------------------------------------


Change Testimonials Slider Properties
- Open for editing js/scripts.js
- Find the section /* Card Slider - Swiper */
- And then fiddle with the settings using the documentation here: https://swiperjs.com/swiper-api


-----------------------------------------------------


Update statistics number settings
- To change the statistics numbers find the /* Counter */ section and update the data-purecounter-end="" attribute
- You can also set the speed of each counter with data-purecounter-duration="3"
- The count speed can be adjusted to have all counters finish almost at the same time
- If you give bigger numbers less time to be counted to then they will finish close the the smaller ones


-----------------------------------------------------


Change the header video background
- To change the header video background you need to open index.html
- Find the Header section and then find the following lines of code
<!-- Video Background -->
<video autoplay loop muted id="video-background" poster="images/header-background.jpg" playsinline>
    <source src="images/header-background-video.mp4" type="video/mp4" />
</video>
<!-- end of video background -->

- Place your new video in the Images folder
- It's recommended to have a 1920 x 1080 resolution video in mp4 format
- And update the path src="images/header-background-video.mp4"
- You can also update the Poster image which will appear until the video loads
- It's best to take a screenshot of one of the first frames from the video
- Then place it in the Images folder and update the path poster="images/header-background.jpg" if necessary
- Save index.html and refresh the browser window to see the changes


-----------------------------------------------------


Updating the projects section
The Projects section uses Isotope plugin which can be configured as described here https://isotope.metafizzy.co/

Adding A New Project
To add a new project in the projects section, you need to:
- Open for editing index.html and find the Projects section
- Here focus on the code area just below
<div class="grid">

- You can copy the following piece of code:
<div class="element-item finance">
    <a href="article.html">
        <img class="img-fluid" src="images/project-1.jpg" alt="alternative">
        <p><strong>Online banking</strong> - delivered to and to major company in pharmace ski jump from</p>
    </a>
</div>

- And paste it wherever you want your project to be in the Show All order
- Now replace the name and the image as per your requirements
- Also add it to a designated category. Now it's set for "finance" as you can see from the code but you can change it to any category you define
- You can also designate it to multiple categories, just add the category as a class name like "business finance"

Adding A New Category
To add a new project category in the projects section, you need to:
- Open for editing index.html and find the Projects section
- Here in the Filter section duplicate a line like the one below:
<button class="button" data-filter=".finance">FINANCE</button>

- And replace the word "finance" in both locations with your category name
- Then also add it to the project line below
<div class="element-item finance">

- By replacing "finance" with your category name