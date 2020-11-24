# Hairitage
## A website to support the Hairitage mobile application

The hypothetical Hairitage mobile application allows users to store and browse information relating to their history of hairstyles, hence the pun on the word "heritage".
The Hairitage website serves chiefly as an advertisement for the mobile app, offering potential users the chance to sign-up to beta test the application in its current form.

### Definitions ###
In what follows I will use the terms:
- 'barber' to refer to the collection of terms 'barber/stylist/hairdresser/etc.' 
- 'barbershop' to refer to the collection of terms 'barbershop/salon/hairdresser/etc.' 
- 'cut' to refer to the collection of terms 'cut/styling/colouring/etc.'
- 'user' to refer to users of the applications that are not themselves barbers.

### Application Features ###

The current key features of the application are:
* Allows users to save before and after photos taken at the time of each cut
* Allows users to store the style requested, barbershop attended and the barber that performed the cut
* Allows users to rate their barber, add personal notes and additional photos for future reference
* Allows barbers to leave notes about users' hair that may be useful in the future for both the user and other barbers, e.g. presence of a hidden double crown
* Allows users and barbers to view hairstyle trends by location based on anonymous user data

## UX ##
User stories:
- As a user type, I have no specific knowledge of the app but have heard it mentioned, e.g. through word of mouth
- As a user type, I have some knowledge of the application and would like to understand it better
- As a user type, I am aware of the product and most of its features and would like to sign up

Site owner story:
- Wants to present the basics of what the application can do in a manner that will entice potential users to sign up for the beta verison of the app.

### Five Planes ###
* Strategy: Given the above user and site-owner stories, the strategy is to convey basic information regarding the app in a way that is easy to understand. The website will provide the opportunity for users to sign up to the app and showcase some testimonials to show how other users have enjoyed using it.

* Scope: The scope will be quite limited as the hypothetical app is still in the testing phase at the moment. A sign-up form, information about the app's features and images of models sporting fashionable haircuts will be used to bolster the idea that the app could be useful.

* Structure/Skeleton: The below images show wireframes for the four sections I had originally planned on including (the About section later subsumed the Home page).

    #### Wireframes ####

    - [Desktop Home](https://github.com/spf34/milestone-project-1/tree/master/assets/images/wireframes/desktop-home.png)
    - [Desktop About](https://github.com/spf34/milestone-project-1/tree/master/assets/images/wireframes/desktop-about.png)
    - [Desktop Testimonials](https://github.com/spf34/milestone-project-1/tree/master/assets/images/wireframes/desktop-testimonials.png)
    - [Desktop Sign-Up](https://github.com/spf34/milestone-project-1/tree/master/assets/images/wireframes/desktop-sign-up.png)

    - [Mobile Home](https://github.com/spf34/milestone-project-1/tree/master/assets/images/wireframes/desktop-home.png)
    - [Mobile About](https://github.com/spf34/milestone-project-1/tree/master/assets/images/wireframes/desktop-about.png)
    - [Mobile Testimonials](https://github.com/spf34/milestone-project-1/tree/master/assets/images/wireframes/desktop-testimonials.png)
    - [Mobile Sign-Up](https://github.com/spf34/milestone-project-1/tree/master/assets/images/wireframes/desktop-sign-up.png)

* Surface: I will chiefly use muted colours (black, grey, white) along with a seagreen to enhance the minimal and 'fresh' feel of the website. Images will be mainly black & white with some of bright colour for contrast.

## Features ##

On each page:
- Easy to use navigation bar with links to all pages and a brandname link to the initial page position
- The navbar will collapse into the burger icon on smaller devices to save screen space
- The navbar is fixed on the About page but not on the others. I found this to be useful as this page is the only one long enough for substantial scrolling. For consistency, it may have been better to have a universal behaviour.
- Footer with social media links (Instagram & YouTube) and a further link to the initial page position
- Underlining of the active page/section was removed as this could be slightly confusing with the merger of Home and About into one page but two sections

[Home](https://github.com/spf34/milestone-project-1/tree/master/assets/images/app/home-live.png)

On the Home/About page (as noted above, these two were combined)
- Hero image to catch the user's eye and immediately set the context of the app - men's haircuts
- An About section featuring Bootstrap's Card component to easily display 4 facets of the app, along with images of well styled gents. The Card component will be responsive in the sense that the 4 cards will move to 2 rows of 2 when the screen width is smaller than Bootstrap's xl size.
- A reference to Einstein's quote about god not playing dice, along with an image of his own "Hairitage", i.e. the evolution of his famous hair over the years. The idea being that using Hairitage ensures the user will no longer be "playing dice" whenever they visit a new barber

[About](https://github.com/spf34/milestone-project-1/tree/master/assets/images/app/about-live.png)

On the Testimonials page
- Bootstrap's Carousel component featuring 4 images, together with quotes, from happy users of the app
- The images and quotes will be used to highlight common problems that the app can address. For example, a man with an esoteric looking mohican states that his hair can only be styled/cut right by looking at previous pictures of it. Having used the Before/After feature of the app to record previous cuts, this is no problem for our gent.

[Testimonials](https://github.com/spf34/milestone-project-1/tree/master/assets/images/app/testimonials-live.png)

On the Sign Up page
- A very simple input form requiring first name, last name and email address
- A button accompanies the form, declaring that the user can "Request Download Link"
- A background image further enforces the idea of the application and its users as being fashionable gents

[Sign up](https://github.com/spf34/milestone-project-1/tree/master/assets/images/app/sign-up-live.png)

## Technologies, Frameworks & Tools Used ##
- HTML/HTML5
- CSS/CSS3
- Bootstrap 4: Framework with pre-built HTML/CSS features
- Gitpod: online IDE
- Github: version control framework hosting code repository
- Font Awesome: source of icons
- Google Fonts: source of 'Roboto' and 'Playfair Display' fonts
- tinypng: reduce image file size

## Testing ##
- [HTML code validator](https://validator.w3.org/) - No errors or warnings (after fixing 1 inital bug identified this way)
- [CSS code validator](https://jigsaw.w3.org/css-validator/) - No errors or warnings
- Checking that all links are live and lead to the expected destination. Checking that this is true for all pages.
- Viewing all pages on all of the available devices in Chrome developer tools. Several issues discovered this way and fixed satisfactorily. There may still be screen sizes for which the behaviour is not perfect.
- Checking for and removing any unused css classes
- Checking for and removing any unused features within css classes
- Checking all images have alternate text (background-images were excluded from the check as they are purely aestetic)
- Test using Chrome and Safari
- Check that all Bootstrap columns are children of Bootstrap rows

## Bugs ##
- The right navigation pane for the carousel on the Testimonials page was blocking the navigation links in the upper right toolbar. To fix the issue I used absolute positioning to move the navigation panes down.

- Several bugs related to media responsiveness. In particular, the images in the carousel were either highly blurred or did not fill the screen, depending on which device was being used. 
To tackle this issue I took both portrait and landscape sub-images from each image and then utilised a media query to display the most relevant image depending on the device in question. 
This meant that the screen was filled without undue distortion of the image. However, since the base images were not all of the same size/aspect ratio, I was unable to 'match them' perfectly in the sense that the heights of the quote containers are not the same across images.

- A similar fix based on a media query was used to increase the size of the Cards on the About page on tablet-sized devices. At this size, only two columns were being displayed, however, the space was not being well utilised before this query was added.

- Found typo with initial HTML validator check

### Unresolved/Disappeared ###
- I had an error related to using a file originally named "about.html". Upon changing the name the issue seemed to disappear (and reappear upon changing it back)

- The Chrome developer tools would sometimes show misalignment of content that was actually fine (as checked versus e.g. Responsive Viewer). Restarting Chrome & Gitpod generally fixed this issue although it was somewhat sporadic.


## Deployment ##
This section closely follows the example given here: [README example](https://github.com/AJGreaves/portrait-artist/blob/master/README.md)

The project was developed using the Gitpod IDE and commited to github with git.

The project was depolyed from its [GitHub repository](https://github.com/spf34/milestone-project-1) to GitHub pages using the usual steps:
1. Navigate to the repository on GitHub
2. Click 'Settings' and scroll down to the 'GitHub Pages' subsection
3. Under Source click the drop-down menu labelled None and select Master Branch
4. On selecting Master Branch the page is refreshed and the website will now be deployed
5. Here is a link to the deployed page: [GitHub Pages Deployment](https://spf34.github.io/milestone-project-1/)

## Credits ##

### Code ###
The Card section of the About page is very closely modelled on examples provided in the Card section of the components page on the bootstrap website:
[Bootstrap 4 Card Component](https://getbootstrap.com/docs/4.5/components/card/)

The Carousel section of the Testimonials page is very closely modelled on examples provided in the Carousel section of the components page on the bootstrap website:
[Bootstrap 4 Carousel Component](https://getbootstrap.com/docs/4.5/components/carousel/)

The form section of the Sign Up page makes heavy use of the material covered in the 'Adding the contact form' subunit of Code Institute's User Centred Frontend Design module

I found the idea of using two classes of images with different aspect ratios depending on the user's device in this Stack Overflow response:
[Stack Overflow Media Query Question](https://stackoverflow.com/questions/23459754/trying-to-show-two-different-images-depending-on-two-media-queries)

### Media ###
Images were taken from Upsplash:
https://unsplash.com/

### Acknowledgement ###
- My tutor, Nishant Kumar, for ideas and debugging help
- The tutor support team at CodeInstitute 