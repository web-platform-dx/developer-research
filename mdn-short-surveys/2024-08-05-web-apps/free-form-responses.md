**I. Development & Technical Challenges**

*   **Cross-Browser Compatibility & Standards:**

    *   Web app manifest details and Apple platform icons and splash screens lol
    *   The fact that only Chromium seems to care about web applications. I need to tell my users to use Chromium-based browsers because Safari and Firefox won't implement features that are essential to be able to build web applications that have the same capabilities of native applications. I'm generally against a single product dominating its alternatives, but in this case I'm happy for the Chromium dominance, as other browsers are doing zero effort to bring native capabilities to web applications (actually, they are putting all their effort in stopping native capabilities to be added to the standards)	
    *   Apple deliberately slow-walking web technologies, especially PWAs
    *   Cross-browser support for APIs (Safari..), and architecting around this. Best practices for testing/debugging PWAs (i.e., installing, push notifications, etc)
    *   Some things just aren't supported in some mobile browsers (eg. issues with Huawei devices) or some things aren't implemented in the same way (eg. Safari does weird things sometimes)
    *   poor apple support
    *   Lack of full support for web push notifications and other PWA features in iOS safari (orientation lock, deep linking). Basically this tweet: https://x.com/dannymoerkerke/status/1803055577100091874
    *   Browser quirks
    *   Not being able to test my PWAs on Safari browsers without owning an Apple computer and iPhone, which is somewhat critical considering the overall poor implementation of web standards on Safari.
    *   Getting Apple to support all PWA features in iOS
    *   Browser support. Chrome has always been the best for this because of the assortment of web APIs that are meant for installable app usage. Browser compatibility becomes a chore, it becomes a question of "should I even bother doing alternative/fallbacks when the experience is subpar?" I care very much about what users (which includes me in the group) experience, and to me a subpar experience is worse than none at all.	
    *   Support and inconsistency. Firefox doesn't support it at all. And those that do support it, things are very inconsistent between different browsers and platforms.
    *   Apple putting hurdles
    *   Different API support/implementation by browser vendors
    *   · Web Runtime (Webview) is not open, not in Standard, and Chromium-only. · Web applications generally have more failure points than the native ones. · Web itself is still not designed for application. See below: Web itself is still not designed for application. Application development is not feasible under Web. The frameworks can't really solve this, they only make Web App development more complex. What's more, Web development is also very open to bad practices. Many will not take Web applications seriously, when they realize Web Apps can use eval() freely, and window.alert() hangs the execution. We need more feature for App, and enforce good practices in Web App development. Maybe even something like < !doctype application>.
    *   Interoperability
    *   Getting styles to appear consistently across browsers has been the biggest issue, to the point that I re-implemented all the graphical logic of the app into JS and manually output everything to a canvas for visuals. Even after all that, getting the canvas to look the same on all browsers is still an issue.
    *   cross platform support
    *   Supporting multiple browsers.
    *   Apple :( And for mobile: Being unable to deactivate swipe navigation reliably
    *   Browser interoperable and framework churn.
    *   Cross-platform compatibility.
    *   compatibility
    *   Testing features on all platforms, thankfully I got a free Browserstack subscription for my FOSS app.
    *   Varying support for basic features between the platforms leaves you uncertain if it's worth it.
    *   1. Levels of specification implementation differs by OS 2. various bugs for each OS.
    *   Apple support.
    *   Browser support
    *   consistency across device and os. web apis are pretty exhaustive and well supported currently which is great, but the experience is never in parity between ios and android (the main targets of the installable apps) and the same is true of macos and windows, but to a less impactful degree.
    

*   **API Limitations & Access to Native Features:**

    *   Local notifications, especially when you consider oftentimes, web apps will not need access to a network once installed and would make Push Notifications more expensive/complicated for the developer to implement.
    *   File system interactions - for me, completely eliminates the possibility of using PWAs for more complex apps
    *   Accessing lower level APIs, and ensuring high quality offline availability
    *   Not being able to start a TCP Client. This happened to me twice already, and I had to use a Node & Rust backends to solve it
    *   Background tasks e.g. tracking the geolocation when the app is closed.
    *   Native video encoding. Push notifications. Fancy compositing effects (manipulating image of elements on the page)
    *   Access to all device capabilities, such as nfc or bluetooth.
    *   limitted access to native device features
    *   Accessing native functions using web developing languages
    *   - Limited access to native device APIs - Setting up proper offline support can prove tricky. Native apps are just more capable of doing more offline than PWAs. Simpler browser APIs are needed to declaratively say "when this PWA is installed, fetch the code for the following routes and keep them permanently offline". As of right now, there's too much boilerplate involved to get this set up in a service worker..	
    *   Accessing native Components like Bluetooth or long running background tasks while the app is in the background
    *   hard to call native apis
    *   Access to device storage and receiving intends would be helpful. Registering background conditions (location, location change, a duration) would be very helpful to implement proper background functionality
    *   Push Notifications Storage
    *   access to hardware resources
    *   The file IO and other local needed operation. Like i want to read a file by path and it can't be implement with PWA or other web app framework
    *   Access of native notification system and replicate back navigation button of native mobile apps
    *   Integrations into native OS systems.
    *   No more PWA Support on OS.
    *   Support for background support for sensors such as background GPS location. Another one is background timers for scheduling notifications on a cron job.
    *   The most difficult part is the workarounds to make it work on iOS devices, due to some limitations on Safari, I need to rethink some standard APIs like FileSystem, screen orientation, CSS anchor positioning, etc.
    *   So far, the biggest difference between native and web is that on native you only have to request access to a resource once (for instance microphone), but on—iOS specifically— the user has to confirm access during each use of the app. Not a deal breaker, but would be more seamless if those options were retained/can be configured.
    *   Interacting smoothly with the filesystem
    *   No notification support on IOS, no background fetching.
    *   Integration with system interactions, using WebApps to recognize that they are not native apps, especially when opening and interacting with apps.
    *   Multi threading and accessing native features. Performance, dependency with browser vendors.


*   **UI/UX & Design:**

    *   Seamless integration with the Native System UI. For example, a button on Windows feel and look different from a macOS button, and the position is also different. Also, even in the same operating system the UI differ, is not the same Windows 10 from Windows 11 I know this could just be ignored the same way all Electron apps did, but for me is a bit annoying.
    *   building animatable ui
    *   design
    *   Non standard ui library
    *   The biggest challenge building web application is making UI interface
    *   a cross platform UI, local file managment
    *   Making them pretty.
    *   1. Managing the soft keyboard state (open/close it), and creating a layout that responds to the keyboard geometry 2. Managing the safe-area-inset for iOS. 3. Inconsistent cross- platform behavior of contentEditable.
    *   Functional use for the user
    *   ability to blend with system UI in a way similar to native apps. users notice small things like this (e.g. text selection which is implicitly allowed on web platforms/implicitly disabled on native, some scrolling behaviours, etc.) but don't understand the reason behind them, so they just see it as unusual behaviour and see the app as less trustworthy
    *   Designing the front end
    *   Platform consistency (i.e., the app doesn't look native) and lack of lower-level APIs.
    *   Responsive CSS
    *   The user interface still takes about 80% of the work required
    *   Make the experience more like a native app with some animations and transitions that only the apps have in palm of your hand.
    *   In this context, being able to meet (much less exceed) user expectations on interaction, animation, and responsiveness. I've found Windows and Android users don't see as much of a difference than iOS/macOS users, as the latter cite smoother animations, and better UX in general, which aren't always possible on the web (see view transitions).
    *   structure and templating
    *   css layout is a mess. no matter how many times it has been improved on, it seems unsalvageable

*   **Performance & Optimization:**

    *   size and performance
    *   Performance, accessibility and anti-piracy
    *   Performance compare to native is bad.
    *   Performance, tooling Sometimes you only need a tiny, optional binary to run on the actual system, but it's hard to connect those two.
    *   Making sure it doesn't run like absolute garbage
    *   low speed and optimizations
    *   Multi threading and accessing native features. Performance, dependency with browser vendors.

*   **Frameworks, Tools, and Ecosystem:**

    *   Getting the current framework (NextJS) to play nice on PWA
    *   Staying away from unnecessary libraries/frameworks/dependencies. Standard web technique is quite nice nowadays and very usable without a lot of the extra stuff nowadays.
    *   New flavor of the month frameworks. React syntax looks bad. Hail vanilla JS.
    *   javascript building system, tool, module, versioning,
    *   Browser interoperable and framework churn.
    *   Ever changing technologies/frameworks.
    *   Making frontend frameworks and pwa work together, synchronising data and keeping it locally, accessing the full app offline
    *   The updation of service worker is a headache when used with frameworks.
    *   A lot of tools that do the same thing but only a few of them doing it good
    *   Lack of standards and great bunch of different tools
    *   Integrating frontend with backend technologies
    *   Constant change in the technology

*   **State Management & Data Handling:**

    *   Browser storage. Without certainty about longterm status of an app's storage, it's hard to make a truly mission critical app. The web treats website storage as a cache it can clear at any time. We had to do a ton of work to make sure all user data was backed up because we couldn't rely on the OS at all.
    *   managing updates with service workers - sometimes some parts of the app are updated but others aren't? probably a skill issue tho
    *   - custom session management (user can see how many active sessions in other devices). - THE BIGGERST PROBLEM i had is struggling with browser's back button and handle back button event, there is no standart between browsers and that was pain for me
    *   Offline usage and data persistance
    *   I tried to used ffmpeg.wasm for transcoding on browser. It works on mostly works on Edge, Chrome but failed on others. (mostly memory limit of browsers) Cross-Origin-Opener-Policy: same-origin Cross-Origin-Embedder-Policy: require-corp these headers and focus on "crossOriginIsolated" killed the payment gateway and some other APIs. I find workaround, but still it was too slow and buggy. I delete all those codes from frontend and make it on backend. Now, there is no other problem.
    *   keep the code simple so it can be maintainable - it's all about "state'
    *   System design & Database design
    *   adding raw data on the web applications
    *   Safari *aggressively* deleting my user's data. What a shit browser.
    *   Limited capabilities to customize window header on desktop. Missing functionality that allows to add different translations in manifest.json (name and description for the app and shortcuts). In this case we need to prepare different builds of the app. Missing built- in functionality that makes data caching easier, without custom implementations using service workers. No clear standards regarding cache data retention on different platforms/browsers.


*   **Service Workers & Offline Functionality:**

    *   Building a more complex service worker
    *   Discovery, offline caching (service workers are waaay too complicated and prone to breakage).
    *   As of right now, there's too much boilerplate involved to get this set up in a service worker..
    *   Tighter integration with native services, inconsistency of features across platform (eg navigator.vibrate), lack of forced orientation on mobile, need for "black box" libraries like workbox to implement service workers correctly
    *   Making frontend frameworks and pwa work together, synchronising data and keeping it locally, accessing the full app offline
    *   The updation of service worker is a headache when used with frameworks.
    *   - Limited access to native device APIs - Setting up proper offline support can prove tricky. Native apps are just more capable of doing more offline than PWAs. Simpler browser APIs are needed to declaratively say "when this PWA is installed, fetch the code for the following routes and keep them permanently offline". As of right now, there's too much boilerplate involved to get this set up in a service worker..	



**II. User & Business Challenges**

*   **Users expecting to get apps from an app store:**

    *   Teaching users how to access the "add to homescreen" function.
    *   The immutable mindset of users that apps come from an appstore.
    *   Customers don't know the web capabilities, so don't know what to ask.
    *   Users don't understand what installable web apps are, or how to install them.
    *   Mobile adoption and mobile user acquisition.
    *   Getting users to be aware they can install web apps on their devices
    *   getting people to install them, they should be allowed in app stores
    *   For me, the biggest drawback of PWAs is gaining the trust needed to install something on your mobile device that doesn't come from the Google Play Store or Apple App Store
    *   Conditional/programmatic prompt for installation. Transperancy regarding permissions/more control over how it's presented to the user. Better integration with the OS.
    *   Shipping to an app store
    *   True install-ability. Only Chromium browsers provide the "native" functionalities that I look for: standalone PWA and dedicated file-opening.
    *   Integration with system interactions, using WebApps to recognize that they are not native apps, especially when opening and interacting with apps.



*   **Business & Development Process:**

    *   Deciding on hosting platform probably. I've found push and webauthn quite frustrating to implement too.
    *   Understanding business process
    *   -compiling with xcode is a pain in the.. -setup and obtain a verified an apple store account -too many apple guidelines -have 50 testers on play store for individual dev
    *   Biggest challenge to build a web app is to learn 3 languages. HTML CSS JavaScript. There are frameworks which is making the process easier but in most of the cases we have to learn HTML CSS JavaScript mandatory. In android we can build apps only by learning 1-2 things majorly.
    *   Using multiple API's and running into CORS errors, then utlizing Backend as I am not full stack, I am mainly a front end developer with some UI skills.


**III. Other & General Challenges**

*   **Documentation & Learning Resources:**

    *   Not enough documentation. Additionally, when using a javascript framework to make PWA, it is quite difficult due to not much being written on the subject
    *   As a newbie developer no one really teaches how to build web apps, they teach the tools and different features that you can use but not what's the most efficient way to put them together
    *   So much outdated information available.
    *   setting up project
    *   The web platform, especially the JavaScript eco system is a very fast moving target. It's hard to stay up to date with the state of the art imho.
    *   tooling and documentation
    *   learning
    *   Figuring out its quirks, what I can and cannot do and starting out.
    *   deploy :)
    *   Getting good specs
    *   The challenge of where to start is a challenge

*   **Security:**

    *   Network & Information Security, also Data Protection Privacy.
    *   Deploying in a production environment. Knowing what the best security practices are.
    *   security

*   **Uncategorized/Unclear:**

    *   different
    *   no
    *   None
    *   Yes
    *   Not killing myself when writing JS
    *   Making enough good as native apps
    *   Nothing
    *   Toi mong lắm rồi
    *   tonyjaa
    *   6V8PPM
    *   Orders
    *   good
    *   {b6d24b9b-9379-423f-bd33-fbab1d0bba6f}:"value"
    *   types
    *   Passionate
    *   Online Money tik tok
    *   Eradicate proprietary solutions that exist only to regress technology.
    *   < canvas id="canvas">< /canvas>
    *   few in responsive issue
    *   compability with old phones and tablets
    *   Making typescript happy.
    *   compatibility with minimum resource devices.
    *   太多解决方案。 当然这不是坏事，我只是说对于一个学习者来说，太多的方案令人难以选 择。
