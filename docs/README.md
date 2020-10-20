# MS 1 Project



User Stories
======

As **an event organiser**, I want to **post the event with all the relevant details** so that **I can sell tickets on the website**.

As **a visiting user**, I want to **view upcoming events** so that **I can buy tickets to events I like**


Strategy
======

Build a website that allows event organisers to post events and allows visiting users to buy tickets to attend these events.

Scope
====== 

#### Features:

Event organisers can post all relevant details about their event and the tickets they are selling for that event.

Visiting users can browse events and buy tickets to events that they would like to attend.

#### Product Limitations:

There is no backend or no stripe limitations. When a user posts an event or purchases tickets the button will bring them back to the homepage.

#### Future Features:

Integration with Stripe to take credit card payments.

User accounts can be created.

Customer credit card details can be saved for future use.

Event organisers can sell as many or as few ticket types (early bird, general admission, back-stage access etc.) as they want.

Event organisers can decide when each ticket type will start and stop selling. They can choose to allow tickets to start selling at a specific date or time or when another specific ticket type is sold out.

When an event is sold out, customers can choose to store their credit card details to be charged if another customer requests a refund.

Event organisers can decide to only allow refunds if another customer has saved their credit card details and is waiting to buy the ticket.

Event organisers can re-sell refunded tickets for a higher price.


Structure
======

The home page will list all of the events and show summary details for each event. When a user clicks an event, they will be brought to that event's specific page.

The event page will have a image for the event; display all the details relating to the event (start time and date, location etc.); it will display the tickets for purchase; an option of the user to select how many of each ticket they wish to purchase and a button to complete purchase.

The create event page will contain a form allowing the event organiser to post event details - name of event, location, start date and time, end date and time. 
There will be three ticket types (eg. early bird, general admission, back-stage access etc.) for each event. 
For each ticket type, the event organiser must include a name of the ticket type, the price and the quantity of tickets to sell. There will be an option to include a description.

In the header, I will include a nav bar that has links to the home page and a 'create event' page. This will be on every page.

In the footer, I will include a copyright notice and links to social media platforms. These will open in a new window. This will be on every page.


Skeleton:
======

Wireframes are available [here](./wireframes.pdf)


Surface:
======

Background grey: #eeecec
Dark grey: #8f897c
White: #fff
Black: #000
Dark Blue: #293d6a
Fonts: Nunito and Bitter from Google Fonts


Resources:
======

Testing:
======

Project barriers and solutions:

Couldn't add shadow to tickets because they are comprised of two many divs.

======

Version control:
======

Deployment:
======

Credits:
======

Tickets based on https://codepen.io/verpixelt/pen/cEJLa 

Colors from www.rte.ie/news and www.gaytodo.com

Nav links animations from https://codepen.io/chancesq/pen/qBOyQoW

https://stackoverflow.com/questions/6805482/css3-transition-animation-on-load

https://stackoverflow.com/questions/11679567/using-css-for-a-fade-in-effect-on-page-load

https://www.freecodecamp.org/news/how-to-keep-your-footer-where-it-belongs-59c6aa05c59c/

https://codepen.io/sdthornton/pen/wBZdXq

https://codepen.io/zesht/pen/MWgQxer

pics from unsplash:
https://unsplash.com/photos/hzgs56Ze49s
https://unsplash.com/photos/3ckWUnaCxzc
https://unsplash.com/photos/juHayWuaaoQ

Text for party event from https://www.eventbrite.ie/e/psychedelic-gaff-23-dark-progressive-night-w-hypogeo-tickets-96357603185?aff=erelexpmlt

Credit Card Details CSS: https://designmodo.com/create-credit-card-ui/#download-the-credit-card-html

Glowing input: https://css-tricks.com/snippets/css/glowing-blue-input-highlights/

Button Grows on hover from https://css-tricks.com/snippets/css/scale-on-hover-with-webkit-transition/

Remove blue border when input selected: https://stackoverflow.com/questions/1457849/how-to-remove-the-border-highlight-on-an-input-text-element

Credit Card Number will only accept 16 digits: https://www.w3schools.com/tags/att_pattern.asp

Prevent horizontal overflow. Second Answer here: https://stackoverflow.com/questions/23367345/100vw-causing-horizontal-overflow-but-only-if-more-than-one

Acknowledgements: 
======
My Code Institute Mentor, Rohit

https://css-tricks.com/snippets/css/a-guide-to-flexbox/
https://www.w3schools.com/icons/fontawesome_icons_intro.asp
https://css-tricks.com/min-max-and-clamp-are-css-magic/





