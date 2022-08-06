# Bigger testing Frameworks

## Cypress

![](Cypress.png)

**Web Page:** https://www.cypress.io/

**What is Cypress:**

Cypress is a next generation front end testing tool built for the modern web.

**It's possible to:**

Set up tests

Write tests

Run tests

Debug Tests

Cypress is most often compared to Selenium; however Cypress is both fundamentally and architecturally different. Cypress is not constrained by the same restrictions as Selenium.
This enables you to write faster, easier and more reliable tests.

**Users:** QA engineers building web applications using modern JavaScript frameworks.

**Coverage:** Cypress enables you to write all types of tests:

End-to-end tests

Integration tests

Unit tests

Cypress can test anything that runs in a browser.

**Ecosystem:**

Cypress consists of a free, open source, locally installed application and a Dashboard Service for recording your tests.

First: Cypress helps you set up and start writing tests every day while you build your application locally. TDD at its best!
Later: After building up a suite of tests and integrating Cypress with your CI Provider, our Dashboard Service can record your test runs.

**Features:**

Cypress comes fully baked, batteries included. Here is a list of things it can do that no other testing framework can:

Time Travel: Cypress takes snapshots as your tests run. Hover over commands in the Command Log to see exactly what happened at each step.

Debuggability: Stop guessing why your tests are failing. Debug directly from familiar tools like Developer Tools. Our readable errors and stack traces make debugging lightning fast.

Automatic Waiting: Never add waits or sleeps to your tests. Cypress automatically waits for commands and assertions before moving on. No more async hell.

Spies, Stubs, and Clocks: Verify and control the behavior of functions, server responses, or timers. The same functionality you love from unit testing is right at your fingertips.

Network Traffic Control: Easily control, stub, and test edge cases without involving your server. You can stub network traffic however you like.

Consistent Results: Our architecture doesn’t use Selenium or WebDriver. Say hello to fast, consistent and reliable tests that are flake-free.

Screenshots and Videos: View screenshots taken automatically on failure, or videos of your entire test suite when run from the CLI.

Cross browser Testing: Run tests within Firefox and Chrome-family browsers (including Edge and Electron) locally and optimally in a Continuous Integration pipeline.

## Puppeteer

![](Puppeteer.png)

**Web Page:** https://pptr.dev/

**What is Puppeteer:**

Puppeteer is a Node library which provides a high-level API to control Chrome or Chromium over the DevTools Protocol. Puppeteer runs headless by default, but can be configured to run full (non-headless) Chrome or Chromium.

**What can it do?:**

Most things that you can do manually in the browser can be done using Puppeteer! Here are a few examples to get you started:

Generate screenshots and PDFs of pages.

Crawl a SPA (Single-Page Application) and generate pre-rendered content (i.e. "SSR" (Server-Side Rendering)).

Automate form submission, UI testing, keyboard input, etc.

Create an up-to-date, automated testing environment. Run your tests directly in the latest version of Chrome using the latest JavaScript and browser features.

Capture a timeline trace of your site to help diagnose performance issues.

Test Chrome Extensions.

**Difference with Selenium:**

Selenium/WebDriver focuses on cross-browser automation; its value proposition is a single standard API that works across all major browsers.

Puppeteer focuses on Chromium; its value proposition is richer functionality and higher reliability.

That said, you can use Puppeteer to run tests against Chromium, e.g. using the community-driven jest-puppeteer. While this probably shouldn’t be your only testing solution, it does have a few good points compared to WebDriver:

Puppeteer requires zero setup and comes bundled with the Chromium version it works best with, making it very easy to start with. At the end of the day, it’s better to have a few tests running chromium-only, than no tests at all.

Puppeteer has event-driven architecture, which removes a lot of potential flakiness. There’s no need for evil “sleep(1000)” calls in puppeteer scripts.
Puppeteer runs headless by default, which makes it fast to run. Puppeteer v1.5.0 also exposes browser contexts, making it possible to efficiently parallelize test execution.

Puppeteer shines when it comes to debugging: flip the “headless” bit to false, add “slowMo”, and you’ll see what the browser is doing. You can even open Chrome DevTools to inspect the test environment.

## Selenium

![](Selenium.png)

**Web Page:** https://www.selenium.dev/

**What is Selenium:**

Selenium is an umbrella project for a range of tools and libraries that enable and support the automation of web browsers.

It provides extensions to emulate user interaction with browsers, a distribution server for scaling browser allocation, and the infrastructure for implementations of the W3C WebDriver specification that lets you write interchangeable code for all major web browsers.

At the core of Selenium is WebDriver, an interface to write instruction sets that can be run interchangeably in many browsers. Once you’ve installed everything, only a few lines of code get you inside a browser.

**Web Driver:**

WebDriver drives a browser natively, as a user would, either locally or on a remote machine using the Selenium server, marks a leap forward in terms of browser automation.

Selenium WebDriver refers to both the language bindings and the implementations of the individual browser controlling code. This is commonly referred to as just WebDriver.

Selenium WebDriver is a W3C Recommendation

WebDriver is designed as a simple and more concise programming interface.

WebDriver is a compact object-oriented API.

It drives the browser effectively.

**What can it do?**

Selenium supports automation of all the major browsers in the market through the use of WebDriver. WebDriver is an API and protocol that defines a language-neutral interface for controlling the behaviour of web browsers. Each browser is backed by a specific WebDriver implementation, called a driver. The driver is the component responsible for delegating down to the browser, and handles communication to and from Selenium and the browser.

This separation is part of a conscious effort to have browser vendors take responsibility for the implementation for their browsers. Selenium makes use of these third party drivers where possible, but also provides its own drivers maintained by the project for the cases when this is not a reality.

The Selenium framework ties all of these pieces together through a user-facing interface that enables the different browser backends to be used transparently, enabling cross-browser and cross-platform automation.

Selenium setup is quite different from the setup of other commercial tools. Before you can start writing Selenium code, you have to install the language bindings libraries for your language of choice, the browser you want to use, and the driver for that browser.

# Other Node js testing tools

## Cucumber

![](Cucumber.png)

**Web Page:** https://cucumber.io/

**What is Cucumber:**

Cucumber is a tool for running automated tests written in plain language. Because they're written in plain language, they can be read by anyone on your team. Because they can be read by anyone, you can use them to help improve communication, collaboration and trust on your team.

This is the JavaScript implementation of Cucumber. It runs on maintained versions of Node.js. You can quickly try it via CodeSandbox, or read on to get started locally in a couple of minutes.

**Great for BDD and live documentation.**

## Jasmine

![](Jasmine.png)

**Web Page:** https://jasmine.github.io/

**What is Jasmine?**

Jasmine is a behavior-driven development framework for testing JavaScript code. It does not depend on any other JavaScript frameworks. It does not require a DOM. And it has a clean, obvious syntax so that you can easily write tests.

Run your browser tests and Node.js tests with the same framework.

**Supported environments**

Jasmine tests itself across popular browsers (Safari, Chrome, Firefox, and Microsoft Edge) as well as Node.

Environment Supported versions
Node

Safari

Chrome

Firefox

Edge

## Jest

![](Jest.png)

**Web Page:** https://jestjs.io/

**What is Jest?**

Jest is a delightful JavaScript Testing Framework with a focus on simplicity.

It works with projects using: Babel, TypeScript, Node, React, Angular, Vue and more!

**What can it do?**

zero config

Jest aims to work out of the box, config free, on most JavaScript projects.

snapshots

Make tests which keep track of large objects with ease. Snapshots live either alongside your tests, or embedded inline.

isolated

Tests are parallelized by running them in their own processes to maximize performance.

great api

From it to expect - Jest has the entire toolkit in one place. Well documented, well maintained, well good.

## Mocha

![](Mocha.png)

**Web Page:** https://mochajs.org/

**What is Mocha?**

Mocha is a feature-rich JavaScript test framework running on Node.js and in the browser, making asynchronous testing simple and fun. Mocha tests run serially, allowing for flexible and accurate reporting, while mapping uncaught exceptions to the correct test cases. Hosted on GitHub.

**What can it do?**

browser support

simple async support, including promises

run Node.js tests in parallel

test coverage reporting

string diff support

JavaScript API for running tests

auto-detects and disables coloring for non-TTYs

async test timeout support

test retry support

test-specific timeouts

reports test durations

highlights slow tests

file watcher support

global variable leak detection

optionally run tests that match a regexp

auto-exit to prevent “hanging” with an active loop

easily meta-generate suites & test-cases

config file support

node debugger support

node native ES modules support

source-map support

detects multiple calls to done()

use any assertion library you want

extensible reporting, bundled with 9+ reporters

extensible test DSLs or “interfaces”

before, after, before each, after each hooks

arbitrary transpiler support (coffee-script etc)

TextMate bundle

## Protractor

![](Protractor.png)

**Web Page:** https://www.protractortest.org/

**What is Protractor?**

Protractor is an end-to-end test framework for Angular and AngularJS applications. Protractor is a Node.js program built on top of WebDriverJS. Protractor runs tests against your application running in a real browser, interacting with it as a user would.

**What can it do?**

Test Like a User

Protractor is built on top of WebDriverJS, which uses native events and browser-specific drivers to interact with your application as a user would.

For Angular Apps

Protractor supports Angular-specific locator strategies, which allows you to test Angular-specific elements without any setup effort on your part.

Automatic Waiting

You no longer need to add waits and sleeps to your test. Protractor can automatically execute the next step in your test the moment the webpage finishes pending tasks, so you don’t have to worry about waiting for your test and webpage to sync.
