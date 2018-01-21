----------- ----------- ----------- ----------- -----------

                         OBSHAGCE

   The Official Blueberry Soft Hypermedia Adventure Game
                    Construction Engine

----------- ----------- ----------- ----------- -----------

       https://github.com/ryliejamesthomas/obshagce

----------- ----------- ----------- ----------- -----------

 Hi!

 This is a little framework / template thing I'm working on
 for building hypermedia adventure games--simple
 collections of HTML and CSS and whatever media you want to
 stick in there.

 I've tried to keep things easy to understand, so avoided
 Javascript and any ideas about trying to keep it as one
 page (EVIL). The only thing that's kinda dynamic (?) is
 the status window, which is a iframe. Otherwise each board
 is it's own HTML page with some inline CSS. There's a
 general style sheet (base.css) too.

 I hope this will encourage people to make more cool,
 personal websites. And explore the possabilites of a
 JS-free WWW.

----------- ----------- ----------- ----------- -----------
                           Goals
----------- ----------- ----------- ----------- -----------

 - Easy to read markup (with comments).
 - Be a useful earning tool for HTML and CSS.
 - No Java Script
   (but feel free to fork if you're into that).
 - Help show games can use simple technologies.
 - Promote cool, simple hypermedia.

----------- ----------- ----------- ----------- -----------
                     Project structure
----------- ----------- ----------- ----------- -----------

 /
 ├─ boards/
 │  ├── ...
 │  └── ...
 ├─ images/
 │  ├── ...
 │  └── ...
 ├─ messages/
 │  ├── ...
 │  └── ...
 ├─ sounds/
 │  ├── ...
 │  └── ...
 ├─ base.css
 ├─ games_list.txt
 ├─ index.html
 └─ readme.txt

----------- ----------- ----------- ----------- -----------

 So a game might work like this:
 You make a title/intro screen in index.html
 This points to HTML files in 'boards'
 These files have graphics and text and things you can
 click on in the cells on the right (what I call the board)
 and these open text, or HTML, or sounds, or whatever in
 the message widow in the lower left.
 You can also add some stuff to describe what is 'seen',
 'smelt', 'touched' etc., under the icons for those senses.

----------- ----------- ----------- ----------- -----------
                     Style Sheet Stuffs
----------- ----------- ----------- ----------- -----------

 Trying to explain the purpose / use of the IDs and
 classes used.

----------- ----------- ----------- ----------- -----------
 IDs:

 'splashimage'	For title screen images.

 'windows'

----------- ----------- ----------- ----------- -----------
 Classes:

 'board'        References the main game board.

 'heading'

 'senses'       The

 'sensed'

 'title'

 'window'       References elements that make up the main
                three windows, but exludes their contents.

 Also included at the end of 'base.css' are some clases you
 can apply for graphic effects. For example alignment and
 rotation.

 'align_*'      For easily alligning things in cells.

 'empty'        To make a cell as empty. It removes the
                border, so if used in the main game board
                the cell will not be indented.

 'no_scale'     For images you don't want to scale to fill
                a cell.

 'rotate_*'     For rotating elements, in 90 degree
                increments.

 And some classes for animated effects :)

 'blink'        Replicates the old <blink> tag. You can
                easily set the speed to your liking.

 'cycle'        A colour-cycling effect. Quickly cycles
                through a set of colours. Colours are easy
                enough to change. If you want to add more
                you'll need to add more steps (the numbers
                with the percent signs).

----------- ----------- ----------- ----------- -----------
 HTML

 <base target="message_frame">
                This makes links open thing in the message
                window unless told otherwise. Other targets
                you might find useful are
    _self       to open in the same window, and
    _blank      to open in a new tab or window depending
                on how the person's browser is set-up.

----------- ----------- ----------- ----------- -----------
----------- ----------- ----------- ----------- -----------
