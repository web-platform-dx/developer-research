# TC39 proposals Short Survey

## Date

The survey ran between 2025-04-07 - 2025-04-15 and was shown to all users of MDN JavaScript pages.

## Questions

1. Please rank these proposals in order of preference for inclusion in JavaScript:
   
   _Respondents were asked to drag and drop the following proposals into a ranked list. Not all proposals had to be ranked and respondents could rank as few or as many proposals as they wanted._

   _Respondents were also presented with a link to [a document which described the proposals](https://docs.google.com/document/d/1DMPXS4Po5Nd-l0mIEYj78H1S_R5FrB7CkHbluhqQPVo/edit)._
   
   _The proposals were presented in a random order for each respondent._

   * Decorators
   * ESM phase imports
   * Deferred module evaluation
   * JSON.parse source text access
   * Source phase imports
   * Joint iteration
   * Iterator sequence

2. Please tell us more about how your top ranking option would help you as a developer

   _Free-form text_

## Results

The survey received **2220** responses.

[Results in csv format](results.csv)

## Interpretation

The following interpretations are proposed by [Patrick Brosset](https://github.com/captainbrosset), product manager at Microsoft Edge.

### Final ranking of proposals

Here is the final ranking of the proposals:

| Proposal | Overall rank | Score | No. of rankings |
| --- | --- | --- | --- |
| Decorators | 1 | 8769 | 1736 |
| ESM phase imports | 2 | 7029 | 1675 |
| Deferred module evaluation | 3 | 6963 | 1677 |
| JSON.parse source text access | 4 | 6903 | 1646 |
| Source phase imports | 5 | 6852 | 1675 |
| Joint iteration | 6 | 5856 | 1604 |
| Iterator sequence | 7 | 5821 | 1609 |

![Chart showing the final ranking of the proposals. The order is Decorators, Iterator sequence, Joint iteration, Deferred module evaluation, JSON.parse source text access, Source phase imports, ESM phase imports.](ranked-proposals.png)

The above data shows that **Decorators** is the most highly ranked proposal.

Here is a chart comparing the scores of the proposals:

![Bar chart showing the final scores of the proposals, as seen in the table above](scores.png)

### Top ranked proposal per-respondent

The following table and chart show how many times each proposal was selected as the top ranked proposal by respondents:

| Proposal | No. of top rankings | Percentage of top rankings |
| --- | --- | --- |
| Decorators | 757 | 40% |
| ESM phase imports | 136 | 7.2% |
| Deferred module evaluation | 238 | 12.6% |
| JSON.parse source text access | 244 | 12.9% |
| Source phase imports | 130 | 6.9% |
| Joint iteration | 214 | 11.3% |
| Iterator sequence | 172 | 9.1% |

![The above table data as a pie chart, showing that Decorators was picked as the first proposal by 40% of the respondents.](top-ranked.png)

Decorators was the most popular choice, with 40% of respondents ranking it as their top choice, far ahead of the next most popular choice, JSON.parse source text access, which was ranked first by 12.6% of respondents.

### Decorators

#### Reasons for picking Decorators

Here are the main categories that emerge from the free-form responses from people who ranked Decorators as their top choice:

| Category | Number of comments |
| --- | --- |
| Cleaner, more ergonomic, shorter code (less repetition, better abstraction, more expressive, easier to read, more maintainable, less boilerplate) | 86 |
| Generally useful (either using it already, or would use it but have been waiting for it for years) | 65 |
| Parity with other languages and frameworks (Java, C#, PHP, Rust, Python, Dart, Nest.js, Django) | 32 |
| Parity with Typescript and/or Angular (waiting for the non-standard TS implementation to be standardized) | 24 |
| Useful for web components, custom elements, parity with Lit | 15 |
| Better performance, less dependencies, no need for a build step if implemented natively | 11 |
| Use case: Logging | 11 |
| Useful for libraries | 7 |
| Useful but not essential | 6 |
| Use case: Dependency injection | 6 |
| Use case: Memoization | 6 |
| Use case: Debugging | 4 |
| Use case: Input and data validation | 4 |
| Use case: ORM | 3 |
| Use case: Authentication, authorization, and other middlewares | 2 |
| Use case: Measure function execution time | 2 |
| Use case: Serialization | 2 |
| Use case: Function result caching | 1 |
| Use case: Testing | 1 |
| Use case: Clean-up after function execution (close files, database connections, etc.) | 1 |

The vast majority of people who picked Decorators as their top choice did so because they find it useful for writing cleaner, more ergonomic, and shorter code. Many also mentioned that they have been waiting for the feature for a long time in JavaScript, and that they have been using it in other languages already.

#### Overall sentiment about Decorators

Here are the sentiments which emerge from free-form responses that mention Decorators, irrespective of the respondent's top choice:

| Sentiment | Number of comments |
| --- | --- |
| Positive | 145 |
| Neutral | 71 |
| Negative | 38 |

### ESM phase imports

#### Reasons for picking ESM phase imports

Here are the main categories that emerge from the free-form responses from people who ranked ESM phase imports as their top choice:

| Category | Number of comments |
| --- | --- |
| Developer ergonomics | 8 |
| Helping with build tools and bundles | 7 |
| Better performance | 6 |
| Standardization of inconsistent implementations | 2 |

The main reason people picked ESM phase imports as their top choice is that they find it improves developer ergonomics, helps avoid bundler issues, and improves performance.

#### Overall sentiment about ESM phase imports

Here are the sentiments which emerge from free-form responses that mention ESM phase imports, irrespective of the respondent's top choice:

| Sentiment | Number of comments |
| --- | --- |
| Positive | 8 |
| Neutral | 5 |
| Negative | 1 |

### Deferred module evaluation

#### Reasons for picking Deferred module evaluation

Here are the main categories that emerge from the free-form responses from people who ranked Deferred module evaluation as their top choice:

| Category | Number of comments |
| --- | --- |
| Better performance | 47 |
| Better architecture | 4 |
| Simpler architecture and code | 3 |
| Avoid circular dependencies | 1 |

The main reason people picked Deferred module evaluation as their top choice is that it improves performance.

#### Overall sentiment about Deferred module evaluation

Here are the sentiments which emerge from free-form responses that mention Deferred module evaluation, irrespective of the respondent's top choice:

| Sentiment | Number of comments |
| --- | --- |
| Positive | 15 |
| Neutral | 14 |
| Negative | 4 |

### JSON.parse source text access

#### Reasons for picking JSON.parse source text access

Here are the main categories that emerge from the free-form responses from people who ranked JSON.parse source text access as their top choice:

| Category | Number of comments |
| --- | --- |
| To transport certain data types (floats, dates, bigints) from the server to the client with simpler code nicer | 30 |
| To remove the need for complex custom code or libraries | 12 |
| To more easily debug parsing issues | 6 |
| To make libraries more robust | 2 |
| For faster and more secure JSON handling code | 2 |

The main reason people picked JSON.parse source text access as their top choice is to unlock important data type transport from the server, and simplifying their code and making it more robust at the same time.

#### Overall sentiment about JSON.parse source text access

Here are the sentiments which emerge from free-form responses that mention JSON.parse source text access, irrespective of the respondent's top choice:

| Sentiment | Number of comments |
| --- | --- |
| Positive | 23 |
| Neutral | 5 |
| Negative | 2 |

### Source phase imports

#### Reasons for picking Source phase imports

Here are the main categories that emerge from the free-form responses from people who ranked Source phase imports as their top choice:

| Category | Number of comments |
| --- | --- |
| To simplify the integration/import of wasm and workers, and make it easier to work with bundlers (or remove the need for them) | 25 |
| Because I depend on wasm in my work and want it to be as nice to work with as possible | 17 |
| To improve performance | 2 |

The main reason people picked Source phase imports as their top choice is because of how it makes working with WASM easier and more ergonomic.

#### Overall sentiment about Source phase imports

Here are the sentiments which emerge from free-form responses that mention Source phase imports, irrespective of the respondent's top choice:

| Sentiment | Number of comments |
| --- | --- |
| Positive | 14 |
| Neutral | 5 |
| Negative | 2 |

### Joint iteration

#### Reasons for picking Joint iteration

Here are the main categories that emerge from the free-form responses from people who ranked Joint iteration as their top choice:

| Category | Number of comments |
| --- | --- |
| Reduces the need for custom code, workarounds, or libraries, leading to cleaner code | 37 |
| Unlocks unique use cases (working with data, collections, sets, maps, arrays, streams, etc) | 14 |
| Provides parity with a known paradigm/other languages | 12 |
| Improves performance | 6 |
| Is easier for new developers | 1 |

The main reason people picked Joint iteration as their top choice is that it greatly reduces the need for custom code or libraries for handling unique use cases that, otherwise, require more complex code.

#### Overall sentiment about Joint iteration

Here are the sentiments which emerge from free-form responses that mention Joint iteration, irrespective of the respondent's top choice:

| Sentiment | Number of comments |
| --- | --- |
| Positive | 30 |
| Neutral | 2 |
| Negative | 0 |

### Iterator sequence

#### Reasons for picking Iterator sequence

Here are the main categories that emerge from the free-form responses from people who ranked Iterator sequence as their top choice:

| Category | Number of comments |
| --- | --- |
| More convenient, simple, efficient, and flexible code | 18 |
| Removes the need for custom or library code | 7 |
| Provides parity with other languages | 7 |
| Better performance | 6 |

The people who picked Iterator sequence as their top choice did so mostly for convenience reasons.

#### Overall sentiment about Iterator sequence

Here are the sentiments which emerge from free-form responses that mention Iterator sequence, irrespective of the respondent's top choice:

| Sentiment | Number of comments |
| --- | --- |
| Positive | 9 |
| Neutral | 1 |
| Negative | 0 |
