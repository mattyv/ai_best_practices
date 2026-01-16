# Minimum Project Requirements for AI Tool Use

## Build System

- [ ] Standard build commands work without special knowledge:
  ```bash
  cmake -S . -G Ninja -B build
  cmake --build build
  ctest --test-dir build
  ```
- [ ] Single command/script to build, test, and analyze
- [ ] Clear error messages if required tools are missing

## Compiler Warnings

- [ ] Warnings enabled: `-Wall -Wextra -Wconversion -Wshadow` (GCC/Clang) or `/W4` (MSVC)
- [ ] **Warnings as errors enabled** (`-Werror` / `/WX`)

## Static Analysis

- [ ] clang-tidy integrated into build
- [ ] clang-tidy warnings as errors
- [ ] `.clang-tidy` config file present

## Code Formatting

- [ ] clang-format integrated into build
- [ ] `.clang-format` config file present

## Dynamic Analysis

- [ ] UBSan enabled in default/debug build
- [ ] ASan enabled in default/debug build

## Testing

- [ ] Test framework set up (Catch2 header-only recommended)
- [ ] Tests run automatically with build or single command
- [ ] Code coverage enabled (`--coverage`)
- [ ] Single command to generate coverage report
- [ ] Coverage threshold enforced (coverage must not decrease)

## Documentation

- [ ] `CLAUDE.md` (or equivalent) containing:
  - Build instructions
  - Test instructions
  - Coverage instructions
  - Coding standards not enforced by tooling
  - Positive directives only ("always do X" not "never do Y")
  - Specific style requirements (e.g., "C++20 with constexpr" not "modern C++")

## Code Hygiene

- [ ] No stale/dead code
- [ ] No commented-out code
- [ ] No incomplete stub functions
- [ ] No TODO comments for abandoned work

## CI/CD

- [ ] CI pipeline configured
- [ ] Tests run on multiple compilers/platforms
- [ ] All checks (build, test, analysis, formatting) run in CI

## Advanced (Optional)

- [ ] Mutation testing enabled
