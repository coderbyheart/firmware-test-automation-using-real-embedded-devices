# Firmware test automation using real embedded devices

![Publish](https://github.com/coderbyheart/firmware-test-automation-using-real-embedded-devices/workflows/Publish/badge.svg?branch=saga)

Slides for my talk about firmware test automation using real embedded devices

- [Markdown](./slides.md)
- [Interactive](https://coderbyheart.github.io/firmware-test-automation-using-real-embedded-devices/index.html)

## Abstract

In this talk I am going to present my approach on testing embedded firmware that
using real hardware, because testing firmware in emulators drastically limits
what actually gets tested and it can quickly become very tedious to mock, fake
and set up environments for embedded firmware that needs to connect to cloud
services. The approach I am showing is going a different route: let the firmware
run on real hardware, and test its behavior. I will show how I implemented these
tests using Zephyr, and AWS but this solution can be applied in any environment
which cannot be run inside a test runner.

Here is how it looks like:
https://twitter.com/coderbyheart/status/1321394949007560704

Key takeaways:

- Learn how to use GitHub Action Hosted Runners to execute firmware builds on
  real target
- Have an idea which building blocks are needed to run tests
- Know which essentials to focus on: firmware-over-the-air updates

## Viewing

An up-to-date version is published to
[GitHub pages](https://coderbyheart.github.io/firmware-test-automation-using-real-embedded-devices/index.html).

Press `s` to show the speaker notes.

### Locally

Open the project using
[Dev Container](https://code.visualstudio.com/docs/remote/containers).

Open two shells:

1. `npm run watch`
2. `npm start`

You can now view the slides at <http://127.0.0.1:8000>.

## Building

Render to reveal.js:

    make build

Render to PowerPoint (useful for copying to a PowerPoint template):

    make public/slides.pptx
