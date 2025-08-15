# tiny-allocator

A small, educational memory allocator written in C.  
`tiny-allocator` starts with a simple bump allocator and evolves into a free-list–based system with coalescing, alignment, and `realloc` support.

## Features (planned)

- **Bump Allocator** – ultra-fast linear allocation.
- **Free List Allocator** – freeing, coalescing, and reuse.
- **Alignment Handling** – align allocations to 8/16 bytes.
- **Realloc Support** – grow/shrink allocations safely.
- **Valgrind Clean** – no leaks, no nonsense.

## Goals

- Understand how `malloc`, `free`, and `realloc` work internally.
- Explore fragmentation, alignment, and heap metadata.
- Keep the implementation small and readable.
- Serve as a hands-on learning project for C developers.

## Build & Run

```bash
# Build the allocator demo
make

# Run demo program
./bin/allocator

# Run tests
make test

# Check for leaks with Valgrind
valgrind --leak-check=full ./bin/alloc_tests
