# Waste Matters
## Table of Contents
- [Project purpose](#project-purpose)
- [UX](#ux)
  * [User stories](#user-stories)
  * [Strategy](#strategy)
  * [Scope](#scope)
  * [Surface](#surface)
    + [Color Scheme](#color-scheme)
    + [Typography](#typography)
    + [Imagery](#imagery)
  * [Wireframes](#wireframes)
- [Features](#features)
- [Technologies Used](#technologies-used)
  * [Languages used](#languages-used)
  * [Frameworks, Libraries & Programs Used](#frameworks--libraries---programs-used)
- [Testing](#testing)
  * [Code Validation](#code-validation)
  * [Functionality test](#functionality-test)
  * [Problems during development](#problems-during-development)
  * [Browser Compatibility](#browser-compatibility)
  * [Responsiveness Testing](#responsiveness-testing)
  * [Unresolved Bugs](#unresolved-bugs)
  * [Google Lighthouse Scores](#google-lighthouse-scores)
- [Deployment to Github Pages](#deployment-to-github-pages)
- [Clone](#clone)
- [Credits](#credits)
  * [Media](#media)
  * [Acknowledgments](#acknowledgments)

<small><i><a href='http://ecotrust-canada.github.io/markdown-toc/'>Table of contents generated with markdown-toc</a></i></small>
## Project purpose
Waste matters Ltd. offers waste and recycling solutions to Irish businesses. The interactive demo aims to advertise and sell polystyrene compactors. The demo will guide the user through a mini-game in which they will drag and drop polystyrene blocks into a compactor machine before turning it on. While interacting with the demo, the user will receive key facts about polystyrene recycling and waste matters. On completion of the demo, the user will have the option to ‘learn more’ which will lead them to the current waste matters website.

## UX

### User stories
* As a user, I would like the user experience on the website to be
intuitive.

    * The interactive demo guides users using [clear instructions](https://github.com/Wbwren/waste-matters/blob/master/assets/img/user-instruction-arrow.png)

* As a user, I want to learn about polystyrene compactors and how
they work.

    * The demo demonstrates how the [polystyrene compactors work](https://github.com/Wbwren/waste-matters/blob/master/assets/img/compactor-compacting.png)

* As a user, I want to learn about polystyrene recycling in an engaging manor.

    * The interactive demo requires user engagement while displaying the information in a [clear manor](https://github.com/Wbwren/waste-matters/blob/master/assets/img/user-notification.png)

* As a user, I want my experience on the website to be enjoyable.

    * The interactive demo is built on a rigid body physics engine. [Interacting with the polystyrene blocks](https://github.com/Wbwren/waste-matters/blob/master/assets/img/interacting-with-blocks.png) can elicit a positive emotional response.

### Strategy
__Goal__: To inform users about polystyrene recycling in an engaging manor and sell polystyrene compactors through waste matters Ltd.

### Scope
* An interactive demo utilizing Matter.js, a 2D rigid body JavaScript physics engine.

### Surface

#### Color Scheme
* Font color: #f0f8ff
* background color: #14151F
* User instructions: #ff0000
#### Typography
Roboto Mono is the font used on the webpage with monospace as the fallback font in the case of the default font failing to load correctly.
The default font weight of 400 is used throughout the page.
#### Imagery
* The imagery is cartoon-like in style.
### Wireframes
* [Mobile View](https://github.com/Wbwren/waste-matters/blob/master/wireframes/mobile-wireframe.png)

* [Tablet View](https://github.com/Wbwren/waste-matters/blob/master/wireframes/tablet-wireframe.png)

* [Desktop View](https://github.com/Wbwren/waste-matters/blob/master/wireframes/desktop-wireframe.png)
## Features
This project is an interactive game built on the 2d physics engine matter.js. It allows users to place polystyrene objects into a compactor and turn it on. This game serves the purpose of engaging the user and allowing for an alternative way of imparting information. Facts about polystyrene recycling, polystyrene compactors and waste matters appear as the user interacts with the demo.
## Technologies Used
### Languages used
* HTML5
* CSS3
* JavaScript
### Frameworks, Libraries & Programs Used
* [Matter.js](https://brm.io/matter-js/)
* [Visual Studio Code](https://code.visualstudio.com/)
* [Google Fonts](https://fonts.google.com/)
* [Font Awesome](https://fontawesome.com/)
* [Git](https://git-scm.com/)
* [Github](https://github.com/)
* [Balsamiq Wireframes](https://balsamiq.com/wireframes/)
* [Microsoft PowerPoint](https://office.live.com/start/powerpoint.aspx)
* [Microsoft Word](https://office.live.com/start/word.aspx)
* [Google Chrome Developer Tools](https://developers.google.com/web/tools/chrome-devtools)
* [jQuery](https://jquery.com/)
## Testing

### Code Validation
* HTML was validated using W3C Markup Validation Service.

* CSS was validated using W3C CSS Validation Service - Jigsaw

* JavaScript was passed through the linter jshint with no warnings
### Functionality test
| Num | Test                                                                                                                      | Action                                             | Outcome Image                                                                                                                                                 | Result | Notes                                          |
|-----|---------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------|--------|------------------------------------------------|
| 1   | On page-load a user notification appears                                                                                  | Load page on devices with a variety of resolutions | [Image of user notification](https://github.com/Wbwren/waste-matters/blob/master/assets/img/user-notification.png)                                            | Pass   |                                                |
| 2   | The 'next' button makes a user instruction arrow appear                                                                   | Click next button                                  | [Image of user instruction arrow](https://github.com/Wbwren/waste-matters/blob/master/assets/img/user-instruction-arrow.png)                                       | Pass   |                                                |
| 3   | The 'P' button when clicked, moves the user instruction arrow, spawns a polystyrene block and presents a new user message | Click spawn button                                 | [Image of user instruction arrow, polystyrene block and new message](https://github.com/Wbwren/waste-matters/blob/master/assets/img/spawn-button-outcome.png) | Pass   |                                                |
| 4   | The 'P' button when clicked immediately after next button behaves as expected                                             | Click spawn button immediately after next button   | [Image of user instruction arrow frozen on spawn button](https://github.com/Wbwren/waste-matters/blob/master/assets/img/user-instruction-arrow-frozen.png)   | Fail   | User instruction arrow freezes on spawn button |
| 5   | The compactor switch ejects compacted polystyrene from the machine                                                        | Click compaction switch                            | [Image of compacted polystyrene ejected from the machine](https://github.com/Wbwren/waste-matters/blob/master/assets/img/compacted-polystyrene-ejected.png)   | Pass   |                                                |
| 6   | The compactor switch triggers the final user message                                                                      | Click compaction switch                            | [Image of final user message](https://github.com/Wbwren/waste-matters/blob/master/assets/img/final-user-message.png)                                          | Pass   |                                                |
| 7   | The 'Learn more' button when clicked opens in a separate tab and brings users to wastematters.ie                          | Click Learn more button                            | [Image of wastematters.ie opening in a new tab](https://github.com/Wbwren/waste-matters/blob/master/assets/img/wastematters.ie-opening-new-tab.png)           | Pass   |                                                |
<br>

### Problems during development
| Num 	| Problem                                                                                                        	| Fix                                                                                                                                                                                                                           	|
|-----	|----------------------------------------------------------------------------------------------------------------	|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| 1   	| Textures not appearing on matter.js shapes                                                                     	| Disable wireframes under render.options.wireframes                                                                                                                                                                            	|
| 2   	| Polystyrene blocks not appearing behind the compactor image in the canvas (3D effect)                          	| The order in which you add objects to the world determines the z-index. Adding the foreground image of the compactor after the polystyrene blocks allows the blocks to appear behind the image, giving the desired 3D effect. 	|
| 3   	| When user creates a polystyrene block, they appear in-front of the                                             	| Use add to world method within the polystyrene creation function and re-add                                                                                                                                                   	|
|     	| images, giving no 3D effect.                                                                                   	| the images on each call.                                                                                                                                                                                                      	|
| 4   	| On-screen messages were interfering with the mouse drag function                                               	| Add a style attribute of 'pointer-events: none;' to the message div                                                                                                                                                           	|
|     	| [Image of mouse drag bug](https://github.com/Wbwren/waste-matters/blob/master/assets/img/mouse-drag-bug.png) 	| [Image of mouse drag bug fix](https://github.com/Wbwren/waste-matters/blob/master/assets/img/mouse-drag-bug-fix.png)                                                                                                        	|
| 5   	| Could not get vertices to work correctly on matter.js                                                          	| This problem was not resolved.                                                                                                                                                                                                	|
|     	| [Image of vertices bug](https://github.com/Wbwren/waste-matters/blob/master/assets/img/vertices-bug.png)     	|                                                                                                                                                                                                                               	|
<br>

### Browser Compatibility
| Num | Browser         | Test result |
| ---|:-------------:| :----: |
| 1 | Chrome | Passed
| 2 | Opera | Passed
| 3 | Mozzilla | Passed

<br>

### Responsiveness Testing
* Chrome developer tools was used to test a wide variety of device sizes and resolutions.

* The website has been tested on an iPhone 5, Samsung Galaxy s10, Acer swift 3 and a desktop PC with a 1080p and 4k monitor.

* [Am I responsive image](https://github.com/Wbwren/waste-matters/blob/master/assets/img/am-i-responsive.png)

### Unresolved Bugs

* Users can turn on the compactor before placing any objects into it.

* When smaller devices are in horizontal view mode it can [break the responsiveness](https://github.com/Wbwren/waste-matters/blob/master/assets/img/small-screen-horizontal-view.png) due to canvas limitations with matter.js. However, as this website is primarily targeted to professionals looking to buy polystyrene compactors it is very likely it will be viewed on a desktop.  

### Google Lighthouse Scores
* [Lighthouse mobile result](https://github.com/Wbwren/waste-matters/blob/master/assets/img/lighthouse-results-mobile.png)
* [Lighthouse desktop result](https://github.com/Wbwren/waste-matters/blob/master/assets/img/lighthouse-results-desktop.png)

## Deployment to Github Pages
1. Create a Github account at [github.com](https://github.com/)

2. Click on the 'New' button in the top left corner

3. Enter a name for the repository, check the 'Add a README file' box

4. Click 'Create repository'

5. Open the repository in preferred integrated development environment

6. Save changes by clicking the save button

7. Once a feature has been successfully created using the 'git add .' command to stage the changes made

8. Then use the command 'git commit -m"[enter commit title here]"'

9. All meaningful changes to the code should have its own commit

10. To push the commits to Github use the command 'git push'

11. Once the website is ready for deployment return to [github.com](https://github.com/)

12. Click on the 'settings' tab

13. Scroll down to the 'GitHub Pages' section

14. Click the 'None' dropdown button

15. Select the master branch

16. Click save

17. After a few minutes, the site will be published to GitHub pages and can be accessed using the URL at the GitHub Pages section
## Clone
1. Follow this link to my [Github Repository](https://github.com/Wbwren/waste-matters).

2. Click 'Clone or Download'.

3. In the Clone with HTTPs section, click the 'copy' icon.

4. In your local Integrated Development Environment open Git Bash.

5. Change the current working directory to where you want the cloned directory to be located.

6. Type 'git clone', and paste the URL you copied before.

7. Press enter and your local clone will be available.
## Credits
### Media
* Compactor image: https://wastematters.ie
* Styrofoam texture: https://3dtextures.me/2019/03/21/styrofoam-001/
* P button image: https://www.pngkey.com/detail/u2w7q8e6y3e6a9a9_pow-button-mario-pixel-art-mario-christmas-pixel/
* Floor block image: https://webstockreview.net/image/brick-clipart-super-mario/125781.html
* Lever image: https://www.kissclipart.com/cartoon-lever-png-clipart-computer-icons-clip-art-1f8vxo/s
* Refresh-arrow: http://clipart-library.com/clipart/8T68KdEGc.html
* Green pipe: https://publicdomainvectors.org/en/free-clipart/Green-pipe/39369.html

### Acknowledgments
* [Stackoverflow](https://stackoverflow.com/) as a resource for learning and troubleshooting.
* [Matter.js documentation](https://brm.io/matter-js/docs/)
* [The coding train YouTube channel](https://www.youtube.com/user/shiffman/)
* A special thanks to my mentor Brian Macharia for his invaluable guidance throughout this project.
* Thanks to Simen Daehlin for his very helpful feedback on the project.
