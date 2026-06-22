# Canvas Usage Insights

## Distilled General Insights

* **Games and Visualizations Lead Usage:** The most prominent use cases for the Canvas API are interactive and data-heavy applications. Games are the leading category at 56.7%, closely followed by Charting & graphical information at 49.8%.
* **Gaming is the Most Approachable Use Case:** Creating games is perceived as one of the easiest tasks within Canvas, with 43% of respondents rating the difficulty as "Neutral" and 26% rating it as "Easy". Conversely, plotting charts is more difficult, with 39% of developers rating charting as either "Difficult" or "Very difficult".
* **Custom Animations Pose the Greatest Challenge:** Working with custom animations (like Lottie or Rive) is a major friction point. It scored the highest in difficulty across all categories, with a combined 48% of users rating it as "Difficult" or "Very difficult".
* **Boilerplate is a Barrier to Entry:** Developers are frustrated by the amount of setup required just to get started. As one respondent noted, "There is so much boilerplate to doing anything in the API. The manual setting of various properties before being able to draw things properly, the long instantiation (creating canvas, getting 2d context) needed to do even basic things".
* **Developers Want Native Utilities and Math Helpers:** The API's lack of built-in foundational tools forces developers to recreate the wheel. One user stated, "There are no built in methods for common things so evrything needs to be written yourself, which is annoying". Specifically, developers requested additions like "A default interface for vector 2 and vector 3. And the normal math functions that help with vector math".
* **Certain Native Functions Need Redesigning:** Some existing API features are actively causing developer friction. The ellipse tool was explicitly called out: "I detest the ellipse function; its interface is infuriating to work with... The ellipse drawing functionality is badly designed".
* **Rendering Quirks Impact Visual Fidelity:** Quality control issues like anti-aliasing and aspect ratios are recurring complaints. One user noted that "for pixel art the image can look blurry or edges... might not exactly appear like they should". Others cited that "pixel aspect ratio is challenging" and mentioned a "known zoom blurry problem".
* **Performance Bottlenecks:** Performance optimization is highly requested, especially for complex operations and lower-end hardware. One respondent emphasized, "The chromium engine could use some optimization with the canvas api, as it is very hard to use on lower-end devices".
* **Lottie and Rive are Approaching SVG Dominance:** While SVG is the most used animation format at 60.9%, third-party complex animation libraries are highly prevalent. Both Lottie and Rive are used by 52.2% of respondents.
* **Strong Demand for Native Lottie Support:** Developers are incredibly eager to shed the performance weight of third-party JavaScript players. One user pointed out that "The Lottie library is a sizable overhead". If all browsers supported Lottie natively, a massive 64% of developers would immediately drop the JS player — and impressively, 61% would still stop shipping the player for a specific browser if even just one browser supported it natively.

> We had previously thought we’d need full native lottie support across browsers for developers to adopt native support and stop shipping the JS player, but the % of developers who’d use native support with just one browser vs. all is effectively identical 

---

## Specific Areas of Suggested Focus

### High Demand for Native Lottie
* “The Lottie library is a sizable overhead and using the Canvas API is somewhat cumbersome.”
* “Interactive stuff and playback control.”
* “No way to modify objects already on the canvas.”

### Making Canvas Easier to Use / More Ergonomic
* “CANVAS API ARE STILL COMPLEX IT CAN BE SIMPLE”
* “I wish the API threw more errors in lieu of returning nulls. I haven't found a case where I want to do anything other than fail if I can't get a context”
* “I detest the ellipse function; its interface is infuriating to work with.”
* “2D context is easy to use, WebGL is more difficult but that's mostly because I'm not that experienced with it.”

### More Built-in Functionality
* “A default interface for vector 2 and vector 3. And the normal math functions that help with vector math”
* “The native canvas api without any external lobraries to work over it is hard to use, counterintuitive and lacks a lot of functionality. There are no built in methods for common things so evrything needs to be written yourself, which is annoying. Ofent times the behavior of some functionalities is questionable at best and does not do what it is supposed to do”
* “There is so much boilerplate to doing anything in the API.”

### Canvas Performance
* “The chromium engine could use some optimization with the canvas api, as it is very hard to use on lower-end devices.”

### Pixel Aspect Ratio
* “Especially for pixel art the image can look blurry or edges of pixel art images might not exactly appear like they should. This can be disabled but it's not obvious.”
* “pixel aspect ratio is challenging”
* “I use echarts so not exposed to canvas problems other then the known zoom blurry problem which probably can be fixed by rerender after zoom”

### Suggestions Unrelated to Canvas
* Phone number verification
