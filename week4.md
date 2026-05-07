Lab Notebook — Week 4 (Arnav Shah)
This week was all about the "boss level" Rust concepts like generics, traits, and lifetimes, plus actually putting everything together for the Chapter 12 CLI project. It finally felt like I was doing real software development instead of just memorizing syntax. Some of this stuff was honestly brutal at first (especially lifetimes) because most other languages I’ve used don't make you care about memory and references this much. After rereading the book and grinding through more Rustlings, I’m starting to get why Rust is built like this.

What I Did
- Read Chapters 10 through 14 of the Rust book.
- Finished Rustlings exercises from 14_generics all the way to 18_iterators.
- Built the Chapter 12 CLI project (a mini version of grep).
- Learned how to handle command-line arguments and read files properly.

What I Learned
- Generics and Traits: These were confusing at first, but I realized they’re just a way to make code reusable without breaking the type system.
- Iterators: These are awesome. They make loops and processing data look way cleaner than doing everything by hand.
- Lifetimes: Basically, it’s how the compiler ensures a reference doesn't stick around longer than the data it’s pointing to.
- Project Structure: I learned how to organize code across different modules and use error handling in a way that actually makes sense for a real app.

My Thoughts
The Chapter 12 CLI project was easily the best part of the week. Building a tool that searches through files like a basic grep felt like a real accomplishment compared to just solving practice puzzles. It forced me to actually use everything I’ve learned (ownership, borrowing, and error handling) all in one place.

I’ve realized that Rust makes way more sense when you’re actually building something. The CLI project made the hard concepts click because I could finally see why they matter. It’s one thing to read about generics, but it’s another thing to use them to make a search tool actually work. Overall, it was a tough week, but it feels like it’s all finally coming together.
