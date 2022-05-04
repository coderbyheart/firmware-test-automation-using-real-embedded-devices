# Abstract: Firmware test automation using real embedded devices

In this talk I am going to present my approach on testing embedded firmware that using real hardware, because testing firmware in emulators drastically limits what actually gets tested and it can quickly become very tedious to mock, fake and set up environments for embedded firmware that needs to connect to cloud services. The approach I am showing is going a different route: let the firmware run on real hardware, and test its behavior. I will show how I implemented these tests using Zephyr, and AWS but this solution can be applied in any environment which cannot be run inside a test runner.

Here is how it looks like: https://twitter.com/coderbyheart/status/1321394949007560704

Key takeaways:
- Learn how to use GitHub Action Hosted Runners to execute firmware builds on real target
- Have an idea which building blocks are needed to run tests
- Know which essentials to focus on: firmware-over-the-air updates
