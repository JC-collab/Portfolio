# portfolio

This project was a challenge as I struggle with html positioning and targeting the correct element with CSS.  Working from scratch (after re-watching all the videos) my comfort level increased greatly.

Reactive:

I did get the reactive to work, on the main page I gave background colors to the lower third of the main page as it would provide visual indicator to size changes.

/* the bottom oart of the page will have a light gray backgrown, the intent is to practice HTML-reactive skills, for tablet it should change to light green, then light red*/

#showcase .skills .lower-third p {
    background-color: rgb(161, 161, 161);
}

/* Tablet Style*/

@media only screen and (min-width:401px) and (max-width: 960px) {
    #showcase {
        background: url(../img/BackGroundBanner-2.jpg) no-repeat center center/cover;
        height: 1200px;
        margin: auto;
    }
    #showcase .lower-text {
        margin-top: 200px;
        margin-left: 40px;
        margin-right: 40px;
    }
    #showcase .skills .lower-third p {
        background-color: rgb(181, 231, 181);
    }
}

@media only screen and (max-width:400px) {
    #showcase {
        background: url(../img/BackGroundBanner-2.jpg) no-repeat center center/cover;
        height: 1500px;
        margin: auto;
    }
    #showcase .lower-text .info {
        font-size: 20px;
        font-weight: 400px;
        line-height: .5px;
    }
    #showcase .skills .lower-third p {
        background-color: rgb(236, 181, 181);
    }
}

