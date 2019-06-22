# Preface
The following sections are taken straight from the proposal submission form, so ideally you would be able to copy and paste the text from each section into the submission form.

# Talk Information
**Note: Avoid personally identifying information in this section to avoid bias from reviewers. This is a request specifically from RBR!**

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
The confidence that my code does what I think it does is intoxicating. It's a breath of fresh air.
It's plugging in a USB cable correctly on the first try. What if I told you that you could get that confidence and use your time more efficiently? Wouldn't you be excited? There's your answer! I'm excited to talk about this because I just want to help you out!

# Balancing Information

## What is your previous speaking experience?
I've given two talks at my local Rust meetup (Indy.rs), and a lightning talk at PyOhio.
The first talk was about cache-friendly Rust, and was essentially a summary of a conference talk I watched on YouTube. If my memory serves this was the first actual talk at the meetup. Then came the lightning talk at PyOhio, which included an ASCII-art Clippy for good measure. The second talk at Indy.rs was a small case study of scientific computing in Rust in which I discussed my experience writing a CLI application to do some physics simulations for my PhD.

## Have you presented on this topic at other events? If so, where and when?
Not this topic specifically. There was a slide or two related to property based testing in one of the talks I gave at my local meetup, but not an entire talk dedicated to this subject.

## Are you from the Rust Belt?
Not originally, but I've been at Purdue for graduate school for several years (please don't make me count).
