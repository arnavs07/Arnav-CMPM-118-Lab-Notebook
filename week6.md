Arnav Shah Lab Notebook - Week 6

This week was more about design concepts in Rust rather than just syntax and ownership! We learned more about object-oriented programming features in Rust, more about patterns and matching, and we also started our first actual lab assignment this week! This week was more like applying rust and it actually began feeling more like real systems programming rather than just practice exercises we had been working on till now.

What I Did:
- Read Chapters 18 and 19 of the Rust Programming Language book
- Learned more about how Rust can handle OOP differently from other languages like Java or even Python
- Learned more about trait objects and dynamic dispatch which was used using Box<dyn Trait>
- Also read more about these design trade offs in Rust, especially when it came to references. 
- Learned more about pattern matching, destructuring, refutable vs. irefutable patters, and even match syntax. 
- Started the first filesystem lab assignment which had to use recursion when it came to data structures and even traits!
- Had to use BTreeMap, Box<T>, file handles, and also had to traverse through paths.

What I learned: 
- Rust is actually object-oriented in quite a few ways, but comapred to other languages in terms of inhertience, it approaches OOP very differently. Rather than classes and inheritance, Rust is mainly focused around structs, enums, traits, and even trait objects
- Trait objects were actually one of the biggest things we had covered this week. I learned more about Box<''>, e.g. Box<dyn Draw> and how this in specific can help different types to share the same behavior, all through a common trait. 
- I also had learneed the difference between generics and trait objects! Generics are better when all the values are actually the same type, while trait objects are more useful when it comes to storing different types of data together.
- Refutable vs. Irefutable patterns: It was confusing at first, but eventually I understood that some patterns can actually fail to match, while others can always succeed/succeed most of the time.

The hardest part of this week was definitely the filesystem lab. It was actually the first time we had to combine a lot of different Rust concepts together apart from the ch. 12 project we had done earlier. When using recursive path enums using the Box feature, so in this case Box<Path>, it was extremely confusing at first and honestly still is a little. But, slowly I began understanding why these recursive types do actually need heap allocation in a language like Rust. 

One thing I thought that was pretty cool was actually how realistic the lab felt. We began to use more concepts that were similar to real operating systems which was really cool to see as someone interested in that field. We had to incoroparte file descriptors, traversal, and even trees for filesystems. It made everything feel a lot more practical and really cool lol.

The pattern matching was also something I was confused with at fist, and am still a little bit confused but it is a lot better overall as it was a really important concept this week. They felt like nicer swtich statements, and I think I slowly began to realize why and how it is a huge part of how Rust can handle enums, recursion, and even the control flow of a program.

Although I said the filesystem lab was the hardest part of this week, I definitely think it was the most important! Even though it was frustrating at times, I do think that having to work through those concepts like recursion, traversal, etc., heap allocation etc., it all came together and helped me understand these individual concepts a lot better than just reading them in a book. The lab also did help me realize that Rust is a language where organization matters more over anything. Breaking these things into helper functions and much smaller problems made the assignment a lot easier. 

Initially, I would just try to solve everything and get confused with all the mumbo jumbo, but once I began slowing down, everything started making a lot more sense. Overall, I still need help with recursive enums and pattern matching because those were probably the biggest challenges for me this week. But, I do feel like this week was one of the biggest jumps so far. It actually helped me understand Rust is less about memorization, and more about ownership and structure, or in other words how data can move through a system.
