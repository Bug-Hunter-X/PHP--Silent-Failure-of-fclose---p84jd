# PHP: Silent Failure of fclose()

This repository demonstrates a common, yet subtle, error in PHP file handling: ignoring the return value of the `fclose()` function.  While seemingly innocuous, this can lead to resource leaks and unexpected behavior if the file closure fails.

The `bug.php` file shows the problematic code.  The `bugSolution.php` file provides the corrected version with proper error handling.

This is a simple example, but the principle applies to any situation where a function might fail silently and resource management is critical.