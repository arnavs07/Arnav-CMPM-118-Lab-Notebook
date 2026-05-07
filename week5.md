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

We also had another reading this week about CHERI (Capability Hardware Enhanced RISC Instructions). That reading was honestly really difficult at first because it went deep into processor architecture, memory protection, and operating system security. After taking notes and rereading sections though, I understood the main purpose better. CHERI basically extends normal pointers by adding metadata like permissions, bounds, and validity tags so hardware can enforce stronger memory safety protections.

One thing I found really interesting was how CHERI tries to improve security for languages like C and C++, which normally have a lot of memory safety vulnerabilities. The paper explained how capabilities are “unforgeable,” meaning corrupted programs cannot just randomly create valid pointers. It also talked about how CHERI works alongside existing architectures like ARM and RISC-V instead of completely replacing modern systems.

Overall, this week definitely felt like a big jump in difficulty, but it was also one of the most interesting weeks so far because it connected programming languages, operating systems, concurrency, and computer architecture all together.
