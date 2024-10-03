
-  
___
**JIT** -> Unlike traditional compiled languages, where source code is compiled entirely into machine code **before execution**, in JIT compilation, code is compiled **just when it is needed** during execution.
- The **"just in time"** part refers to the fact that instead of translating the entire program into machine code before it runs, JIT compiles methods or parts of the code **only at the moment they are about to be executed** for the first time.
___
# Comparison
## Visual comparison
### Compiled Language
![[compiled-language.png]]

### Interpreted Language
![[interpreted-language.png]]

### Managed Language
![[managed-language-compiler.png]]![[managed-language-jit.png]]![[managed-langugage.png]]![[managed-langu![[managed-language-jit.png]]age-jit.png]]







## Tabular Comparison
	## Compiled vs. Interpreted vs. Managed Languages

| Feature | Compiled Languages | Interpreted Languages | Managed Languages |
|---|---|---|---|
| Code Translation | Source code is compiled into machine-specific binary code | Source code is translated line-by-line during execution | Source code is compiled into intermediate language (IL/bytecode), then JIT compiled to machine code at runtime |
| Execution Speed | Fast (since machine code is executed directly) | Slower (due to runtime interpretation of code) | Near-native speed (due to JIT compilation and caching) |
| Memory Management | Manual (developer manages memory allocation and deallocation) | Automatic (handled by the interpreter) | Automatic (via garbage collection) |
| Typing | Typically strongly typed | Typically loosely typed or dynamically typed | Strongly typed (type information available at both compile-time and runtime) |
| Portability | Platform-specific (requires recompilation for different platforms) | High (interpreters are platform-independent) | High (requires a runtime like .NET CLR or Java JVM to run) |
| Error Checking | Compile-time errors caught early, but runtime memory errors are common | Errors are found at runtime (due to dynamic typing) | Compile-time and runtime error checking, with type safety and memory safety |
| Development Speed | Slower due to need for recompilation after changes | Faster due to no compilation step | Moderate (compilation is quick, but JIT improves performance during execution) |
| Performance | Excellent performance (compiled code runs directly on CPU) | Typically slower due to interpretation overhead | Close to native performance (due to JIT compilation and optimization) |
| Common Examples | C, C++, Rust | Python, JavaScript, Ruby | C#, Java, .NET languages |
| Runtime Overhead | Low (no runtime overhead after compilation) | High (interpreter continuously translates code during execution) | Moderate (JIT adds some overhead, but machine code is cached for reuse) |
| Memory Safety | Developer must handle manually (risk of memory leaks) | Automatic, but no low-level control over memory | Automatic with garbage collection and runtime checks |
| Calling the Same Method 1000 Times | Executed 1000 times directly by the CPU without additional overhead | Each time, the interpreter translates the method again, causing overhead on every call | IL-to-machine code translation happens only once on first call; subsequent calls use the cached machine code | 

**Summary:**

* **Compiled languages** are fast but less portable, requiring manual memory management.
* **Interpreted languages** are slower but more portable with automatic memory management.
* **Managed languages** strike a balance, offering strong performance, portability, and automatic memory management. 