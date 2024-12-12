# Text editing Short Survey

## Date

Survey run between 2024-11-19 - 2024-11-25 to 10% of users on Web API pages. See [background discussion](https://github.com/web-platform-dx/developer-research/issues/34).

## Questions

1. Please share your feedback about the following features: _(each option listed with 4 choices: "Never heard of it", "Heard of it but not used it", "Used it and not satisfied", "Used it and satisfied")_
   * Custom Highlight: Format text ranges with no additional DOM node
   * EditContext: Build text editors to support advanced input methods
   * Async Clipboard: Read from and write to the system clipboard
   * Clipboard unsanitized HTML support: Read raw HTML from the clipboard
   * Clipboard custom formats support: Read and write custom data from the clipboard
   * Clipboard SVG support: Read and write SVG data from the clipboard
   * writingsuggestions HTML attribute: Toggle the browser's AI writing suggestions
   * document.caretPositionFromPoint(): Get the caret position from a point
   * document.elementFromPoint(): Get DOM elements from a point
   * Selection: Control and modify user text selections
   * selection.getComposedRanges: Get user text selections across shadow DOM
   * selectionchange event: Detect user text selection changes
   * Static range: Handle immutable text ranges effectively
   * contenteditable: HTML attribute to make text editable
   * contenteditable=plaintext-only: Edit plain text not rich text

2. Please share your feedback about the following proposals: _(each option listed with 3 choices: "Never heard of it", "Heard of it but not interested", "Heard of it and interested")_
   * CSS.highlights.highlightsFromPoint: Get custom highlights from a point
   * Support for range.getBoundingClientRect() in input and textareas
   * clipboardchange event: Detect changes to clipboard contents
   * placeElement: Allows HTML elements to be drawn on canvas

3. Are there any text or editing related features that are difficult to implement? _(free-form text)_

## Results

[Results in csv format](results.csv)

### Q1 - Existing features

| Feature | Never heard of it | Heard of it but not used it | Used it and not satisfied | Used it and satisfied | Responses |
| ------- | ----------------- | --------------------------- | ------------------------- | --------------------- | --------- |
| Custom Highlight | 33<br>(62.3%) | 14<br>(26.4%) | 3<br>(5.7%) | 3<br>(5.7%) | 53 |
| EditContext | 36<br>(72%) | 8<br>(16%) | 1<br>(2%) | 5<br>(10%) | 50 |
| Async Clipboard | 13<br>(27.1%) | 10<br>(20.8%) | 10<br>(20.8%) | 15<br>(31.3%) | 48 |
| Clipboard unsanitized HTML support | 29<br>(56.9%) | 15<br>(29.4%) | 3<br>(5.9%) | 4<br>(7.8%) | 51 |
| Clipboard custom formats support | 21<br>(42.9%) | 17<br>(34.7%) | 7<br>(14.3%) | 4<br>(8.2%) | 49 |
| Clipboard SVG support | 27<br>(55.1%) | 15<br>(30.6%) | 2<br>(4.1%) | 5<br>(10.2%) | 49 |
| writingsuggestions HTML attribute | 36<br>(76.6%) | 8<br>(17%) | 1<br>(2.1%) | 2<br>(4.3%) | 47 |
| document.caretPositionFromPoint() | 33<br>(66%) | 6<br>(12%) | 3<br>(6%) | 8<br>(16%) | 50 |
| document.elementFromPoint() | 27<br>(57.4%) | 6<br>(12.8%) | 2<br>(4.3%) | 12<br>(25.5%) | 47 |
| Selection | 9<br>(19.1%) | 14<br>(29.8%) | 7<br>(14.9%) | 17<br>(36.2%) | 47 |
| selection.getComposedRanges | 39<br>(81.3%) | 7<br>(14.6%) | 1<br>(2.1%) | 1<br>(2.1%) | 48 |
| selectionchange event | 16<br>(34.8%) | 12<br>(26.1%) | 3<br>(6.5%) | 15<br>(32.6%) | 46 |
| Static range | 34<br>(75.6%) | 6<br>(13.3%) | 0<br>(0%) | 5<br>(11.1%) | 45 |
| contenteditable | 3<br>(6.3%) | 7<br>(14.6%) | 13<br>(27.1%) | 25<br>(52.1%) | 48 |
| contenteditable=plaintext-only | 22<br>(46.8%) | 13<br>(27.7%) | 4<br>(8.5%) | 8<br>(17%) | 47 |
| Total responses |  |  |  |  | 53 |

### Q2 - Proposed features

| Feature | Never heard of it | Heard of it but not interested | Heard of it and interested | Responses |
| ------- | ----------------- | ------------------------------ | -------------------------- | --------- |
| CSS.highlights.highlightsFromPoint | 40<br>(88.9%) | 3<br>(6.7%) | 2<br>(4.4%) | 45 |
| range.getBoundingClientRect() in input and textareas | 23<br>(51.1%) | 4<br>(8.9%) | 18<br>(40%) | 45 |
| clipboardchange event | 26<br>(57.8%) | 4<br>(8.9%) | 15<br>(33.3%) | 45 |
| placeElement | 28<br>(62.2%) | 2<br>(4.4%) | 15<br>(33.3%) | 45 |
| Total responses |  |  |  | 45 |

### Q3 - Feedback about features that are difficult to implement (free-form)

The following challenges were extracted from the free-form responses:

| Challenges | Responses |
| ---------- | --------- |
| Browser compat (dealing with keyboard events, clipboard, or `contenteditable` across browsers) | 4 |
| Implementing syntax highlighting | 2 |
| Not enough file type support in clipboard API | 1 |
| Hard to implement undo/redo | 1 |
| Canvas-based text editing is very complex | 1 |
| Reading from the clipboard without user intervention | 1 |
| `contenteditable` is hard to work with | 1 |
| Mobile text selection is difficult | 1 |
| Selection preservation after DOM mutations | 1 |
| Unrelated answers | 4 |
| No issues | 2 |

## Interpretation

This interpretation is provided by Patrick Brosset and Taylore Givens, of Microsoft Edge, who initially proposed the short survey.

### Statistical significance

The survey received **62 responses**, which means that the results may not be representative of the wider developer community. However, the features and proposals listed in the survey are quite specific and targeted at a niche audience, so the responses are likely to be more representative of the developers who are either actively working on text editing features, or interested in them.

### Adoption of existing features

![Bar chart showing the list of features and for each the amount of participants who said they'd used it vs. not.](usage-existing.png)

The chart above shows the list of features and, for each, how many participants said they had used it vs. how many said they hadn't.

It shows that the vast majority of the text & editing features are not used by the participants. The exception are **Async Clipboard** and **Selection**, which are just above the 50% mark, and **contenteditable** which is used by ~80% of the participants.

### Satisfaction with existing features

![Bar chart showing the list of the features used by more than 10 participants, for each the ratio of participants that are satisfied vs. unsatisfied with the feature is shown.](satisfaction-existing.png)

The chart above only shows the features that more than 10 participants said they had used. For each of these features, the chart shows the ratio of participants that are satisfied vs. unsatisfied with the feature.

Participants are satisfied with most of the features they use (between 60% and 85%, with the variance likely not statistically significant). The only exception is **Clipboard custom formats support**, with 64% of participants being unsatisfied with it.

### Awareness of new features

![Bar chart showing the list of proposed features and for each the amount of participants who said they'd heard of it vs. not.](awareness-new.png)

The chart above shows the list of proposed features and, for each, how many participants said they had heard of it vs. how many said they hadn't.

All features have more than 50% of participants who have never heard of them, with **CSS.highlights.highlightsFromPoint** being the least known feature with almost 90% of participants who have never heard of it.

### Interest in new features

![Bar chart showing the list of the proposed features and for each the number of participants that are interested vs. not interested in the feature is shown.](interest-new.png)

The chart above shows the list of proposed features and, for each, how many participants said they were interested vs. how many said they weren't.

While there is clear interest in **range.getBoundingClientRect() in input and textareas**, **placeElement**, and **clipboardchange event**, the very few participants who have heard of **CSS.highlights.highlightsFromPoint** are not particularly interested in it.
