# Preface
The following sections are taken straight from the proposal submission form, so ideally you would be able to copy and paste the text from each section into the submission form.

# Talk Information
**Note: Avoid personally identifying information in this section to avoid bias from reviewers. This is a request specifically from RBR! The exact wording:**
- **Please help us avoid unconscious/unintentional bias by not including personally identifying information in this section, including gendered pronouns, websites, or company names.**

## Title
Test Smarter, Not Harder - Metamorphic and Property-Based Testing in Rust

## Abstract
You've just written some tests. You think you've done a good job handling anything a user could throw at you, but hubris will be your downfall. The Eldritch horrors of a mangled Unicode string have corrupted your Doggie Daycare Locator app, and now Amazon is informing customers that the us-east-1 datacenter has been swallowed by a portal to the abyssal plain.

This doesn't have to be you. It's hard to beat the simplicity of a basic unit test, but two alternative testing methodologies, metamorphic testing and property-based testing, can provide significantly better coverage with fewer tests. In this talk, I'll show you how you can use property-based testing with the proptest crate, putting your code through the wringer with randomly generated inputs. Then I'll show you how you can use metamorphic testing as a force multiplier with the Monarch crate, turning a few operations into hundreds of individual test cases. Researchers have used metamorphic testing to find bugs in the Spotify and YouTube APIs, and although I'm also a researcher and I've used property-based testing to verify the correctness of physics simulations, you don't need to have a PhD to use and benefit from more efficient testing techniques.

## Notes for reviewers (additional info about what you might cover)
I've written a metamorphic testing framework for Rust, but it's very barebones as of today. Between now and the talk I plan to implement the most basic remaining features and use it to test public APIs until I find a bug that I can use as an example in the talk. I'll also show examples of how I used property-based testing with the proptest crate to verify the correctness of a simulation tool I wrote. Both of these techniques revolve around testing abstract properties of your programs, so I plan to provide examples of a variety of these properties so that new users can get a feel for what to look for.

## Who's your ideal audience?
My ideal audience is everyone because everyone can stand to write better tests. Tests are an important part of software development, regardless of industry or skill level. On the Rust homepage Rust is described as "A language empowering everyone
to build reliable and efficient software." Better test coverage can locate more bugs, making your software more reliable, and writing fewer tests makes YOU more efficient. Less experienced programmers will appreciate that these techniques can reveal unexpected edge cases and learn to handle them accordingly, while more experienced developers with a "code is a liabilty" mindset will appreciate that these techniques allow for a smaller test suite.

## Why are you excited to talk about this?
One of my favorite aspects of Rust is the power it gives me to write rock-solid software. Knowing that my code does what I think it does is a breath of fresh air. It's plugging in a USB cable correctly on the first try. A comprehensive test suite is another piece of that rock-solid puzzle, but writing good unit tests requires that I know the multitude of ways that something could go wrong. Not only will these techniques help me catch these bugs, but they will teach me what to look out for in the future. I'm excited to talk about this because I'm a software nerd, I love teaching people about software, and I want people to know that there are very powerful tools at their disposal that they may not be aware of.

# Balancing Information

## What is your previous speaking experience?
I've given two 30-minute talks at my local Rust meetup, and a lightning talk at PyOhio.
The first Rust talk was about writing Rust to efficiently use CPU caches. This talk was essentially a summary of a conference talk I watched on YouTube, but I found it interesting and our meetup needed a speaker. My next talk was the PyOhio lightning talk, and was about abusing type annotations to shoehorn Rust-like macros into Python. This talk was really just for fun, and included an ASCII-art Clippy for good measure. My most recent talk was my second Rust talk, and was a case study of scientific computing in Rust. In that talk I discussed my experience writing a command line program for doing a certain type of physics simulation.

## Have you presented on this topic at other events? If so, where and when?
I haven't spoken solely on this topic before, but I did briefly discuss property-based testing in my second Rust talk since I used property-based testing to validate user input and ensure that simulations were physically correct.

## Are you from the Rust Belt?
Not originally, but I've been at Purdue for graduate school for several years (please don't make me count).
