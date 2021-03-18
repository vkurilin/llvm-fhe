# llvm-fhe
Translation of llvm-ir into of native interfaces of fully homomorphic encryption libraries.

Unlike [SHEEP](https://github.com/alan-turing-institute/SHEEP) project, this project aims to generating code, allowing you to:
1. Get rid of any overhead caused by on-the-fly translation from SHEEP circuit language
   if your goal is to explore current limitations of fully homomorphic encryption
   
2. The lowest possible entry level for using fully homomorphic encryption in your project.
   It's enough for you just to write a function in the original programming language 
   without using unsupported constructs, and boom - code is generated that calls the native methods 
   of the most suitable library of fully homomorphic encryption.
   
------
Thanks [SHEEP](https://github.com/alan-turing-institute/SHEEP) for the idea and implementation of a 
uniform interface to different fhe-libraries.
Thanks [llvm-tutor](https://github.com/banach-space/llvm-tutor) for a great example of building new-style LLVM passes.
