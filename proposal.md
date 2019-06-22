# Preface
The following sections are taken straight from the proposal submission form, so ideally you would be able to copy and paste the text from each section into the submission form.

# Talk Information
**Note: Avoid personally identifying information in this section to avoid bias from reviewers. This is a request specifically from RBR!**

## Title
Test Smarter, Not Harder - Alternative Testing Methodologies

## Abstract

### High level ideas
- You can do better than "with this exact input I expect this exact output".
- Alternative methodologies
  - Property based testing (PBT)
  - Metamorphic testing
- Using proptest to put polsim through the wringer
- Monarch (metamorphic testing utility I haven't written yet)
- Something else to tie it all together

### Pain point
- You've written a test, but aren't sure whether you've considered all the edge cases.
- You have considered a bunch of edge cases, but to address them you've had to either write one big test or duplicate your test code for each case.

### Solution
- Use a testing methodology that's a force multiplier.
- A property test will randomly generate inputs to explore your code in ways you wouldn't have thought to.
- Metamorphic testing lets you explore your code without needing to find general properties.

### Supporting points
- Researchers (see [this paper (PDF)](http://www.lsi.us.es/~segura/files/papers/segura17-tse.pdf)) used metamorphic testing to find 3 bugs in the Spotify API, and 8 bugs in the YouTube API.
- I've written dozens of PBTs to verify the behavior of various scientific tools I've written.

### Personal/funny stuff
I think I want to open with something like this:
> You've just written some tests. You think you've done a good job handling anything a user could throw at you. Sweet summer child, your hubris has gotten the better of you. The Eldritch horrors of a mangled Unicode string are wreaking havoc on your `_____` as a Service app, and Amazon has just informed customers that the us-east-1 datacenter has been swallowed by a portal to the abyssal plane.

From there I would say something like "all of this could have been prevented if `_____`".

### Draft
You've just written some tests. You think you've done a good job handling anything a user could throw at you, but your hubris will be your downfall. The Eldritch horrors of a mangled Unicode string are wreaking havoc on your `_____` as a Service app, and Amazon has just informed customers that the us-east-1 datacenter has been swallowed by a portal to the abyssal plane.

This doesn't have to be you. Metamorphic testing (MT) is a force multiplier, turning a small number of operations into hundreds of individual test runs. Researchers have used this technique to find bugs in the YouTube and Spotify APIs. Property based testing (PBT) puts your code through the wringer with randomly generated inputs. I've used PBT for tasks ranging from validating user input to verifying physics simulations. In this talk I'll teach you how you can use these alternative testing methodologies to get better coverage with fewer tests.

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
