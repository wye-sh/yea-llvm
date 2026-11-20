# yea-llvm

A trimmed copy of the official [LLVM 19.1.7](https://github.com/llvm/llvm-project/releases/tag/llvmorg-19.1.7) Linux x64 release, with only the files Yea's builds use (clang, lld and the LLVM tools Yea calls, plus clang's resource headers) and LLVM's licence. The files are unchanged; only the others are left out.

It's packed with zstd: 93 MB, which unpacks in about 1 s, where the official 1.6 GB xz takes 23 s. Yea's `tools/bootstrap.sh` downloads it from this repository's Releases and checks its sha256.

LLVM is licensed under the Apache License v2.0 with LLVM Exceptions; see `LICENSE.TXT`.
