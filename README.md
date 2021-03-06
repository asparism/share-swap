# share-swap
A website for exchanging timeshares



<div class="mdl-cell  mdl-cell--12-col message-card mdl-card mdl-shadow--2dp mdl-grid">
  <div class="mdl-card__title">
    <h3>Creating This Website</h3></div>
  <div class="mdl-card__actions mdl-card--border">
    <p>Probably the most impactful part of making this website was the use of Material Design Lite. The visual design was vastly simplified with MDL components.<br><br>
      <h4>MVC Architecture</h4>
      <ul>
        <li>Components, or segments of the website, were dynamically created and then appended to the "content" div of the HTML.</li>
        <li>In each of these segments, a parent div was created and all the elements were appended to the parent, which was then returned as a dynamically created HTML element.</li>
      </ul>
      <hr>
      <ul>
        <li>Because there wasn't much state to maintain, I opted for a global model instead of giving each component their own.</li>
        <li>An "update" object determined the view in two parts:
          <ul>
            <li>determining which component to append to the "content" div based on the state of the model</li>
            <li>clearing the innerHTML of the "content" div and appending a new component</li>
          </ul>
        </li>
        <li>Components were declared inside of a so-called component collection object, where they could be called as functions by the "update" object and returned the HTML elements that would be appended to the "content" div</li>
        <li>Creating and adding components was a lot easier because of this preexisting structure</li>
      </ul>
      <hr>
      <ul>
        <li>There were a lot things to consider as I thought about the structure of the code</li>
        <li>For example, should event listeners be added to an element immediately after it was declared, or should they all be located at the same place in the component's function?</li>
        <li>A small library of functions was used frequently, and this library was also updated as the project progressed. The more I built, the more I found opportunities to condense oft-repeated code into reusable functions. I created an "mdl" object which
          made it easy for me to dynamically write MDL components like input textfields</li>
      </ul>
      <hr>
      <h4>Things To Add/Improve</h4>
      <ul>
        <li>Save message draft</li>
        <li>Save My Share draft</li>
        <li>The search could be improved in these ways:
          <ul>
            <li>omit non-alphabetical/non-alpha-numeric characters in possible keywords</li>
            <li>omit repeated words</li>
            <li>stop the search early if a match is found</li>
            <li>ignore caps</li>
          </ul>
        </li>
        <li>Center sign up form correctly on mobile</li>
        <li>And realistically much more as the project moves more and more into the realm of actual production</li>
      </ul>
    </p>
  </div>
  <div class="mdl-card__actions mdl-card--border">
    <p>
      <h4>This website was created by asparism. Contact:</h4>
      <h5>asparism/Ian Lee</h5>
      <h5>
        <ul>
          <li>email: ianforrestlee@gmail.com</li>
          <li>portfolio: <a href="https://asparism.github.io" target="_blank">portfolio</a></li>
          <li>github: <a href="https://github.com/asparism" target="_blank">github.com/asparism</a></li>
          <li>codepen: <a href="https://codepen.io/asparism" target="_blank">codepen.io/asparism</a></li>
        </ul>
      </h5>
   </p>
  </div>
</div>
