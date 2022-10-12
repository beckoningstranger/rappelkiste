# Contents

* [**Validator Testing**](#validator-testing)
  * [HTML and CSS](#html-and-css)
  * [Lighthouse Test](#lighthouse-test)
  * [WAVE Web Accessibility Evaluation Tool](#wave-web-accessibility-evaluation-tool)
* [Responsiveness Test](#responsiveness-test)
  * [Chrome Dev Tools](#chrome-dev-tools)
  * [Firefox Dev Tools](#firefox-dev-tools)
* [Testing User Stories]()
* [Solved Bugs](#solved-bugs)
* [Known Bugs](#known-bugs)

[Back to README.md](README.md)

# Validator Testing

## HTML and CSS

To test compliance with HTML standards, the [W3C Markup Validation Service](https://validator.w3.org/) was used. Here are the results for all files:

![index.html](/assets/documentation-images/code-validation-index.png)
![team.html](/assets/documentation-images/code-validation-team.png)
![stories.html](/assets/documentation-images/code-validation-stories.png)
![contact.html](/assets/documentation-images/code-validation-contact.png)
![thankyou.html](/assets/documentation-images/code-validation-thankyou.png)
![style.css](/assets/documentation-images/jigsaw-validation.png)

[Back to top](<#contents>)

## Lighthouse Test

Lighthouse Test for desktops - Home

![Lighthouse Test for desktops - Home](/assets/documentation-images/lighthouse-desktop-home.png)

Lighthouse Test for mobile devices - Home

![Lighthouse Test for mobile devices - Home](/assets/documentation-images/lighthouse-mobile-home.png)

Lighthouse Test for desktops - Team

![Lighthouse Test for desktops - Team](/assets/documentation-images/lighthouse-desktop-team.png)

Lighthouse Test for mobile devices - Team

![Lighthouse Test for mobile devices - Team](/assets/documentation-images/lighthouse-mobile-team.png)

Lighthouse Test for desktops - Stories

![Lighthouse Test for desktops - Stories](/assets/documentation-images/lighthouse-desktop-stories.png)

Lighthouse Test for mobile devices - Stories

![Lighthouse Test for mobile devices - Stories](/assets/documentation-images/lighthouse-mobile-stories.png)

Lighthouse Test for desktops - Get in Touch

![Lighthouse Test for desktops - Get in Touch](/assets/documentation-images/lighthouse-desktop-contact.png)

Lighthouse Test for mobile devices - Get in Touch

![Lighthouse Test for mobile devices - Get in Touch](/assets/documentation-images/lighthouse-mobile-contact.png)

Lighthouse Test for desktops - Thank You

![Lighthouse Test for desktops - Thank You](/assets/documentation-images/lighthouse-desktop-thankyou.png)

Lighthouse Test for mobile devices - Thank You

![Lighthouse Test for mobile devices - Thank You](/assets/documentation-images/lighthouse-mobile-thankyou.png)

[Back to top](<#contents>)

## WAVE Web Accessibility Evaluation Tool

[Back to top](<#contents>)

# Responsiveness Test

Extensive test were conducted to ensure that the website looks great both on devices as small as the Galaxy Fold, which has only 280px of horizontal space when in portrait mode up to viewports with 1920px in viewport width such as desktop computers. Mobile devices were tested with both Google Chrome and Firefox Dev Tools and both in portrait as well as landscape mode.

All tests were carried out in the developer tools of the browsers.

## Chrome Dev Tools

|| Moto G4 | iPhone SE | iPhone XR | iPhone 12 Pro | Pixel 5 | Samsung Galaxy S8+ | Samsung Galaxy S20 Ultra | iPad Air | iPad Mini | iPad Pro (12.9 inch) | Surface Pro 7 | Surface Duo | Galaxy Fold | Nest Hub | Nest Hub Max | Pixel 2 XL | Laptops (1366x768) | Desktops (1920x1080px) |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Render | pass | pass | pass | pass | pass | pass | pass | pass | pass | pass | pass | pass | pass | pass | pass | pass | pass | pass |
| Images | pass | pass | pass | pass | pass | pass | pass | pass | pass | pass | pass | pass | pass | pass | pass | pass | pass | pass |
| Links | pass | pass | pass | pass | pass | pass | pass | pass | pass | pass | pass | pass | pass | pass | pass | pass | pass | pass |

## Firefox Dev Tools

|| iPad Air | iPad Mini | iPad Pro (12.9 inch) | iPhone 12/13 + Pro iOS 14.6 | iPhone 5/SE iOS 10.3.1 | iPhone 2nd gen iOS 14.6 | iPhone XR/11 iOS 12 | Microsoft Lumia 550 | Microsoft Lumia 950 | Laptops (1366x768) | Desktops (1920x1080px)
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| User Agent | Safari | Safari | Safari | Safari | Safari | Safari | Safari | Edge | Edge | Firefox | Firefox |
| Render | pass | pass | pass | pass | pass | pass | pass | pass | pass | pass | pass |
| Images | pass | pass | pass | pass | pass | pass | pass | pass | pass | pass | pass |
| Links | pass | pass | pass | pass | pass | pass | pass | pass | pass | pass | pass |

[Back to top](<#contents>)

# Browser compatibility

The website was tested in Google Chrome, Mozilla Firefox and Microsoft Edge. Everything worked as intended in realistic use cases. The layout is breakable, e.g. when you narrow the viewport height below 400px on desktop computers that maintain a wide viewport, but I do not expect users to run into scenarios like this.

[Back to top](<#contents>)

# Testing User Stories

**As somebody who wants to get in touch with the day care center I want an easy way of calling, writing an email or otherwise contacting somebody, be it to plan a personal visit as an interested parent, to phone in to coordinate with the teachers for parents whose child already attends, or as somebody looking for an internship, just as a few examples.**

  * Users will find 'Get in Touch' prominently in the top menu. On the Get in Touch page, they are made aware of the footer if they have not noticed it already. Clicking either of the links allows them to get in touch, in addition to the form. Of course, they may also find the footer while exploring the other pages.

**As a parent who has made an appointment for a personal visit, I want an easy way to navigate to the day care center.**

  * 




[Back to top](<#contents>)

# Solved Bugs

1. One problem that came up during Lighthouse testing was 'Tap target are not sized appropriately'. This was because the links in the top menu were two close together on small displays like on the Motorola G4. I first applied 'display: flex' and 'justify-content: space-between' to the menu to arrange for more horizontal space, then increased the overall size of the header for more vertical space. This solved the problem and got me to a perfect score in the SEO category if the Lighthouse test.

2. A problem that was highlighted during my mid-project meeting with my mentor was that the background pictures on the Home page occupied so much vertical space that users had to scroll quite a bit before reaching the next section with the next background picture. This was not an easy fix because I had set the vertical space in px instead of a relative unit of measurement. In the end I had to change to whole layout in so far as I set the height of each section in vh. Now all middle sections of the Home page occupy 100vh whereas the top and bottom sections occupy 90vh, leaving just enough space for header and footer to be shown at the same time. This solved the problem nicely, but had the side effect that the background pictures were often cut off. I had to address this, too.

3. Due to the change described in 2., combined with the problem that the background pictures on the Home page were often showing only small parts of the picture on small viewports, I had to create more background picture files that catered better to the needs of the smaller viewports. Anything else would have rendered the pictures useless as they would not have had the desired effect. It was a challenge to find a working solution for this, because if you want to support both portrait and landscape modes one has to keep in mind that one has a lot of vertical space and very limited horizontal space and the vice versa. Rotating the picture with the device would have been ideal, but of course this was not possible. So I decided to upload squared pictures, making sure that the most important content was dead in the center. To support small viewports as best as possible, I uploaded 1024x1024px (the iPad Mini has a 1024x768 viewport), for tablets I uploaded images in the 1368x1368px format (the Surface Pro 7 and iPad Pro have resolutions of 912x1368 and 1024x1366 respectively). For most devices, this lead to decent results, but the pictures are best viewed on large viewports, of course. 

4. Another bug was that the top menu didn't show the border-top defined as .active in the CSS, because there just wasn't enough vertical space and the elements underneath simply overlapped this border. Again, this was fixed by giving the top menu more vertical space.

5. The original photo at the very top of the Home page (building with blue sky) had cables coming from the roof and going to the top left of the picture. This did not look right, at the beginning of the process, the top menu simply overlapped the first picture. So my first attempt at solving this was giving the header its own area. This resulted in another problem, namely that I had to photoshop the sky area of the picture so that there would be no visible transition to the header area. I did this with GIMP. After this, the cables ended just under the header area, but also did not look right. In the end I used GIMP again to remove the cables entirely. They are still visible in the wireframes I created.

6. When trying to position the text boxes on the Home page, I first used absolute position. After spending hours on fine tuning these positions and testing on many devices of many different sizes I realized that this was too much work to main, also my numbers never worked for all viewport sizes. So I moved away from absolute positioning and turned to flexbox. This allowed me to center the boxes in the middle of the images at positions that relative to the viewport height. Together with the changes described in 2. this lead to much better results and is also a lot easier to maintain, resulting in less code.

7. I had some trouble figuring out how to center the text in the text boxes on the Home page. After trying to find magic numbers for padding that would just work for all viewport sizes, I finally realized that this too could be solved with flexbox, align-items and justify-content. This also solved the problem of finding an appropriate size for the text boxes. Before centering the text in them, they would often be either too small or too big. After centering the text, bigger boxes are preferred because they still look good, even if the content does not fill them completely.

8. A lot of time was spent on making the size really responsive. After realizing that relative units of measurement were key for this, I started defining font-sizes in vw. This yielded good results for small viewports, but on larger viewports fonts became gigantic. With media queries that change the font size to rem at the 768px breakpoint, I could solve this problem.

9. After a lot of work on making the site responsive and testing I realized I also had to deal with the possibility that users would want to view the site in landscape mode, even on small phones like the Moto G4 or iPhone SE. After doing my research I found the property (orientation: landcape) that can be used in media queries. After putting in more hours in fine-tuning the CSS, I now get much better results and the site remains readable, even on small devices in landscape mode. The pictures don't realize their full potential here, I probably would have needed to upload even more pictures to cater to this specific format.

10. When doing the Team page layout for viewports >540px width and <1200px width I wanted some of the team member photos to appear on the left, some on the right side. After fiddling around with the float property I finally turned to the Code Institute tutors who made me aware of flexbox. Having done the research I found that I could reverse the order of elements with the order property, which is what I used to solve this problem. I now know that the flex-direction property could also have helped here and this is probably what I would do next time.

11. The form on the Get in Touch page would often overlap with the footer, especially on small viewports in landscape mode. This was fixed by giving the main section more height. Ideally, the main section would always fill up the entire alloted space between header and footer, but I don't think this can be done in an efficient way. One would probably have to optimize for every device specifically.

12. Lighthouse Testing revealed a problem on the Stories page, where I had used \<h3\> for an article heading where I should have used \<h1\> because it was the topmost heading. I had done this in order not to confuse the styling with the heading on the Home page. This was solved by replacing the \<h3\> with \<h1\> and precise CSS styling.

[Back to top](<#contents>)

# Known Bugs

1. As I have mentioned before, when users navigate to the Teams page on viewports >1200px width, they will see the layout where all team member photos are displayed next to each other with an empty under the photos. Only when they hover the mouse over a photo or tap it (e.g. on tablets) will they see a description for this team member. This is not ideal, but I really believe in this layout because it's nicely interactive, shows all team members side by side and does not require any scrolling at all, making it nicely compact. I contacted the Code Institute tutors for help, but they could not figure out a way of showing the page with a team member pre-selected, at least not with pure HTML/CSS. This is something that I will solve once I learn about JavaScript, as I have been told that this is a common way of doing a layout like this.

2. The form on the Contact page does not *actually* work, it does not send the gathered data anywhere. This is an obvious limitation in this project but can be rectified once I learn about back end technology.

[Back to top](<#contents>)

[Back to README.md](README.md)