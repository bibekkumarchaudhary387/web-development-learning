10. HTML Frames and Framesets

10.1 What is frames?
-> Frames allow you to divides a single browser window into multiple sections. Where each section loads a sperate HTML document.

10.2 The <frameset> Tag:
-> This is the container that defines how the window is divided. It is uses two main attributes.
  *bullet* divides the window horizonally (e.g rows="20%, 80%").
  *bullet* divides the window vetically (e.g, cols= "15%, *"). The * means take the remaining space.

10.3 The <frame> Tag:
-> This tag defines the content for each section created by the frameset.
 *bullet* src -> The URL of the page to load in the frame.
 *bullet* name -> A unique name for the frame (used to rarget links).
 *bullet* noresize -> Prevents the user from draggin the frame border to chnage, its size.
 *bullet* scrolling -> can be set to yes, no and auto


Practical Exercise
To practice frames, you actually need three files. Create a new folder called Frame_Project and add:

menu.html: A simple page with a list of links.

content.html: A simple page with some text (e.g., "Welcome to the main page").

index.html (The Main Frame File):

Use <frameset cols="20%, 80%">.

In the first frame, load menu.html.

In the second frame, load content.html. Give this frame the name main_window.

Critical Challenge: In menu.html, create a link: <a href="https://tu.edu.np" target="main_window">Open TU Site</a>. This tells the browser to open the TU website inside the right-side frame instead of replacing the menu.