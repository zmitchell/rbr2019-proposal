# Preface
The following sections are taken straight from the proposal submission form, so ideally you would be able to copy and paste the text from each section into the submission form.

# Talk Information
**Note: Avoid personally identifying information in this section to avoid bias from reviewers. This is a request specifically from RBR! The exact wording:**
- **Please help us avoid unconscious/unintentional bias by not including personally identifying information in this section, including gendered pronouns, websites, or company names.**

## Title
Test Smarter, Not Harder - Alternative Testing Methodologies

## Abstract
You've just written some tests. You think you've done a good job handling anything a user could throw at you, but your hubris will be your downfall. The Eldritch horrors of a mangled Unicode string have corrupted your Doggie Daycare Locator app, and now Amazon is informing customers that the us-east-1 datacenter has been swallowed by a portal to the abyssal plain.

This doesn't have to be you. It's hard to beat the simplicity of a basic unit test, but two alternative testing methodologies, metamorphic testing (MT) and property based testing (PBT), can provide significantly better coverage with fewer tests. In this talk, I'll show you how you can use MT as a force multiplier, turning a few operations into hundreds of individual test cases without needing to know the correct outputs ahead of time, and how PBT can put your code through the wringer with randomly generated inputs. Researchers have used MT to find bugs in the Spotify and YouTube APIs, and although I'm also a (physics) researcher and I've used PBT to verify the correctness of physics simulations, you don't need to have a PhD to use and benefit from more efficient testing techniques.

## Notes for reviewers (additional info about what you might cover)
I've written the first metamorphic testing framework for Rust, called Monarch (https://github.com/zmitchell/monarch). It's early days for Monarch, but I plan to use it to find bugs in public APIs so that I can show some real-world examples in the talk. I'll also show examples of how I used PBT (the proptest crate) to verify the correctness of a simulation tool I wrote. I'm aware of another testing technique called mutation testing, but the two existing crates are not actively maintained, writing a new crate would be an enormous undertaking, and I don't think I could do all three techniques justice in the time provided.

## Who's your ideal audience?
I hesitate to say "everyone", but this topic should have very broad appeal. Tests are an important part of software development, regardless of industry or skill level. On the Rust homepage Rust is described as "A language empowering everyone
to build reliable and efficient software." Better test coverage makes your software more reliable, and writing fewer tests makes YOU more efficient. Less experienced programmers will appreciate that these techniques can reveal unexpected edge cases and learn to handle them accordingly, while more experienced developers with a "code is a liabilty" mindset will appreciate that these techniques allow for a smaller test suite.

## Why are you excited to talk about this?
One of my favorite aspects of Rust is the power it gives me to write rock-solid software. Knowing that my code does what I think it does is a breath of fresh air. It's plugging in a USB cable correctly on the first try. A comprehensive test suite is another piece of that rock-solid puzzle, but writing good unit tests requires that I know the multitude of ways that something could go wrong. Not only will these techniques help me catch these bugs, but they will teach me what to look out for in the future. I'm excited to talk about this because I'm a software nerd, I love teaching people about software, and I want people to know that there are very powerful tools at their disposal that they may not be aware of.

# Balancing Information

## What is your previous speaking experience?
I've given two 30-minute talks at my local Rust meetup, and a lightning talk at PyOhio.
The first Rust talk was about writing Rust to efficiently use CPU caches. This talk was essentially a summary of a conference talk I watched on YouTube, but I found it interesting and our meetup needed a speaker. My next talk was the PyOhio lightning talk, and was about abusing type annotations to shoehorn Rust-like macros into Python. This talk was really just for fun, and included an ASCII-art Clippy for good measure. My most recent talk was my second Rust talk, and was a case study of scientific computing in Rust. In that talk I discussed my experience writing a command line program for doing a certain type of physics simulation.

## Have you presented on this topic at other events? If so, where and when?
Not this topic specifically. There was a slide or two related to property based testing in one of the talks I gave at my local meetup, but not an entire talk dedicated to this subject.

## Are you from the Rust Belt?
Not originally, but I've been at Purdue for graduate school for several years (please don't make me count).
