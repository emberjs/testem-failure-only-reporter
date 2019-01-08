testem-failure-only-reporter
---

Two `testem` reporters extracted from [`emberjs/ember.js`](https://github.com/emberjs/ember.js) for use by `emberjs` repositories. 

#### Default, failure-only test reporter.
Extends from the `testem` `tap` reporter. Only outputs results on failure. Outputs progress once every 100 tests to keep CI alive. 
```js
// testem.js
const FailureOnlyReporter = require('testem-failure-only-reporter');

//...
  reporter: FailureOnlyReporter
```

#### failure-only test reporter, grouped by browser

Extends from the above default failure-only reporter. Summarizes results by browser.

```js
const FailureOnlyReporterGroupedByBrowser = require('testem-failure-only-reporter/grouped-by-browser');
```
