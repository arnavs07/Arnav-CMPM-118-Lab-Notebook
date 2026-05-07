This week was a deep dive into some of the more advanced Rust stuff, specifically smart pointers, concurrency, and async programming. It definitely felt a lot more "low-level" and closer to how systems actually work compared to the beginner stuff from the first few weeks.

What I Did
Finished Chapters 15–17 of the Rust book.

Knocked out Rustlings exercises 19 and 20.

Learned about smart pointers like Box, Rc, and RefCell.

Read up on concurrency (threads and message passing).

Started scratching the surface of async programming, futures, and async/await.

Read the CHERI systems security paper.

What I Learned
- Smart Pointers: These aren't just regular references; they can actually own data and do extra things behind the scenes.
- Concurrency: Rust uses its ownership rules and type checking to stop threading bugs before the code even runs.

- Threads vs. Message Passing: These are tools to help a program do multiple things at once without crashing everything.

- Async: This is mostly for slow stuff, like waiting for a website to respond or a file to load, so the whole program doesn't just freeze.

- CHERI: A way to use hardware to force memory safety and security.

The chapter on smart pointers was probably the hardest part for me. There were a ton of new ideas at once, and trying to wrap my head around reference counting (Rc) and interior mutability (RefCell) took a minute. It’s starting to click how Rust manages memory safety even when things get complicated. The concurrency part was cool too, mostly because it’s awesome that the compiler can catch threading mistakes that would normally be a nightmare to find later.

Async programming is still pretty confusing, honestly. I don’t think I fully get "futures" or "runtimes" yet. The main takeaway for me was that async lets the program swap between tasks while waiting for slow things to finish. The explanation of concurrency vs. parallelism helped clear some things up, though.

The CHERI Paper

We also had a reading about CHERI (Capability Hardware Enhanced RISC Instructions). I focused on Sections 1 through 5 and just skimmed Section 8. It was really tough at first because it goes super deep into CPU architecture and OS stuff I’ve never seen.

From what I got out of it, CHERI is all about making C and C++ safer. Normally, pointers are just memory addresses, but CHERI adds these "capabilities" which is basically extra info like permissions and bounds. This way, the hardware can stop a buffer overflow or a memory attack right in its tracks.

It’s pretty smart how CHERI works with existing stuff like ARM or RISC-V instead of trying to replace them. It uses compartmentalization to keep different parts of a system isolated, so if one part gets hacked, the rest stays safe. It reminded me a lot of Rust, honestly. Both are trying to solve memory safety, but Rust does it through the compiler while CHERI does it through the hardware.

Section 8 was a bit over my head (mostly future research stuff), but overall, it was cool to see how software and hardware can actually team up to make things more secure.
