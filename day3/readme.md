READING AND INSPECTING FILES
On Day 3, I focused on learning how to read files and inspect information about them. I learned how to use "cat" to display the contents of a file and "less" to read large files page by page without displaying everything at once.

I learned how to use "head" to view the beginning of a file and "tail" to view the end of a file. I also learned how to use "head -n" and "tail -n" when I want to specify exactly how many lines I want to see. One particularly useful command I learned was "tail -f", which allows me to continuously monitor a file as new information is added. This is especially useful when working with log files.

I also learned how to use "wc" to count information about a file, including "wc -l" to count the number of lines. The "file" command helped me identify the type of a file, while the "stat" command allowed me to inspect detailed metadata such as file size, permissions, ownership, timestamps, and other information.

What surprised me is that tail -f continues to monitor files which is good for server logs, audit and security 
