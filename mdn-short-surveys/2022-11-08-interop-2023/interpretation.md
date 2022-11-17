# Interpretation

The results of both surveys were summarized and posted to the interop repo. That is inlined here.

## Results of MDN CSS & HTML survey

| Value | Percent | Responses |
| -- | -- | -- |
| CSS media queries range syntax (example: `@media screen and (428px < width < 744px)`) | 36.9% | 236 |
| CSS custom properties (`@property`) | 28.3% | 181 |
| CSS attribute references (`attr()` function) | 27.2% | 174 |
| CSS math functions (`round()`, `sin()`, `pow()`, `abs()`, etc.) | 27.0% | 173 |
| CSS color spaces and functions (`color()`, `lab()`, gradients, etc.) | 24.8% | 159 |
| CSS `:nth-child()` pseudo-class with selector-list argument | 23.0% | 147 |
| CSS `backdrop-filter` property | 21.1% | 135 |
| CSS images (`border-image`, `image()`, `image-set()`) | 19.8% | 127 |
| CSS containment (`contain`, `contain-intrinsic-size`, `content-visibility`) | 19.4% | 124 |
| CSS `:blank` and `:empty` pseudo-classes | 19.2% | 123 |
| CSS scoping (`@scope` at-rule) | 16.4% | 105 |
| CSS `mask` property (`mask-image`, `mask-mode`, etc.) | 15.8% | 101 |
| CSS `outline` property (including `outline-color`) | 14.5% | 93 |
| CSS `:user-invalid` and `:user-valid` pseudo-classes | 10.9% | 70 |
| Custom Paint API (Paint Worklet) | 10.9% | 70 |
| CSS Typed Object Model (`computedStyleMap()` API) | 9.4% | 60 |
| CSS color font feature detection and palettes | 8.9% | 57 |
| CSS motion path (`offset-path`, `offset-distance`, etc.) | 6.9% | 44 |
| CSS `leading-trim` property | 5.8% | 37 |
| CSS `:dir()` pseudo-class | 5.0% | 32 |

_Originally posted at https://github.com/web-platform-tests/interop/issues/245._

## Results of MDN APIs & JavaScript survey

| Value | Percent | Responses |
| -- | -- | -- |
| Web Components (custom elements, Shadow DOM, etc.) | 38.7% | 296 |
| File System (`navigator.storage.getDirectory()`) | 26.9% | 206 |
| Push notifications | 25.9% | 198 |
| URL (parsing and API) | 21.3% | 163 |
| Web Codecs (`AudioDecoder`, `VideoDecoder`, etc.) | 21.3% | 163 |
| Clipboard API (`navigator.clipboard`) | 20.9% | 160 |
| Navigation API (`window.navigation`) | 18.2% | 139 |
| Temporal API | 18.2% | 139 |
| Editing (`contenteditable`) | 17.9% | 137 |
| History API (`window.history`) | 16.3% | 125 |
| Pointer Events | 15.9% | 122 |
| Intersection Observer | 15.3% | 117 |
| Canvas text rendering | 14.8% | 113 |
| Import Maps | 13.5% | 103 |
| OffscreenCanvas | 12.3% | 94 |
| WebTransport | 11.4% | 87 |
| User agent client hints (`navigator.userAgentData`) | 9.3% | 71 |
| Storage quota estimation (`navigator.storage.estimate()`) | 8.6% | 66 |
| Priority Hints (`fetchpriority` HTML attribute) | 6.3% | 48 |

_Originally posted at https://github.com/web-platform-tests/interop/issues/246._

## Analysis

A layperson look at confidence intervals / errors bars happened in [two](https://github.com/web-platform-tests/interop/issues/245#issuecomment-1311874383) and [comments](https://github.com/web-platform-tests/interop/issues/246#issuecomment-1312098410), finding CIs <4%. In order to not make too much of the exact ranking when options differ by only a few percent, the ranking was instead divided into top third, middle third and bottom third. Comments were made on proposals reporting the results, usually without offering any interpretation. ([Example](https://github.com/web-platform-tests/interop/issues/158#issuecomment-1311876330)) The top choice of each survey also stood out a fair bit from the other options, so that was pointed out for [Range syntax for media/container queries](https://github.com/web-platform-tests/interop/issues/141#issuecomment-1311829551) and [Web Components](https://github.com/web-platform-tests/interop/issues/230#issuecomment-1312116874).

The interop team didn't make a joint judgement about what the results mean, but rather each participating organization could consider the results when forming their own positions for each feature.

TODO: Link to examples of the results being used in the positions process

## Future improvements

Identify best practices for how to interpret confidence intervals for this question type. Is there a best practice that's more rigorous than top/middle/bottom third?

We originally wanted to ask developers to _rank_ up to 5 options, but reverted to checkboxes after it became clear this question type doesn't work well in a narrow layout:

<img src="https://user-images.githubusercontent.com/302715/198219279-a8a05d63-50e7-44d8-932c-4a4b7253ca78.png" alt="Screenshot of the survey with a drag-and-drop interface to rank up to 5 options. It's too narrow and the options aren't readable" width="804">

If this could be resolved, this kind of survey could be more useful as a ranking question.
