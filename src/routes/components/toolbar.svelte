<h2 class="c-h2">Toolbar</h2>

<div class="c-content">
    
    <p>The toolbar is meant as a generic construct to position tools. It provides a structure where you can position items on the left, in the center and on the right.</p>

    <p>The toolbar requires a parent <code>.c-toolbar</code> div that contains children that define the positioning: <code>.c-toolbar-left</code>, <code>.c-toolbar-right</code> and <code>.c-toolbar-center</code>. Within those children, every item is contained in a  <code>.c-toolbar__item</code> div.</p>

    <p>This might seem excessive in terms of structure, but it provides a global method to position items, which is extremely powerful and avoids situational CSS.</p>

    <p>The toolbar construct can be re-used in many parts of the user interface: modals, panels, navbars and popovers all use the toolbar component to position elements in a consistent way.</p>
    
</div>