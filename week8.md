Lab Notebook - Week 8
Arnav Shah

This week I mainly worked on the Chapter 21 final project from the Rust Programming Language Book where we built a multithreaded web server from scratch. This project was one of the more intense ones we've done because there were so many moving parts at once. Rather than only focusing on syntax, or even one Rust feature, this project had a lot of threads, networking, ownership, HTTP requests, and even a lot of debugging. 

Unlike the filesystem lab where we had to genuinely think about the implementation, the MTWS project felt a lot more like following a walkthrough since the solution code was bsically given step by step throughout the chapter. Kinda felt like I was subconciously just copying the code rather than fully understanding what was really happening. To be honest, it kinda felt like they wanted you to solve it, but immediately gave you the answers right after without really letting you properly implement it. 

I think this became even harder because threading was already something I was very unfamiliar with. Since I don't have that much experience w/ web servers, or even multithreaded systems as a whole, I think the project just genuinely became a lot more confusing. I did begin to understand the whole idea of the project in a conceptual manner but like not fully why things were implemented the way they were. 


What I Did:
- Finished the Rust Book
- Finished the MTWS final project
- Attempted to build a TCP server
- Tried parsing HTTP requests with BufReader
- Learned to use thread::spawn() and how it can help w/ multithreading
- Worked with mpsc channels
- Learned a lot more about thread pools, and even workers
- I Learned a lot more about how jobs are sent between threads asw
- Ran and did a lot of testing with cargo run
- Also worked closely with Tcp Stream
- Overall just finished the MTWS project this week!

I think other than the negatives, the MTWS project itself was really cool because it was one of the first times I got to know how web servers work, and even how they can like process requests. Before this, I didn't really look at or even think about how multiple users can connect to a server at once, or even how these requests distribute themsleves. I just thought it happens. Thread pools were the more cooler ideas to me because it helped to show why concorruency matters. Also seeing these worker threads fix issues were really cool.

Although I did struggle with how this project was given, I still think a multithreaded web server is insanely cool. Since this was the end of the Rust Book, I was also thinking about how this book was and helped me with Rust. Personally, I did not find the book super helpful for learning a lot of the concepts. I think it was good when it came to introducing syntax and many ideeas, but a lot of the chapters felt very explanation heavy with little to no problem solving. I honestly think I did more of my learning from Youtube rather than the actual Rust Book itself. Even the quizzes were weird since they didn't give you proper reasoning as to why something was wrong, it was just overall really confusing. 

I do think finishing the Rust Book was a very important experience and it helped to expose me to many concepts I wouldn't have touched or even have thought about before. Ownership, borrowing, traits, lifetimes, etc., are all brand new topics to me that I've never seen before, but they are so interesting to me. Although I did rely on outside resources a lot, I still feel way more comfortable understanding Rust code now, than I did comapred to the beginning. 

