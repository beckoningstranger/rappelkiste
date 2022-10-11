# Rappelkiste e.V.

Rappelkiste e.V. is a site that is aimed at parents who are looking for a day care center for their unborn or newly born child. The German word Rappelkiste could be translated loosely to 'rattlebox', it refers to the house (the box) from which you can hear all kinds of noises (the rattling). "e.V." means "registered association", which is legally relevant and also hints at the fact that this day care center is special in that it was founded and is still run by parents, not the state, a church or any other institution.

Visitors of the site are supposed to get a first impression of what makes this day care center special, i.e. is the picturesque building, the interior's cozy atmosphere, the friendly teachers, the fact that it has an above average sized team and that the teachers have lots of interesting activities and projects in store for the children which parents can read about in the Stories section. Users can then use the Get in Touch page or click the telephone/email links to contact the day care center.

Take a look at the deployed page: <a href="https://beckoningstranger.github.io/rappelkiste/index.html" target="_blank" rel="noopener">Rappelkiste</a>.

![Responsive Design - Rappelkiste e.V.](/assets/readme-images/amiresponsive.png)

# CONTENTS

# User Experience (UX)

## User Stories

### Client Goals

* As the manager of the Rappelkiste I want a way to attract new parents that may visit the site on a wide range of differently sized devices.

* As the manager of the Rappelkiste I want the site to act as a calling card that gives my audience a good impression of the day care center and its team, to build confidence and trust with them.

* As a teacher I want to showcase projects that the teaching team has done with the children to further build confidence/trust in the team's work.

* As the manager I want to give people an easy way to get in touch, be it via telephone, email or a contact form.

### First Time Visitor Goals

* As a parent who is looking for a day care center for my child, I want to build trust with a day care center where my child will potentially spend most of their day.

* As a parent who is looking for a day care center for my child, I want to learn what sets the Rappelkiste apart.

* As a parent who is looking for a day care center for my child, I want to learn what the facilities look like and get a vibe of the atmosphere.

* As a parent who is looking for a day care center for my child, I want to learn about who will look after my child and what background they have.

* As a parent who is looking for a day care center for my child I want to learn about special activities the teachers planned for the children.

* As a parent who is looking for a day care center for my child, I want a quick way of figuring out how far the day care center is from my home.

### Returning Visitor Goals

* As a parent whose kids already attend the day care center, I want to read and learn more about activities that my child talked about after coming home, but couldn't explain fully.

* As somebody who wants to get in touch with the day care center, be it for  I want an easy way of calling, writing an email or otherwise contacting somebody, be it to plan a personal visit as an interested parent, to phone in to coordinate with the teachers for parents whose child already attends, or as somebody looking for an internship, just as a few examples.

* As a parent who has made an appointment for a personal visit, I want an easy way tp navigate to the day care center.

## Design

### Site Structure

The website consists of four main pages and a thank you page. The [Home page](index.html) is the landing page, while the [Team page](team.html), the [Stories](stories.html) and the [Get in Touch](contact.html) page are accessible via the top menu. Once the user successfully submits a message on the [Get in Touch page](contact.html), they are taken to a simple [Thank You page](thankyou.html), from where they can navigate anywhere they want via the top menu.

### Color Scheme

![Color Scheme](/assets/readme-images/color-scheme.jpg)

The color True Blue (#3567BB) was taken from the hero image that you see when you first visit the site, the darker blues were picked to create nice looking gradients that ensured contrast to keep the overlaid white text easy to read. The True Blue that's also present on every site in the header will hopefully set the mood for the entire page, as it is associated with good weather, sunshine and all the feelings that are associated with that.
On the Team page, where the larger font size makes the text easier to read, I have picked a True Blue (#3567BB) to Dark Cornflower Blue (#19366D) gradient, on the Stories page, where the font size is significantly smaller and there's also just more text I have picked a Dark Cornflower Blue (#19366D) to Oxford Blue (#0A214B) gradient.

### Typography

Google Fonts was used for the following fonts:

- Lusitana is used for headings and body text of the site. It is a serif font that is still very easy to read.

- Meow Script is a monoline font that adds character to the site's logo.

### Wireframes

At the outset of this project, the design of the website was desktop first, which is why the emphasis was on creating wireframes for this size format. This later changed, but all designs found their way into the final website except for the Contat page which was redesigned at a late stage of development.

![Home Wireframe](/assets/readme-images/home-wireframe.jpg)
![Team Wireframe](/assets/readme-images/team-wireframe.jpg)
![Stories Wireframe](/assets/readme-images/stories-wireframe.jpg)
![Get in Touch Wireframe](/assets/readme-images/get-in-touch-wireframe.jpg)

As this was my first foray into designing, I had to adapt when I found that the initial design would not work or could be improved. The most significant of these changes was the contact page where I found that the two-column design with the clearly defined border in the middle would not be practical, even on larger screens as the picture would often be cut off or the two columns would not be of equal length, breaking the design. I eventually opted for a screen filling background picture with an overlaid box for the text and form.

The initial Team page design was realized for mid-sized screens, i.e. larger phones in landscape mode and tablets with viewport widths greater than 540px but smaller than 1200px. For smaller viewports I decided on a one-column design and for viewports over 1200px in width I found a completely new design that presents the team as a whole in one line with a text box under the pictures with changing text, depending on which picture the user taps/hovers. 

## Features

### Existing Features

#### __Navigation Menu__

    - The navigation menu lets users access the four main pages of the website. It is responsive and displayed in two rows for viewport widths lower than 768px. In wider viewports, all of the content is fit into one row. 
    - Users on devices with attached pointing devices will see a hovering effect that underlines the menu items they hover over.
    - The page the users are on is displayed as underlined.
    - The logo is also clickable, but will show the Home page if clicked.

  ![Layout for viewport widths below 786px](assets/readme-images/topmenu-one-row.png)
  ![Layout for viewport widths 786px and up](assets/readme-images/topmenu-two-rows.png)

#### __Home page: Picture Gallery with text boxes and full page scrolling__

  - On the Home page, the background pictures cover 80% or 90% of the viewport height per section, depending of device orientation, resulting in a view where the navigation menu covers the top 10-20% and the background picture the rest of the screen. This puts the pictures front and center, with no distrations. Naturally, the pictures look better the larger the viewport is, but I have created 3 picture sizes that are applied depending on the viewport width:

    - For phones, a 1024x1024px sized picture, so that users can also use their phone in landscape mode without the picture being cut off.
    - For tables and small laptops, a 1368x1368px sized picture. This specific size was chosen because of the Surface Pro 7 that has this exact width in landscape mode. The iPad Pro has a width of 1366px, which is very similar.
    - For wider viewports, a picture with a width of 2160px is used.

  All pictures are centered on both axes, except for the hero image where I wanted to avoid the gable of the house being cut off.

  - For each pictures, there is an overlaid text box, that provides additional information for users. This way, users get a good idea of the facilities and values that underpin the day to day life of the day care center. The text box is most located at the bottom center, expect when that would block an element of the photo that I wanted to be in clear view. In these cases, the text box was moved to the top center. These text boxes are also fully responsive and adapt to the viewport width and whether the device is in portrait or landscape mode. A lot of testing went into this, more on this in the [Testing Section](TESTING.md).
  To ensure that the text is easily to read, the overlay text box is semi-transparent, giving enough contrast against the background picture.

  - A side bar with 5 dots, one for each section, gives the user an idea of the amount of sections he can see as well as a means to navigate to each section easily. Using this bar also has the advantage that each picture will be nicely aligned with the viewport edges. This sidebar is positioned at center left and will show a slight hover effect for users using pointing devices.

  ![Home page 1 of 5 sections](assets/readme-images/home-page-content.jpg)

#### __Footer__

  - The footer contains three links. One to easily place a call to the day care center, one to email them and one that will take you to Google Maps in case you want to see where the day care center is located or you want to navigate to it.

  ![Footer](assets/readme-images/footer.jpg)

#### __Team Page__

  - The Team page is fully responsive and will display in three different layouts, depending on viewport size. For viewports below 540px width, there's a one column view, for viewports below 1200px a two column view and for viewports of 1200px and above a third layout, where all of the team members are display side by side and users have to click them to read their descriptions. Even though I like this design, it's probably the poorest UX of all the ones present here, because users will find the page with an empty text box before they tap/hover a picture. I intend to change this once I learn about JavaScript, so that the user will find the page with a photo preselected and the text box at the bottom filled. Unfortunately there does not seem to be a way to do this with pure HTML/CSS, I did quite a bit of research and also eventually consulted the tutor team, with no results.
  - The Team page will give users an idea of who will look after their children and what background they have, the aim is to build trust.

  ![Team page - 1 column layout](/assets/readme-images/team-page-1-column.jpg)
  ![Team page - 2 column layout](/assets/readme-images/team-page-2-columns.jpg)
  ![Team page - wide viewports layout](/assets/readme-images/team-page-wide-viewports.jpg)

#### __Stories Page__

  - The Stories page is also fully responsive, with a one column layout for viewports widths below 1200px and a two column layout for viewports above 1200px width. Where photo and viewport width allow, photos will be displayed next to each other to fit more content on the screen. On this page, users can read more about the team's work, recent events and projects the children did and anything else the teachers might choose to blog about. All of this serves to build trust in the day care center and its team's work.
  
  ![Stories page - 1 column layout](/assets/readme-images/stories-page-one-column.jpg)
  ![Stories page - 2 column layout](/assets/readme-images/stories-page-two-columns.jpg)

#### __Get in Touch Page__

  - The Get in Touch page is displayed with a one column layout for view for viewports below 1200px of width and a background page with an overlaid box on the left hand side for wider viewports. Here, users have another easy way to get in touch with the day care center. Upon submitting the form, users are taken to a simple Thank You page.

  ![Get in Touch page - 1 column layout](/assets/readme-images/contact-page-one-column.jpg)
  ![Get in Touch page - Layout with background image and overlaid form box](/assets/readme-images/contact-page-overlay-box.jpg)

#### __Thank You Page__
  
  - From this simple page, user can navigate back to where they want, as the navigation menu at the top is shown as on all other sites. This just serves as feedback that their message was processed.

  ![Thank You page](assets/readme-images/thank-you-page.jpg)

### Future Implementations

* An admin section that allows teachers to publish more articles on the Stories page.
* A members section where teachers can post announcements for all current parents. Polls are another idea.
* An update to the Team page layout visible with viewports wider than 1200px so that when users come to it, a teacher is pre-selected.
* Swipe actions on mobile devices to let users navigate from page to page, giving it the feel of an app.

### Accessibility

## Technologies Used

### Languages Used

HTML 5 & CSS 3

### Frameworks, Libraries & Programs Used

![Figma](https://figma.com) - For creating designs and experimenting with page layouts

![Git](https://git-scm.com/) - For version control

![Github](https://github.com) - To save and store my project files

![Google Fonts](https://fonts.google.com/) - To find and import fonts

![Font Awesome](https://fontawesome.com/) - To build the full page scrolling navbar and additional iconography

![Google Dev Tools](https://developer.chrome.com/docs/devtools/) - To work out bugs, troubleshoot and test features and play around with property values

![Compressor.io](https://compressor.io) - To compress images

![GIMP](https://gimp.org) - To resize and convert images and to make the skies on the images I used one coherent color so that there is no visible transition to the header

![Favicon.io](https://favicon.io/) - To create a favicon

![Am I Responsive?](https://ui.dev/amiresponsive) - To showcase the website on all of the images used in this README file

![Web Disability Simulator](https://chrome.google.com/webstore/detail/web-disability-simulator/olioanlbgbpmdlgjnnampnnlohigkjla) - To ensure accessibility for all users

## Deployment & Local Development

## Testing

### Validator Testing

- HTML
  - No errors were returned when passing through the official [W3C validator](https://validator.w3.org/nu/?doc=https%3A%2F%2Fcode-institute-org.github.io%2Flove-running-2.0%2Findex.html)
- CSS
  - No errors were found when passing through the official [(Jigsaw) validator](https://jigsaw.w3.org/css-validator/validator?uri=https%3A%2F%2Fvalidator.w3.org%2Fnu%2F%3Fdoc%3Dhttps%253A%252F%252Fcode-institute-org.github.io%252Flove-running-2.0%252Findex.html&profile=css3svg&usermedium=all&warning=1&vextwarning=&lang=en#css)

- Lighthouse

- WAVE

### Unfixed Bugs

## Deployment

- The site was deployed to GitHub pages. The steps to deploy are as follows: 
  - In the GitHub repository, navigate to the Settings tab 
  - From the source section drop-down menu, select the Master Branch
  - Once the master branch has been selected, the page will be automatically refreshed with a detailed ribbon display to indicate the successful deployment. 

The live link can be found here - https://beckoningstranger.github.io/rappelkiste

## Credits

## Acknoledgements

### Content

- Bullet Point 1
- Bullet Point 2

### Media

- Bullet Point 1
- Bullet Point 2

