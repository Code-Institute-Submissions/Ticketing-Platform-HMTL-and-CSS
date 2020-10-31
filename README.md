# MS 1 Project

Purpose of Project
======

Create a ticket selling platform.

Event organisers can post all relevant details about their event and the tickets they are selling for that event.

Visiting users can browse events and buy tickets to events that they would like to attend.


User Stories
======

As **an event organiser**, I want to **post the event with all the relevant details** so that **I can sell tickets on the website**.

As **a visiting user**, I want to **view upcoming events** so that **I can buy tickets to events I like**


Features
====== 

#### Home Page:

![home page screen shot](https://github.com/colmfah/Ticketing-Platform-HMTL-and-CSS/blob/master/assets/images/home.png?raw=true "Home Page")



The home page will list all of the events and show summary details for each event. When a user clicks an event, they will be brought to that event's specific page.

#### Event Page:

![event page screen shot](https://github.com/colmfah/Ticketing-Platform-HMTL-and-CSS/blob/master/assets/images/event.png?raw=true "Create Event Page")

The event page will have a image for the event. 

It will display all the details relating to the event (start time and date, location etc.). 

It will display the tickets for purchase. 

An option of the user to select how many of each ticket they wish to purchase and a button to complete purchase.

#### Create Event Page:

![create event page screen shot](https://github.com/colmfah/Ticketing-Platform-HMTL-and-CSS/blob/master/assets/images/create.png?raw=true "Create Event Page")

The create event page will contain a form allowing the event organiser to post event details - name of event, location, start date and time, end date and time. 

There will be three ticket types (eg. early bird, general admission, back-stage access etc.) for each event. 

For each ticket type, the event organiser must include a name of the ticket type, the price and the quantity of tickets to sell. 

There will be an option to include a description.

#### Header:

In the header, I will include a nav bar that has links to the home page and a 'create event' page. This will be on every page.

#### Footer:

In the footer, I will include links to social media platforms. These will open in a new window. This will be on every page.


#### Product Limitations:

There is no backend or no stripe limitations. When a user posts an event or purchases tickets the button will refresh the page.

#### Future Features:

Integration with Stripe to take credit card payments.

User accounts can be created.

Customer credit card details can be saved for future use.

Event organisers can sell as many or as few ticket types (early bird, general admission, back-stage access etc.) as they want.

Event organisers can decide when each ticket type will start and stop selling. They can choose to allow tickets to start selling at a specific date or time or when another specific ticket type is sold out.


Typography and Color Scheme:
======

Background grey: #eeecec
Dark grey: #8f897c
White: #fff
Black: #000
Dark Blue: #293d6a
Fonts: Nunito and Bitter from Google Fonts

Skeleton:
======

Wireframes are available [here](/docs/wireframes.pdf)

#### Changes to wireframe:

The footer only has social media icons that are spaced evenly using flexbox because I think this looks better.

The footer is the same for mobile and desktop as there is sufficient space on the smallest screens for code to work.


Technology:
======

HTML5
CSS3

Tested HTML using https://validator.w3.org/
Tested CSS using https://jigsaw.w3.org/css-validator
Browser prefixes from https://autoprefixer.github.io/
Gitpod


Best Practices:
======

Used camel-case for class selectors. 

Each class starts with the page or feature it applies to.

For example a class that impacts the home pages starts with "home-"; a class that impacts the create event page starts with "create-"; a class that impacts the nav starts with "nav-" etc.

Testing:
======

Tested HTML using https://validator.w3.org/. No errors displayed.

Tested website on chrome, firefox and safari on a desktop map and tested on chrome and firefox on an andriod mobile.

Used google chrome simulator to test for responsiveness for moto g4, galaxy s5, pixel 2, pixel 2xl, iphone5/se, iphone 6/7/8, iphone 6/7/8 plus, iphone x, ipad, ipad pro, surface duo, galaxy fold and desktop.

I have tested the credit card form in the events page by attempting to submit while leaving each input blank one by one and entering values other than 16 digits for credit card numbers and less than 3 digits for CVV numbers. The form would not send and displayed error.

I have tested the create event form by leaving each input blank one by one and also by selecting a value less than zero for price and less than one for ticket quantity. The form would not send and an error was displayed.

#### Fixed Issues:

Initially I had the image, summary details, description and tickets all contained in the one flexbox container. This worked for all default phone and tablet sizes in google chrome developer tools but at certain screen lengths, it caused the page structure to collapse. I fixed this by putting the image and summary details in one flexbox and the other elements into a separate flexbox.

Tried using maxlength and minlenght to ensure user would get error if they didn't enter credit card with 16 digits and cvv code with 3 digits. This wouldn't work so I used the html pattern attribute instead. Acknowledgement to W3 school is in Acknowledgement section.

There was a horizontal scrollbar even though elements were set to 100vw. This is because a visual error is caused when the vh is above 100vh. Fixed this using `overflow-x:hidden`. Acknowledgement to stackoverflow answer is in the Acknowledgement section.

Content was scrolling over the nav bar. I fixed this by giving the nav `z-index: 2`. This works because the only other z-index on the page has a value of 1


#### Open Issues:

Couldn't add shadow to tickets because they are comprised of two many divs. If tickets were constructed better, this would be possible.

`<input type="datetime-local">` is not supported by safari. `<input type="time">` is also not supported by safari

Tested CSS using https://jigsaw.w3.org/css-validator. It highlighted that `.cardWrap` has the same color and background-color. However this is required for the ticket overall to display properly. It also highlighted that, when checked, the radio button's border color is the same as its background color. I am also satisfied this is okay as there is a gap between the border and the button. The other warnings all related to code that I imported from elsewhere in the internet. All other warnings relate to vendor extension. After seeking advice on slack, I have not changed these.

Version control:
======

This project was developed using Gitpod, committed to git and pushed to GitHub using the built in function within Gidpod.

Deployment:
======

To deploy this page to GitHub Pages from its GitHub repository, the following steps were taken:

* Log into GitHub.
* From the list of repositories on the screen, select colmfah/Ticketing-Platform-HMTL-and-CSS.
* From the menu items near the top of the page, select Settings.
* Scroll down to the GitHub Pages section.
* Under Source click the drop-down menu labelled None and select Master Branch
* On selecting Master Branch the page is automatically refreshed, the website is now deployed.
* Scroll back down to the GitHub Pages section to retrieve the link to the deployed website.

To clone this project from GitHub:


* Follow [this link to the Project GitHub repository](https://github.com/colmfah/Ticketing-Platform-HMTL-and-CSS).
* Click the Code button.
* Copy the HTTPs URL.
* In your local IDE open Git Bash.
* Change the current working directory to the location where you want the cloned directory to be made.
* Type git clone, and then paste the HTTPs URL you copied.
* Press Enter. Your local clone will be created.

Credits:
======

Tickets based on https://codepen.io/verpixelt/pen/cEJLa 

Colors from https://www.rte.ie/news and https://www.gaytodo.com

Nav links animations from https://codepen.io/chancesq/pen/qBOyQoW

CSS transitions on load from: https://stackoverflow.com/questions/6805482/css3-transition-animation-on-load

Fade in on load from: https://stackoverflow.com/questions/11679567/using-css-for-a-fade-in-effect-on-page-load

Keep footer at bottom of page from: https://www.freecodecamp.org/news/how-to-keep-your-footer-where-it-belongs-59c6aa05c59c/

Box shadows from: https://codepen.io/sdthornton/pen/wBZdXq

images from unsplash:
* https://unsplash.com/photos/hzgs56Ze49s
* https://unsplash.com/photos/3ckWUnaCxzc
* https://unsplash.com/photos/juHayWuaaoQ

Text for party event based on https://www.eventbrite.ie/e/psychedelic-gaff-23-dark-progressive-night-w-hypogeo-tickets-96357603185?aff=erelexpmlt

Text for hike event based on https://www.meetup.com/Hiking-in-Wicklow/events/273609230/

Text for zumba classes based on https://westwood.ie/fitness-classes/class-descriptions/zumba/

Credit Card Details CSS: https://designmodo.com/create-credit-card-ui/#download-the-credit-card-html

Glowing input: https://css-tricks.com/snippets/css/glowing-blue-input-highlights/

Button Grows on hover from https://css-tricks.com/snippets/css/scale-on-hover-with-webkit-transition/

Remove blue border when input selected: https://stackoverflow.com/questions/1457849/how-to-remove-the-border-highlight-on-an-input-text-element

Credit Card Number will only accept 16 digits: https://www.w3schools.com/tags/att_pattern.asp

Prevent horizontal overflow. Second Answer here: https://stackoverflow.com/questions/23367345/100vw-causing-horizontal-overflow-but-only-if-more-than-one

Upload image: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input/file

Make placeholder show for input="datetimelocal": https://stackoverflow.com/questions/20321202/not-showing-placeholder-for-input-type-date-field/23683687#23683687

html select date and time: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input/datetime-local

Style radio buttons: https://stackoverflow.com/questions/45327086/how-change-the-color-of-the-radio-button

Style hrs - code based on: https://css-tricks.com/examples/hrs/

Placeholder changes color on hover based on https://stackoverflow.com/questions/54308139/how-to-show-placeholder-when-we-hover-on-input-type-text

Style child when hovering on parent from https://stackoverflow.com/questions/7217244/style-child-element-when-hover-on-parent

Fav icon from https://favicon.io/emoji-favicons/ticket

Flex box troubleshooting: https://css-tricks.com/snippets/css/a-guide-to-flexbox/

Font awesome troubleshooting: https://www.w3schools.com/icons/fontawesome_icons_intro.asp

CSS property clamp: https://css-tricks.com/min-max-and-clamp-are-css-magic/


Acknowledgements: 
======
My Code Institute Mentor, Rohit






