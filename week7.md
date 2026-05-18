Lab Notebook - Week 7 Arnav Shah

This week we were given extra time to finish the filesystem lab, so what i did was I used this to finish up the second half of the assignment, and also clean up a lot of parts that were still pretty confusing to me from last week itself. I was also unfortuantely pretty sick this week and ended up missing the section, so most of my work was done independently although I understand it was important working with a peer. 

Since the lab was pretty big overall, having this extension helped a lot since it gave me more time to work through all the recursive logic and even the ownership issues rather than completely rushing through it all at once. 

What I Did:

- Finished working on and implementing the second half of the filesystem lab
- Worked on the DirectoryHandle and NodeHandle
- I tried implementing a lot more of the traversal logic for the directories and files
- Continued with the recursive enums and even the recursive helper functions
- I had implemented the Display trait so the filesystem tree would properly print out the files
- I also used BTreeMap --> it helped print everything in alphabetical order
- I created a custom FsError error handling which was used throughout the filesystem
- Used Path::from_iter and also worked w/ iterators
- Used create and create_dir for creating the files
- I also tried using traits for the find functionality
- Spent a ton of time with the debugging, especially when it came down to ownership, borrowing, etc. 

What I learned:
- I learned a ton of things about recursive data structures, and also how these filesystems work when with trees
- Path and Box<Path> finally began making more sense, especially after learning a lot more about HeapAllocation in Rust
- I also learned how traits can help with functionality rather than just repeating code
- Helper functions are sooooo important when it comes to recursive traversal. 
    - When you try putting everything into one function it just becomes terrible and confusing

The hardest part of this week was 100% debugging the recursive traversal, and even all the ownership issues. When I tried fixing one compiler error, it would honestly cause an issue elsewhere. One thing that I can safely say helped me was actually slowing down and going line by line throughout the filesystem rather than trying to code everything in one go. Once I started looking at like like it was a tree, all the logic became a lot easier to understand. 

I found it cool how realistic the lab felt. We recreated a lot of concepts that are used in those real OS like traversal, trees, handles, etc. It was honestly a super fun experience. Although this lab was really confusing and frustrating, especially while I was down with a fever, I think it was the most important assignment we've been given since it forced all knowledge to be combined into one intersting project!
