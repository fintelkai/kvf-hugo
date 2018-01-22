---
date: 2014-11-12T19:00:00Z
tags:
- semantics
title: MUST and SHOULD figured out
url: /must-and-should-figured-out/
---

Those of us trying to figure out the meaning of deontic modals, especially the distinction between weak and strong necessity, should just pack in and go on vacation. There's an official RFC[^rfc] that settles the issue.

[Scott Bradner](http://www.sobco.com/sob/sob.html), all around internet wizard at Harvard, wrote [RFC 2119 "Key words for use in RFCs to Indicate Requirement Levels"](http://www.ietf.org/rfc/rfc2119.txt) in 1997. It has this definitive pronouncement on the difference between strong and weak necessity expressions:

* MUST: This word, or the terms "REQUIRED" or "SHALL", mean that the definition is an absolute requirement of the specification.
* SHOULD: This word, or the adjective "RECOMMENDED", mean that there may exist valid reasons in particular circumstances to ignore a particular item, but the full implications must be understood and carefully weighed before choosing a different course.

Exercise for the reader: do any current semantic proposals mesh with this official pronouncement on how *must* and *should* differ?

[^rfc]: "A Request for Comments (RFC) is a publication of the Internet Engineering Task Force (IETF) and the Internet Society, the principal technical development and standards-setting bodies for the Internet." ([Wikipedia](https://en.wikipedia.org/wiki/Request_for_Comments))
