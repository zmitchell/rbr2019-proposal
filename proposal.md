# Preface
The following sections are taken straight from the proposal submission form, so ideally you would be able to copy and paste the text from each section into the submission form.

# Talk Information
**Note: Avoid personally identifying information in this section to avoid bias from reviewers. This is a request specifically from RBR!**

## Title
Test Smarter, Not Harder - Alternative Testing Methodologies

## Abstract
You've just written some tests. You think you've done a good job handling anything a user could throw at you, but your hubris will be your downfall. The Eldritch horrors of a mangled Unicode string have corrupted your Doggie Daycare Locator app, and now Amazon is informing customers that the us-east-1 datacenter has been swallowed by a portal to the abyssal plane.

This doesn't have to be you. It's hard to beat the simplicity of a basic unit test, but two alternative testing methodologies, metamorphic testing (MT) and property based testing (PBT), can provide significantly better coverage with fewer tests. In this talk I'll show you how you can use MT as a force multiplier, turning a few operations into hundreds of individual test cases without needing to know the correct outputs ahead of time, and how PBT can put your code through the wringer with randomly generated inputs. Researchers have used MT to find bugs in the Spotify and YouTube APIs, and although I'm also a (physics) researcher and I've used PBT to verify the correctness of physics simulations, you don't need to have a PhD in order to benefit from more efficient testing techniques.

## Notes for reviewers (additional info about what you might cover)
I've written a metamorphic testing framework called Monarch (https://github.com/zmitchell/monarch). I plan to use it to find bugs in public APIs so that I can show some real-world examples of using MT.

## Who's your ideal audience?
Everyone! You all write tests, right? RIGHT? You're also the ideal attendee if you're exceedingly lazy.
Why write multiple tests for different inputs to the same function, or even choose the inputs in the first place?
Let a computer do that for you!

## Why are you excited to talk about this?
The confidence that my code does what I think it does is intoxicating. It's a breath of fresh air.
It's plugging in a USB cable correctly on the first try. What if I told you that you could get that confidence and use your time more efficiently? Wouldn't you be excited? There's your answer! I'm excited to talk about this because I just want to help you out!

# Balancing Information

## What is your previous speaking experience?
I've given two talks at my local Rust meetup (Indy.rs), and a lightning talk at PyOhio.
The first talk was about cache-friendly Rust, and was essentially a summary of a conference talk I had watched on YouTube. If my memory serves this was the first actual talk at the meetup. Then came the lightning talk at PyOhio, which included an ASCII-art Clippy for good measure. The second talk at Indy.rs was a small case study of scientific computing in Rust in which I discussed my experience writing a CLI application to do some physics simulations for my PhD.

## Have you presented on this topic at other events? If so, where and when?
Not this topic specifically. There was a slide or two related to property based testing in one of the talks I gave at my local meetup, but not an entire talk dedicated to this subject.

## Are you from the Rust Belt?
Not originally, but I've been at Purdue for graduate school for several years (please don't make me count).
