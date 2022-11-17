# Shared Research on Web Developer Experience

## Historic of Shared Research Efforts

In 2019 and 2020, Mozilla and the [MDN Product Advisory Board](https://developer.mozilla.org/en-US/docs/MDN/MDN_Product_Advisory_Board/Membership) developed and ran the [Web Developer Needs Assessment (DNA)](https://insights.developer.mozilla.org/), a large-scale study of developer needs.

One of the key themes emerging from the results was how high **fragmentation** (i.e. browser incompatibilities) was in the list of pain points that developers reported.

These surveys led to two more in-depth studies:
* the [MDN 2020 Browser Compatibility Report](https://insights.developer.mozilla.org/reports/mdn-browser-compatibility-report-2020.html)
* the [MDN 2021 Web Testing Report](https://insights.developer.mozilla.org/reports/mdn-web-testing-report-2021.html)

The former led to the [Compat 2021 effort](https://web.dev/compat2021/), a predecessor to the [Interop project](https://github.com/web-platform-tests/interop/). These efforts aim to reduce fragmentation through a shared implementation focus across browser engines.

[The Web We Want](https://webwewant.fyi/) is another collaborative effort to gather input from the developer community, through a combination of in-person prompts and on-line calls for input.

## Value of Structuring Shared Research Efforts

The experience of the shared research efforts done under the umbrella of the MDN Product Advisory Board has demonstrated some of the benefits that can be expected from a collaborative approach:
* a collaborative effort gives greater status and thus reach and acceptability to the research, which helps with recruiting participants to the effort (e.g. in the case of surveys, respondents);
* collaborating on the design and the execution of the research makes it easier for the involved parties and the broader ecosystem to trust the results of the research and thus increases its impact;
* collaboration on the design helps identify biases, gaps and bugs that may be harder to spot in a single-party effort, and allows to draws expertise and infrastructure not available to any single party.

## Shared Research Efforts Explored in 2022

As the WebDX effort was being explored, we experimented with different approaches to structure and run shared developer research.

To provide input to the prioritization of features that would benefit from such a focus, the [State of CSS 2022 survey](https://www.stateofcss.com/) organizers were contacted so that the timing and content of the survey could be adjusted to the need of Interop 2023. Among other things, the content of the survey was developed with a specific request for input to the community, using <a href="https://github.com/Devographics/surveys/issues?q=is%3Aissue+is%3Aopen+label%3A%22State+of+CSS+2022%22">GitHub issues</a>.

Another set of experiments built on the reach that MDN Web Docs has with developers. Following a framework defined by the MDN Product Advisory Board to run <a href="https://github.com/mdn/pab/issues/83">short surveys on MDN</a>, 3 experimental surveys were run on MDN in 2022:
* one in June that asked developers visiting the CSS pages on MDN their [feedback on CSS cascade layers](https://www.youtube.com/watch?v=kbYeKKLeRR0) - first and foremost as a way to test the infrastructure and the reception of these surveys by MDN visitors
* one in October focused on the browsers developers expect a feature to be supported in before they consider using it ([browser support survey details](https://github.com/web-platform-dx/developer-research/pull/11)
* one in November gathering prioritization info on [proposals submitted to Interop 2023](https://github.com/web-platform-tests/interop/issues/196) ([interop survey details](https://github.com/web-platform-dx/developer-research/pull/12))

So far, the detailed discussions on these MDN Short Surveys have happened in a private repo of the MDN GitHub organization to facilitate these early experimentations. While the use of that private repo may remain necessary moving forward for operational matters, we expect the gist of the design discussions for future surveys to happen in the [WebDX developer research repo](https://github.com/web-platform-dx/developer-research).

Beyond that, a [W3C TPAC 2022 breakout session](https://www.w3.org/2022/09/14-webdx-minutes.html) discussed what the W3C community would expect out of shared survey efforts and explored what additional sources of signals could be exploited: bug reports on browsers, telemetry, StackOverflow questions, polyfill usage.

## Shared Research Roadmap

To help the newly formed WebDX Community Group structure its efforts around shared research, Dom and Kadir have volunteered to draft what a roadmap for our efforts could be for 2023.

Such a roadmap would explore structuring our efforts around MDN Short Surveys, evaluating the need and feasibility of a bigger survey project (à la MDN DNA), and more generally, describing how the various tools and signals available can be best used and combined to deliver the impact we're after in Developer Experience improvements.
