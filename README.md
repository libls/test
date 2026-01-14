# LS Test Harness

Minimal, single-header unit test framework for C.

- Auto-registers test functions.
- Header-only.
- Macros: `ASSERT_EQ`, `ASSERT`, etc.
- ANSI C with minimal extensions.

## Quick Start

1. Copy `ls_test.h` to your project.
2. In one C file:
    ```c
    #define LS_TEST_IMPLEMENTATION
    #include "ls_test.h"
    ```
3. Write tests:
    ```c
    TEST_CASE(my_test) {
        ASSERT_EQ(add(1,2), 3, "%d");
        return 0;
    }
    ```
4. Add main:
    ```c
    TEST_MAIN
    ```
5. Compile and run.

## License

MIT.
