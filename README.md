# pascal-compiler           
            
Introduction         
Pascal is a procedural and imperative programming language. The various elements of the language are common to many other elements: the existence of if / then / elses,cycle(while,repeat,for) and the functions and procedures that promote the concept of DRY - don't repeat.          
       
Architecture   
Traditional compilers are written in a low-level language (usually C) that parses the input program, parses it, and converts it into machine code.     
          
           
need       
Python (2.5.4)                   
PLY (http://pypi.python.org/pypi/ply/3.1)                       
LLVM (http://llvm.org)                     
LLVM-py (http://mdevan.nfshost.com/llvm-py/download.html)            
              
                 
Semantic Analysis         
Whenever we enter a new block (whether it is a program, loop, function, procedure), we create a new context, adding itself to the stack (and deleting it at the end). This allows us to access the variable of the block and all the blocks it is in whenever we enter a block (but when adding a variable, it is always in the top block).          
      
      
Code generation          
If you find a program, when you browse the tree, create the block and add standard functions. And recursively traverse the block.           
           
           
conclusion       
In developing this work, I learned to perform various stages of compilation, and write the required code.    
