8. CSS Layout (Positioning, float and Flexbox)

8.1 The position property:
-> This property determines how an elemnet is placed in the document.
  *bullet* Static -> The default. Element following the normal flow of the page.
  *bullet* relative -> positioned relative to its normal position. You can move it using top, right, left, bottom without affecting other elements.
  *bullet* absolute -> positioned relative to its nearest ancestors (an ancestors with relative, absolute or fixed). It is "removed" fom the normal.
  *bullet* fixed -> positioned relative to the browser window. It stays in the same place even when you scroll.
  *bullet* sticky -> swtiches between relative and fixed depending on the scroll position (great for navigation bars).

8.2 Float and CLear
-> Before modern layout, we used to fixed to put element side by side.
 *bullet* float: left; -> pushes the element to the left and allows text to wrap arroung it.
 *bullet* clear: both; -> prevent elements from floating next to a specitic box. It "clear" the float effect.

8.3 Flexbox
-> Flexbox is a 1 dimensional layout model. It makes aligning items incredibly easy. To start using it set display: flex; on the parent container.

 Parent Properties:
   *bullet* flex-direction -> row(default) or column
   *bullet* justify-content -> align item horizontally (center space-between, space around).
   *bullet* align-item ->align item vertically (center, flex-start, flex-end)

Practical Question:

Create a navigation bar and a two-column layout using Flexbox.
HTML (day8.html):
Create a <nav> with 3 links.
Create a <div> with class="main-content".
Inside it, create two <div> elements: class="sidebar" and class="content".
CSS (style.css):
Use display: flex and justify-content: space-around on the <nav>.
Use display: flex on .main-content.
Give the .sidebar a width: 30% and .content a width: 70%.