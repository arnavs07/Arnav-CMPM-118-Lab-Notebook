Lab Notebook — Week 5 (Arnav Shah)

This week focused on some of the more advanced Rust concepts, especially smart pointers, concurrency, and async programming. Compared to the earlier weeks, the material felt a lot more low-level and closer to actual systems programming.

What I Did
- Read Chapters 15 through 17 of The Rust Programming Language
- Completed Rustlings exercises 19 through 20
- Learned about smart pointers like Box<T>, Rc<T>, and RefCell<T>
- Read about concurrency with threads and message passing
- Started learning about async programming, futures, and async/await
- Read the CHERI systems security paper

What I Learned
- Smart pointers can own data and provide extra functionality beyond normal references
- Rust uses ownership and type checking to help prevent concurrency bugs
- Threads and message passing help programs run multiple tasks more safely
- Async programming is mainly useful for handling slower operations like networking or file I/O
- CHERI uses hardware-supported capabilities to improve memory safety and security

The smart pointers chapter was probably the hardest part for me because there were a lot of new concepts introduced at once. Understanding reference counting and interior mutability took some time, but I started seeing how Rust handles memory safety in more complicated situations. The concurrency chapter was also interesting because it explained how Rust tries to catch threading issues during compilation instead of letting them become runtime bugs later.

The async chapter was honestly still pretty confusing, especially futures and async runtimes, and I definitely do not fully understand everything yet. From what I understood though, async programming lets programs switch between tasks while waiting for slower operations to finish. The explanations about concurrency vs parallelism helped make the ideas a little easier to follow.

We also had another reading this week about CHERI (Capability Hardware Enhanced RISC Instructions). For this reading, I mainly focused on Sections 1 through 5 and skimmed over Section 8. The reading was honestly really difficult at first because it went deep into processor architecture, operating systems, and memory protection concepts that I had not really seen before.

From what I understood, the main purpose of CHERI is improving memory safety and security in systems that use languages like C and C++. Instead of normal pointers just storing memory addresses, CHERI capabilities also include extra metadata like permissions, bounds, and validity tags. This allows the hardware itself to enforce stronger memory protection and prevent certain types of attacks or memory corruption issues.

One thing I found interesting was how CHERI tries to work alongside existing architectures like ARM, MIPS, and RISC-V instead of completely replacing current systems. The paper explained how capabilities can help prevent vulnerabilities like invalid memory accesses and buffer overflows by limiting what pointers are allowed to access. I also thought it was interesting how the architecture focuses heavily on compartmentalization and limiting privileges between different parts of a system.

The sections about concurrency, memory safety, and hardware enforcement reminded me a lot of Rust because both CHERI and Rust are trying to solve memory safety problems, just in different ways. Rust mainly approaches the problem through the programming language and compiler, while CHERI approaches it through hardware-level protections.

I also skimmed over Section 8, which talked more about future research directions and possible future improvements for CHERI systems. Overall, this reading was definitely challenging, but it was interesting seeing how hardware and software can work together to improve security and memory safety.
