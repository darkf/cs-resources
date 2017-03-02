<a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">Creative Commons Attribution-NonCommercial 4.0 International License</a>.

# Computer Science / Programming Resource Guide

## General Topics


### Game Development
See also the general topics below, especially data structures and algorithms.
- [Game Programming Patterns](http://gameprogrammingpatterns.com/) (free book on some design patterns possibly useful in games)
- [Invent Your Own Computer Games with Python](https://inventwithpython.com/chapters/), [Making Games with Python & Pygame](https://inventwithpython.com/pygame/chapters/) (free books)
- [Entity Component Systems](https://en.wikipedia.org/wiki/Entity%E2%80%93component%E2%80%93system)
  - [A simple high-level explanation](http://gamedev.stackexchange.com/a/31491)
  - [Evolve Your Hierarchy](http://cowboyprogramming.com/2007/01/05/evolve-your-heirachy) (one of the earlier mainstream ECS papers)
- [What Every Coder Should Know About Gamma](http://blog.johnnovak.net/2016/09/21/what-every-coder-should-know-about-gamma)
- [Constructive Solid Geometry](https://en.wikipedia.org/wiki/Constructive_solid_geometry) (CSG) -- boolean operations on meshes
- [Fast Inverse Square Root](https://en.wikipedia.org/wiki/Fast_inverse_square_root) -- famous algorithm for calculating `1 / sqrt(x)`, used heavily for vector normalization (originally for lighting in Quake III Arena)
- [Fix Your Timestep!](http://gafferongames.com/game-physics/fix-your-timestep) (or, how to do timesteps right. Read it.)
- [Game Networking](http://gafferongames.com/networking-for-game-programmers)
- [Red Blob Games](http://www.redblobgames.com/) (good visual resource on algorithms like A\*, hexagonal grids, etc.)
- [Catmull-Rom splines](https://en.wikipedia.org/wiki/Centripetal_Catmull%E2%80%93Rom_spline) (splines that pass through all control points; good for games)

- Game AI
  - [Behavior Trees](https://en.wikipedia.org/wiki/Behavior_tree)
  - [Boids](https://en.wikipedia.org/wiki/Boids) (flocking behavior)

### Programming Language Theory and Compilers/Interpreters
- [The Programming Languages Zoo](http://plzoo.andrej.com)
- [(How to Write a (Lisp) Interpreter (in Python))](http://norvig.com/lispy.html) (follow-up: [(An ((Even Better) Lisp) Interpreter (in Python))](http://norvig.com/lispy2.html))
- [Build Your Own Lisp](http://www.buildyourownlisp.com)
- [The Implementation of Functional Programming Languages](http://research.microsoft.com/en-us/um/people/simonpj/papers/slpj-book-1987)
- [Hindley-Milner explanation](http://akgupta.ca/blog/2013/05/14/so-you-still-dont-understand-hindley-milner)
- [Modern Compiler Implementation in ML](https://www.cs.princeton.edu/~appel/modern/ml) (commercial book; variants in C and Java are available, but aren't as good)
- [Compilers: Principles, Techniques, and Tools](https://en.wikipedia.org/wiki/Compilers:_Principles,_Techniques,_and_Tools) (aka The Dragon Book)
- [Write You A Haskell](http://dev.stephendiehl.com/fun) (currently unfinished)
- [Official LLVM Tutorial](http://llvm.org/docs/tutorial/) (implements a compiler for a tiny toy language called Kaleidoscope); [Haskell](http://www.stephendiehl.com/llvm/) and [OCaml](http://llvm.org/docs/tutorial/OCamlLangImpl1.html) versions also available. 
- [Control Flow Graphs/Analysis](https://en.wikipedia.org/wiki/Control_flow_graph)
- [Data Flow Graphs/Analysis](https://en.wikipedia.org/wiki/Data-flow_analysis)

- Optimization
  - [Constant Folding](https://en.wikipedia.org/wiki/Constant_folding) (basic optimization by statically evaluating constants)
  - [Automatic Vectorization](https://en.wikipedia.org/wiki/Automatic_vectorization) -- automatically convert scalar code to vectorized (SIMD) code
  - [Deforestation](https://en.wikipedia.org/wiki/Deforestation_(computer_science))
  - [Dead Code Elimination](https://en.wikipedia.org/wiki/Dead_code_elimination) (via control flow analysis)
  
- Talks
  - [Growing A Language](https://www.youtube.com/watch?v=_ahvzDzKdB0) (by Guy Steele Jr. of Scheme fame, on the challenges of designing languages that can scale)
  

### Decompilation
- [Reverse Compilation Techniques](https://yurichev.com/mirrors/DCC_decompilation_thesis.pdf) (Cristina Cifuentes' rather in-depth thesis on decompilation)
- [decomp](https://github.com/decomp/decomp)

### Parsing
- [Pratt parsers](http://journal.stuffwithstuff.com/2011/03/19/pratt-parsers-expression-parsing-made-easy) (Recursive Descent + Top Down operator precedence parsing = Pratt parsers)
- [PEG grammars, Packrat parsers](https://en.wikipedia.org/wiki/Parsing_expression_grammar)
- [Top-Down operator precedence parsing](http://eli.thegreenplace.net/2010/01/02/top-down-operator-precedence-parsing)
- [Earley parsers](https://en.wikipedia.org/wiki/Earley_parser) (can parse any grammar)
- [Shunting-yard algorithm](https://en.wikipedia.org/wiki/Shunting-yard_algorithm) (Dijkstra's algorithm for easy infix expression parsing (infix to tree/prefix/postfix))
- [Reverse Polish Notation](https://en.wikipedia.org/wiki/Reverse_Polish_notation) (aka postfix notation)
- [Monadic Parsing in Haskell](http://www.cs.nott.ac.uk/~pszgmh/pearl.pdf) (parsing with monadic combinators)
- [Sexy Lexing with Python](https://web.archive.org/web/20140428082426/http://www.evanfosmark.com/2009/02/sexy-lexing-with-python)

### Algorithms
- [Introduction to Algorithms](https://mitpress.mit.edu/books/introduction-algorithms) (also known as CLRS, a famous algorithms book)
- [Big O in Plain English](http://stackoverflow.com/a/487278)
- [Boyer–Moore–Horspool algorithm](https://en.wikipedia.org/wiki/Boyer%E2%80%93Moore%E2%80%93Horspool_algorithm) (fast substring search, used notably in `grep`)
- [Burrows–Wheeler transform](https://en.wikipedia.org/wiki/Burrows%E2%80%93Wheeler_transform) (decreases entropy in data reversibly, used notably in `bzip2`)
- [Huffman coding](https://en.wikipedia.org/wiki/Huffman_coding) (tree for generating optimal prefix codes, used a lot in compression)
- [Bucket Sort](https://en.wikipedia.org/wiki/Bucket_sort), [Tree Sort](https://en.wikipedia.org/wiki/Tree_sort), [Radix Sort](https://en.wikipedia.org/wiki/Radix_sort)
- Pathfinding / Graph Searching
  - [Dijkstra's Algorithm](https://en.wikipedia.org/wiki/Dijkstra's_algorithm) (general shortest-path pathfinding / graph traversal)
  - [A*](https://en.wikipedia.org/wiki/A*_search_algorithm) (Dijkstra's algorithm with heuristics, very commonly used)
  - [D* Lite](https://en.wikipedia.org/wiki/D*#D.2A_Lite)
  - [Jump Point Search](https://en.wikipedia.org/wiki/Jump_point_search)
- [Topological sorting](https://en.wikipedia.org/wiki/Topological_sorting) (for ordering nodes in a graph based on dependents)
- [Neural Networks and Deep Learning](http://neuralnetworksanddeeplearning.com/) (free book)
- [Creating A Genetic Algorithm For Beginners](http://www.theprojectspot.com/tutorial-post/creating-a-genetic-algorithm-for-beginners/3)

### Data Structures
- [Bloom Filter](https://en.wikipedia.org/wiki/Bloom_filter)
- van Laarhoven lenses (see the Haskell section on `lens`)
- [Purely Functional Data Structures](https://www.amazon.com/Purely-Functional-Structures-Chris-Okasaki/dp/0521663504) (commercial book; extended from [freely available thesis](https://www.cs.cmu.edu/~rwh/theses/okasaki.pdf))
- Free Monads
  - [Purify Code Using Free Monads](http://www.haskellforall.com/2012/07/purify-code-using-free-monads.html)
  - [You Could Have Invented Free Monads](http://www.haskellforall.com/2012/06/you-could-have-invented-free-monads.html)
- Spatial partitioning
  - [Quadtrees](https://en.wikipedia.org/wiki/Quadtree) (2D), [Octrees](https://en.wikipedia.org/wiki/Octree) (3D)
  - [Bounding Volume Hierarchies](https://en.wikipedia.org/wiki/Bounding_volume_hierarchy)
  - [Binary Space Partitioning](https://en.wikipedia.org/wiki/Binary_space_partitioning) (BSP)
- [Tries](https://en.wikipedia.org/wiki/Trie)
- [Interval trees](https://en.wikipedia.org/wiki/Interval_tree) / [Segment trees](https://en.wikipedia.org/wiki/Segment_tree)
- [Blockchain 101](https://anders.com/blockchain) (a good video tutorial and demonstration of [blockchains](https://en.wikipedia.org/wiki/Blockchain_(database)))
- [Distributed Hash Table](https://en.wikipedia.org/wiki/Distributed_hash_table) (self-explanatory; notably used in BitTorrent)

- Memory Allocation
  - [Free Lists](https://en.wikipedia.org/wiki/Free_list)
  - [Buddy memory allocation](https://en.wikipedia.org/wiki/Buddy_memory_allocation)
  - [Dynamic Memory Allocation: Advanced Concepts](http://www.cs.cmu.edu/afs/cs/academic/class/15213-s11/www/lectures/20-allocation-advanced.pdf) (slides; includes Segregated Free Lists)
  - [Reference Counting](https://en.wikipedia.org/wiki/Reference_counting) (a simple form of garbage collection)

### Regular Expressions (Regex)

- [Regular-Expressions.info](http://regular-expressions.info) (tutorial and reference)
- [refiddle](http://refiddle.com), [regex101](https://regex101.com), [regexpal](http://www.regexpal.com) (online regex testers)
- [Implementing Regular Expressions](https://swtch.com/~rsc/regexp)
  - [Regular Expression Matching Can Be Simple And Fast](https://swtch.com/~rsc/regexp/regexp1.html) in particular is well worth a read

### IEEE 754 Floating Point

- What Every Computer Scientist Should Know About Floating-Point Arithmetic [HTML reprint](https://docs.oracle.com/cd/E19957-01/806-3568/ncg_goldberg.html) / [PDF](https://ece.uwaterloo.ca/~dwharder/NumericalAnalysis/02Numerics/Double/paper.pdf)
- http://0.30000000000000004.com
- http://floating-point-gui.de

## Cryptography
- [Lifetimes of cryptographic hash functions](https://valerieaurora.org/hash.html)

## Emulation
- [How To Write a Computer Emulator](http://fms.komkon.org/EMUL8/HOWTO.html) (older Emulation FAQ)
- [GameBoy Emulation in JavaScript](http://imrannazar.com/GameBoy-Emulation-in-JavaScript:-The-CPU) (a tutorial)
- [Statically Recompiling NES Games into Native Executables with LLVM and Go](http://andrewkelley.me/post/jamulator.html) (an attempt at statically recompiling NES binaries)

## Interesting Operating Systems

- [NixOS](https://nixos.org) (see also [Nix](https://nixos.org/nix), its more portable package manager) -- an OS built around Nix, a referentially transparent package manager. Allows you to build an entire OS setup around a single config file, with multiple profiles and no package dependency hell.
- [MenuetOS](http://menuetos.net) -- fairly modern OS written in x86_64 assembly
- [MINIX](https://en.wikipedia.org/wiki/MINIX) -- the teaching OS

## Computer Architectures

### General Concepts
- [Harvard architecture](https://en.wikipedia.org/wiki/Harvard_architecture), [Modified Harvard architecture](https://en.wikipedia.org/wiki/Modified_Harvard_architecture)
- [Stack machines](https://en.wikipedia.org/wiki/Stack_machine) (useful in programming language VMs or concatenative languages)
- [Register machines](https://en.wikipedia.org/wiki/Register_machine)
- [Delay slots](https://en.wikipedia.org/wiki/Delay_slot)
- [Branch Prediction](https://en.wikipedia.org/wiki/Branch_predictor)

### [Lisp Machines](https://en.wikipedia.org/wiki/Lisp_machine)

### [Pong Story](http://pong-story.com)

### x86 / x86_64
- [x86 Assembly Wikibook](https://en.wikibooks.org/wiki/X86_Assembly)
- [x86 Instruction Set Reference](http://x86.renejeschke.de)
- [\[xchg rax,rax\]](https://www.xorpd.net/pages/xchg_rax/snip_00.html) -- interesting/clever x86_64 snippets
- [x86_64 AMD Programmer's Manual (Volume 2, System Programming)](http://support.amd.com/TechDocs/24593.pdf)
- [x86_64 AMD Programmer's Manual (Volume 3, Instruction Reference)](http://support.amd.com/TechDocs/24594.pdf)
- [x86_64 System V ABI](https://software.intel.com/sites/default/files/article/402129/mpx-linux64-abi.pdf)
- [x86_64 ELF File Format](https://uclibc.org/docs/elf-64-gen.pdf)

### MIPS
- [SPIM](http://spimsimulator.sourceforge.net) (MIPS simulator; unfortunately no macros/pseudo-instructions)
- [MARS](http://courses.missouristate.edu/KenVollmar/mars) (another MIPS simulator, more featureful but requires Java)

## Language Specific

### General / Multi-Language
- [Learn X in Y Minutes](https://learnxinyminutes.com) (short intros/walkthroughs of languages via demonstration code with comments)


### Python
- [Automate the Boring Stuff with Python](https://automatetheboringstuff.com) (free book)
- [Documentation](https://docs.python.org/3)
  - GUIs
    - Qt
      - [PyQt](http://pyqt.sourceforge.net) (note that the free version is licensed under the GPL, act accordingly)
      - [PySide](https://wiki.qt.io/PySide) (LGPL but currently Qt 4 only)
      - Tutorials: [PyQt4](http://zetcode.com/gui/pyqt4), [PyQt5](http://zetcode.com/gui/pyqt5), [PySide](http://zetcode.com/gui/pysidetutorial)
    - Tkinter
      - [Tkinter tutorial](http://zetcode.com/gui/tkinter)
      - [Graphical User Interfaces with Tk](https://docs.python.org/3/library/tk.html)

### JavaScript
- [Eloquent Javascript](http://eloquentjavascript.net/) (free book)
- [You Don't Know JS](https://github.com/getify/You-Dont-Know-JS) (series of free books)
- [this](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/this)
- [Fetch API](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API)
- [Typed Arrays](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Typed_arrays) for manipulating binary data / compact native arrays
- [Web Storage](https://developer.mozilla.org/en-US/docs/Web/API/Web_Storage_API), [IndexedDB](https://en.wikipedia.org/wiki/Indexed_Database_API) -- offline in-browser databases
- [TextEncoder](https://developer.mozilla.org/en-US/docs/Web/API/TextEncoder)/[TextDecoder](https://developer.mozilla.org/en-US/docs/Web/API/TextDecoder) APIs for text codecs
- [asm.js](https://en.wikipedia.org/wiki/Asm.js) -- a subset of JavaScript (statically type inferrable, no GC) targetted at efficient machine translation/compilation
- [Web Assembly](http://webassembly.org/) -- a text (S-expression based) and binary IR with goals similar to asm.js
- [SIMD.js](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/SIMD)
- [Emscripten](https://github.com/kripken/emscripten), [Cheerp](http://leaningtech.com/cheerp/) -- C/C++/LLVM to JavaScript/asm.js/webasm compilers
- [Ramda](http://ramdajs.com) -- a library for functional programming in JavaScript; includes lenses, immutable data structures, and is generally much better than lodash.

### TypeScript
- [Tutorial](https://www.typescriptlang.org/docs/tutorial.html)
- [Handbook](https://www.typescriptlang.org/docs/handbook/basic-types.html)
- [Compiler Options Reference](https://www.typescriptlang.org/docs/handbook/compiler-options.html)
- [TypeSearch](http://microsoft.github.io/TypeSearch) (searches for type definitions)

### CSS
- [A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/), [A Complete Guide to Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)

### Java
- [Interface Pollution in the JDK 8](http://archive.is/PeQng)

### Lua
- [LuaJIT](http://luajit.org) (fast JITed Lua interpreter)
- [New Garbage Collector](http://wiki.luajit.org/New-Garbage-Collector) (design doc for LuaJIT 3's future GC)
- [Love](https://love2d.org) (a standalone game framework in Lua using LuaJit)

### Haskell
- [Learn You a Haskell for Great Good!](http://learnyouahaskell.com) (free book)
- [Haskell Programming from First Principles](http://haskellbook.com) (free book)
- [Real World Haskell](http://book.realworldhaskell.org/) (free book)
- [What I Wish I Knew When Learning Haskell](http://dev.stephendiehl.com/hask) (very useful rundown of the ecosystem, common and useful packages/types/etc)
- [Introduction to Haskell](http://www.seas.upenn.edu/~cis194/spring13/lectures.html)
- [Documentation for Prelude](https://hackage.haskell.org/package/base/docs/Prelude.html)
- [Stack](https://docs.haskellstack.org/en/stable/README) (Package manager with stable package tree snapshots and sandboxing)
- Lenses
  - [lens](http://lens.github.io) library
  - [History of Lenses](https://github.com/ekmett/lens/wiki/History-of-Lenses)
  - [Lenses in Pictures](http://adit.io/posts/2013-07-22-lenses-in-pictures.html) (nice visual explanation)
- [Functors, Applicatives, And Monads In Pictures](http://adit.io/posts/2013-04-17-functors,_applicatives,_and_monads_in_pictures.html) (visual explanation of functors/applicative functors/monads)
- [A History of Haskell: Being Lazy With Class](http://research.microsoft.com/en-us/um/people/simonpj/papers/history-of-haskell) (a history of Haskell)
- [Philip Wadler's monad papers](http://homepages.inf.ed.ac.uk/wadler/topics/monads.html)
  - [Monads For Functional Programming](http://homepages.inf.ed.ac.uk/wadler/papers/marktoberdorf/baastad.pdf)
- See the *Purely Functional Data Structures* and *Free Monads* sections in Data Structures above

### LISP
- [Recursive Functions of Symbolic Expressions and Their Computation by Machine](http://www-formal.stanford.edu/jmc/recursive.html) (seminal LISP paper by McCarthy)
- [Structure and Interpretation of Computer Programs](https://mitpress.mit.edu/sicp) (also known as The Wizard Book)
- [Lambda Papers](http://library.readscheme.org/page1.html)

### Racket
- [Racket Guide](https://docs.racket-lang.org/guide/intro.html)
- [Realm of Racket](http://realmofracket.com) (commercial book)

### Erlang
- [Learn You Some Erlang for Great Good!](http://learnyousomeerlang.com) (free book)
- [Documentation](https://www.erlang.org/docs)

### OCaml
- [Real World OCaml](https://realworldocaml.org) (free book)
- [Documentation](http://www.ocaml.org/docs)
- [OPAM](http://opam.ocaml.org) (Package Manager)

### Rust
- [Rust By Example](http://rustbyexample.com) (free book)
- [Manual](https://doc.rust-lang.org/book)
- [Documentation](https://doc.rust-lang.org/std)
- [docs.rs](https://docs.rs) (Third-party package documentation)

### D
- [Programming in D](http://ddili.org/ders/d.en/index.html) (free book / tutorial / reference)
- [Language Reference](https://dlang.org/spec/spec.html)
- [Library Reference](https://dlang.org/phobos/index.html)

### Fortran
- [Fortran on the IBM 704](https://www.fortran.com/FortranForTheIBM704.pdf) (manual for the original Fortran for the IBM 704, from 1957)

## Web

### HTTP
  - [HTTP Made Really Easy](https://www.jmarshall.com/easy/http) (simple introduction/guide to HTTP 1.0 and 1.1)

### Optimization
  - [High Performance Browser Networking](http://chimera.labs.oreilly.com/books/1230000000545/index.html) (free book)

## Tools

### Git
- [git - the simple guide](http://rogerdudler.github.io/git-guide) (simple intro to git)
- [Pro Git](https://git-scm.com/book/en/v2) (free book)
- [Oh shit, git!](http://ohshitgit.com) (for when you inevitably mess up)

### Make
- [Make files not war](https://fabianstumpf.de/articles/makefiles.htm) (tutorial on make)

## Design

- [Dark Patterns](http://darkpatterns.org) (sets of subversive and potentially malicious design patterns)
- [Motherfucking Website](http://motherfuckingwebsite.com) -> [Better Motherfucking Website](http://bettermotherfuckingwebsite.com) -> [Best Motherfucking Website](https://bestmotherfucking.website)

## Culture

- [How To Ask Questions The Smart Way](http://www.catb.org/~esr/faqs/smart-questions.html)
- [On The Cruelty Of Really Teaching Computing Science](https://www.cs.utexas.edu/~EWD/transcriptions/EWD10xx/EWD1036.html) (famous Dijkstra essay)
- [Grace Hopper on Letterman](https://www.youtube.com/watch?v=1-vcErOPofQ)
- [The Cathedral and the Bazaar](http://www.catb.org/esr/writings/cathedral-bazaar) (free book/essay by Eric Raymond)
- [The Jargon File](http://www.catb.org/jargon/html)
- [Execution in the Kingdom of Nouns](http://steve-yegge.blogspot.com/2006/03/execution-in-kingdom-of-nouns.html) (essay on Java-style OOP by Steve Yegge)
- [Kill -9 by Monzy](https://www.youtube.com/watch?v=Fow7iUaKrq4) (a very dense CS-laden nerdrap song performed live at Stanford)
- [Land of Lisp - The Music Video](https://www.youtube.com/watch?v=HM1Zb3xmvMc)
