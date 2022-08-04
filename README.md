# DuckDuckGo Tracker Blocklists

Web tracker blocklists used by DuckDuckGo apps and extensions. Blocklists are based on [Tracker Radar](https://spreadprivacy.com/duckduckgo-tracker-radar/) data and updated monthly.

## Related Resources
- Apps and extensions using blocklists:
  - [iOS app](https://github.com/duckduckgo/iOS) - uses web/apple-tds.json
  - [Android app](https://github.com/duckduckgo/Android) - uses web/tds.json
  - [WebExtension](https://github.com/duckduckgo/duckduckgo-privacy-extension) (for Chrome, Firefox, Edge, and Opera) - uses web/tds.json
  - [Safari extension](https://github.com/duckduckgo/privacy-essentials-safari) - uses web/tds.json
  - Mac app (in beta, code not yet open source) - uses web/apple-tds.json
- [Privacy Configuration](https://github.com/duckduckgo/privacy-configuration) - configuration of privacy features for our apps and extensions
- [Web Tracking Protections](https://help.duckduckgo.com/duckduckgo-help-pages/privacy/web-tracking-protections/) - overview of how each of our web tracking protections works, how they work across supported platforms, and how they provide overlapping protection
- [Tracker Radar](https://github.com/duckduckgo/tracker-radar) - data set of top third-party web domains with rich metadata about them
- [Tracker Radar Detector](https://github.com/duckduckgo/tracker-radar-detector) - code used to build Tracker Radar dataset from crawl data
- [Tracker Radar Collector](https://github.com/duckduckgo/tracker-radar-collector) - code used to crawl the web and identify trackers

## Licensing
Copyright 2022 Duck Duck Go, Inc.

DuckDuckGo Tracker Blocklists are licensed under the [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/). If you'd like to license the list for commercial use, [please reach out](https://help.duckduckgo.com/duckduckgo-help-pages/company/contact-us/).

## Questions

- **How can I contribute to this repository?** The blocklists in this repository are not intended to be manually modified, and as such we are not accepting external pull requests at this time. If you suspect any website usability issues or breakage, or have concerns about what is/isn't blocked, please open an issue in the [Privacy Configuration](https://github.com/duckduckgo/privacy-configuration) repository.

- **Where can I find the code that generates the blocklists?** The code to generate blocklists from the [Tracker Radar data set](https://github.com/duckduckgo/tracker-radar) is not yet open source, but coming soon.

- **Why are there two web blocklists (`web/tds.json` and `web/apple-tds.json`)?** Due to performance limitations, our iOS and Mac apps are currently using a modified version of the blocklist (`web/apple-tds.json`) that contains a subset of the main blocklist’s CNAME entries (`web/tds.json`). This only affects [CNAME Cloaking Protection](https://help.duckduckgo.com/duckduckgo-help-pages/privacy/web-tracking-protections/#cname-cloaking-protection), and we are working on resolving that limitation.