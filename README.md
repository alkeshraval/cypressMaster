## Known Issues
- require use of deprecated cedar-14 heroku stack
- Cypress does not output in [TAP format so failed tests appear green](https://devcenter.heroku.com/articles/testpack-api#output).

## Example Output
```
-----> The Xvfb Google Chrome buildpack does not run tests. Skipping.
-----> Running Node.js buildpack tests...
> cypress-heroku-ci@1.0.0 test /app
> PORT=8080 node run-cypress-tests.js
It looks like this is your first time using Cypress: 3.0.3
[?25l[20:25:40]  Verifying Cypress can run /app/.cache/Cypress/3.0.3/Cypress [started]
[20:25:43]  Verifying Cypress can run /app/.cache/Cypress/3.0.3/Cypress [completed]
[?25h
Opening Cypress...
Xlib:  extension "RANDR" missing on display ":42".
Xlib:  extension "RANDR" missing on display ":42".
====================================================================================================
  (Run Starting)
  ┌────────────────────────────────────────────────────────────────────────────────────────────────┐
  │ Cypress:    3.0.3                                                                              │
  │ Browser:    Electron 59 (headless)                                                             │
  │ Specs:      1 found (simple_spec.js)                                                           │
  └────────────────────────────────────────────────────────────────────────────────────────────────┘
────────────────────────────────────────────────────────────────────────────────────────────────────

  Running: simple_spec.js...                                                               (1 of 1)
  My First Test
starting server on port=8080
  1 passing (3s)
  (Results)
  ┌──────────────────────────────┐
  │ Tests:        1              │
  │ Passing:      1              │
  │ Failing:      0              │
  │ Pending:      0              │
  │ Skipped:      0              │
  │ Screenshots:  0              │
  │ Video:        true           │
  │ Duration:     2 seconds      │
  │ Spec Ran:     simple_spec.js │
  └──────────────────────────────┘
  (Video)
  - Started processing:   Compressing to 32 CRF
  - Finished processing:  /app/cypress/videos/simple_spec.js.mp4 (4 seconds)
====================================================================================================
  (Run Finished)
      Spec                                                Tests  Passing  Failing  Pending  Skipped
  ┌────────────────────────────────────────────────────────────────────────────────────────────────┐
  │ ✔ simple_spec.js                            00:02        1        1        -        -        - │
  └────────────────────────────────────────────────────────────────────────────────────────────────┘
    All specs passed!                           00:02        1        1        -        -        -
[?25h-----> Node.js buildpack tests completed successfully
```
