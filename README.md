<h1>Lottie Component</h1>
<h2>Details</h2>
<ul>
<li>Allows one or two Lottie files, in order to support different aspect ratios.</li>
<li>A Lottie file only loads when 50% of the component is in viewport.</li>
<li>A single button controls Play/Pause/Replay functionality. Note that if the Lottie player is set to loop, the Replay icon will never appear.</li>
<li>If two Lottie files are defined and the browser is resized above/below the defined 767px breakpoint, the visible one will stop on the last frame, while the next one will load and play. Any subsequent resize of the brower will keep them stopped on the last frame.</li>
<li>prefers-reduced-motion is honored and will jump the Lottie player to the last frame and stop.</li>
<li>aria-label is on the component to provide a description of the animation for screen readers.</li>
</ul>

<h2>Considerations</h2>
<ul>
<li>When part of a framework, you'll want to dynamically get and set aspect-ratios during build. You can do this by fetching and parsing the JSON file for 'w' and 'h', and pass those as an aspect-ratio to a CSS Variable.</li>
<li>When providing guidance to the person creating Lottie animations, encourage consistency in sizes/aspect-ratios, and ensure the last frame displays all of the content.</li>
</ul>

<h2>Demo</h2>
<p>There are two Lottie components on this page. The first has two files defined, which have different aspect ratios. The second only has one file.</p>
