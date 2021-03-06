# edit-distance

[![Build Status](https://travis-ci.org/vmchale/edit-distance.svg?branch=master)](https://travis-ci.org/vmchale/edit-distance)

The Levenshtein edit distance, packaged for ATS. This implementation is written
in safe ATS and is performant.

## Benchmarks

| Language | Library | Unicode | Time |
| -------- | ------- | ------- | ---- |
| ATS | `edit-distance` |  | 67.61 ns |
| Rust | `levenshtein-rs` | X | 137.4 ns
| Rust | `strsim` | X | 140.4 ns
| Haskell | `edit-distance` | X | 413.5 ns |
| C | n/a |  | 93.70 ns |

Note that these benchmarks use `libgc` for ATS and C and thus ATS and
C functions may be faster if you use manual memory management.
