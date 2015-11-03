Resilience
==========

Communication methods
---------------------
- Line of sight towers
- Electric Morse code
  - Transatlantic Cable
  - Had the same paranoia (not real, staged)
  - Idealism (never have wars again)
- Arthur C. Clark (sp)
  - use sattelites orbiting at the rate earth spins
- Internet communication follows the majority of the submarine cable paths set up by telegraph cables
- Can the internet survive a nuclear attack? (probably not, but it is resilient)
- Packet switching
- Arpanet, first network communication was "lo" (after first two characters the network crashed)
- TCP/IP creation
  - avoids top-down control
- The internet is a dumb network (on purpose)
  - all packets are treated equally
- Tim Berners Lee read "Dial F For Frankenstein" by Arthur C. Clark as part of the inspiration of HTTP

HTML
----
- HTML formed from many existing behaviors (many elements were borrowed)
- 20+ elements at inception, now 121 elements, backwards compatible
- Fault tolerant
  - ignore tags you don't understand
  - display content
  - designed this way on purpose
- Responsive images
  - srcset
  - added to existing tag
  - picture and other tags ignored, src in img is still required, therefore backwards compatible

CSS
---

Very basic structure

``` css
.selector {

}
```

Preprocessors
Naming/Organizational conventions

The Robustness Principle
------------------------
"Be conservative in what you send, be liberal in what you accept"

These ideas work because CSS & HTML are declarative languages (instruction sets)

Javascript is imperative, needs careful error handling, fragile

Murphy's law. Whee!

Websites should be built to survive the instability of the web.

How to do this:
1. What's my core functionality?
  - identify the barebones thing that you want to provide
2. How do I make this functionality available through the simplest technology available?
  - for presentation, html
  - for messaging, html
  - for sending, html
  - for viewing images, html

3. What do I do to make this more: engaging, visually interesting, etc.

Space Elevator

http://www.frankchimero.com/writing/there-is-a-horse-in-the-apple-store/
