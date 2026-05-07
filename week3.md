Lab Notebook — Week 3 (Arnav Shah)
This week was definitely harder than the first two because we started looking at how Rust actually works under the hood. I read Chapters 4 through 9 of the Rust book, which covered ownership, borrowing, structs, enums, and error handling. Ownership was honestly super confusing at first since it’s so different from other languages I’ve used. I actually had to watch a few YouTube videos while I was reading just to wrap my head around what borrowing and references were even doing. After grinding through more Rustlings exercises (I finished up to exercise 13), it’s finally starting to click.

What I Did
- Read Chapters 4 through 9 of The Rust Programming Language.
- Completed Rustlings exercises up to 13 (mostly error handling).
- Read the "Arrakis: The Operating System is the Control Plane" paper.

What I Learned
- Ownership: Rust is very strict about which part of the code "owns" a piece of data to prevent memory leaks.
- Borrowing: You can let other parts of the code use data without giving up ownership, but there are a lot of rules to follow.
- Structs and Enums: These are basically ways to group data and create custom types.
- Arrakis: A new way to build operating systems that lets apps talk to hardware directly to save time.

My Thoughts
The Arrakis paper was probably the toughest thing I worked on this week. At first, I barely understood what was going on because of all the intense networking and OS terms. But after rereading it and taking a bunch of notes, the main idea made more sense.

Basically, regular operating systems like Linux create a lot of "overhead" because apps always have to ask the kernel for permission to use the network or storage. Arrakis tries to fix this by letting apps access virtualized hardware directly while the kernel just watches from the background to keep things secure.

It’s crazy to think that modern hardware is so fast that the operating system itself is actually the part slowing things down. Arrakis fixes this by splitting the OS into a "control plane" and a "data plane" so the kernel doesn't have to get involved in every single tiny task. The results they showed were pretty cool too. Apps like Redis ran way faster with much lower latency compared to Linux. The only real downside is that current hardware doesn't totally support everything Arrakis needs yet, so they have to fake some parts with software.
