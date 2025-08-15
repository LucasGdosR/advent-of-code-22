# Advent of Code of 2022
For this year, my personal challenges are to solve it in Odin and create visualizations.

I have an extra challenge of thinking of how to solve the problem with a multi-threaded solution. In general, I only propose how it could be multi-threaded, but there may be some multi-threaded solutions and visualizations.

- [x] 01: multi-threaded
- [x] 02: single-threaded; multi-threaded solution idea: parallelize the `for-loop`, each thread accumulates to local variables, and sum accumulated solutions.
- [x] 03: single-threaded; multi-threading: in theory, every set of three lines is indepedent. In practice, with varying lengths, finding sets requires reading them. Might as well solve them. Multi-threading not recommended.
- [x] 04: single-threaded; multi-threaded solution idea: chunk the input roughly, then adjust chunk boundaries to match line breaks. Proccess chunks independently, then sum accumulated solutions.
- [x] 05: single-threaded; multi-threading: this problem is serial, as it deals with stacks. It cannot be solved with multi-threading, except that part 1 and part 2 can be solved in parallel (so 2 threads max).
- [x] 06: single-threaded; multi-threaded solution idea: chunk the input and make chunks overlap so every substring is examinated by one thread. Get the solution index from the thread with the chunk with lowest starting index.
- [x] 07: single-threaded; multi-threading: this problem deals with trees, which are just stacks over time. The first pass, which builds the tree, is therefore serial. With the tree built, the second pass using DFS can be made in parallel, with different threads recursively exploring different branches of the tree. It's trivial with a multi-threading runtime (such as OpenCilk), but tricky with a from scratch solution.
- [x] 08: single_threaded; multi-threadded solution idea: the loops can be done in parallel as long as they don't try to write to the same index in the grid. This is trivial for part 2, which is read-only.
- [ ] 09
- [ ] 10
- [ ] 11
- [ ] 12
- [ ] 13
- [ ] 14
- [ ] 15
- [ ] 16
- [ ] 17
- [ ] 18
- [ ] 19
- [ ] 20
- [ ] 21
- [ ] 22
- [ ] 23
- [ ] 24
- [ ] 25
