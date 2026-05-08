This week was a deep dive into some of the more advanced Rust stuff, specifically smart pointers, concurrency, and async programming. It definitely felt a lot more "low-level" and closer to how systems actually work compared to the beginner stuff from the first few weeks.

What I Did
- Finished Chapters 15–17 of the Rust book.
- Rustlings exercises 19 and 20.
- Learned about smart pointers like Box, Rc, and RefCell.
- Read up on concurrency (threads and message passing).
- Started touching up on async programming, futures, and async/await.
- Read the CHERI systems security paper.

What I Learned
- Smart Pointers: These aren't just regular references since they can actually own data and do extra things behind the scenes. Very similar to the 'pointers' mentioned in the CHERRI article but not quite.
- Concurrency: Rust uses its ownership rules and even type checking to stop threading issues before running the code
- Threads: These are tools to help a program do multiple things at once without crashing everything.
- Async: This is mostly for slow things like waiting for a website to respond or a file to load so basically the whole program doesn't just freeze.
- CHERI: A way to use hardware to force memory safety and security, and it utilizes secure pointers which have different "capabilities"

The chapter on smart pointers was probably the hardest part for me. There were a ton of new ideas at once, and trying to wrap my head around reference counting (Rc) and interior mutability (RefCell) took a minute. It’s starting to click how Rust manages memory safety even when things get complicated. The concurrency part was cool too, mostly because it’s awesome that the compiler can catch threading mistakes that would normally be really difficult to find until later. 

Async programming is still pretty confusing, honestly. I don’t think I fully get "futures" or "runtimes" yet. The main takeaway for me was that async lets the program swap between tasks while waiting for slow things to finish. The explanation of concurrency vs. parallelism helped clear some things up

The CHERI Paper
We also had a reading about CHERI (Capability Hardware Enhanced RISC Instructions). I focused on Sections 1 through 5 and just skimmed Section 8. It was really interesting at first because it goes super deep into CPU architecture and OS stuff I’ve never seen, and I found how you can make these pointers a lot more secure compared to how they initially are which can cause memory corruption.

From what I got out of it, CHERI is all about making C and C++ safer. Normally, pointers are just memory addresses, but CHERI adds these capabilities which is basically extra info like permissions and bounds.

It’s pretty smart how CHERI works with existing stuff like ARM or RISC-V. It uses compartmentalization to keep different parts of a system isolated, so if one part gets hacked the rest of the system can stay safe. It reminded me a lot of Rust, honestly. Both are trying to solve memory safety, but Rust does it through the compiler and CHERI through hardware.

Major Contributions 

One of the biggest contributions of CHERI is that it improves memory safety by adding these capabilities to somewhat support hardware to normal pointers. Instead of pointers only storing memory addresses, they also store permissions, bound, and validity. This helps prevent memory corruption which is caused by languages like C and C++.
- One major strength of CHERI is that it provides strong hardware-level security protections 
- One weakness is that the system becomes very weird and could need some hardware changes

How much performance overhead would capability systems add in real-world applications?

Section 8 was a bit much to understand, but how are async and threads different/when do you use them?
