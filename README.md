# Hello! I'm Yordan Vásquez

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/vyordan)

Junior Systems Developer | 20-year-old Guatemalan student of Systems Engineering (6th semester).
I like efficient software development, particularly native and system-level applications. Most of what I know comes from self-teaching and personal projects.

## Open Source Contributions
### [LLVM Project](https://llvm.org/) – Contribution to **libc++** (C++ Standard Library)
* [LWG3133 implementation for std::complex and std::valarray – PR #208145](https://github.com/llvm/llvm-project/pull/208145)
  Implemented the resolution of LWG3133 by adding `operator_hijacker`-based tests to verify that `std::valarray::operator[]` does not rely on a user-overloadable `operator&`. Marked LWG3133 as Complete.
* [Diagnostic `static_assert`s for LWG3133 named requirements – PR #212360](https://github.com/llvm/llvm-project/pull/212360) **(Open)**
  Extends the previous PR by adding granular `static_assert` checks to both `std::complex` and `std::valarray`, verifying that `T` is a cv-unqualified object type satisfying the four named requirements (default_initializable, copy_constructible, copy_assignable, destructible), with dedicated `.verify.cpp` tests. Currently under review.
  
* [Fix `std::filesystem::canonical("")` to report an error – PR #215031](https://github.com/llvm/llvm-project/pull/215031) **(Open)**
  Fixed a bug where `std::filesystem::canonical("")` incorrectly returned the current directory instead of reporting an error as required by the C++ Standard (`[fs.op.canonical]`). Added an empty-path check before absolutizing, updated `weakly_canonical` internal calls to bypass the now-corrected `canonical("")`, and added dedicated tests.

### [0 A.D. Empires Ascendant](https://play0ad.com/) [(Wildfire Games)](https://wildfiregames.com/) – Contribution to the **Pyrogenesis** engine (C++)
* [Progressive loading optimization (VSync) – PR #8898](https://gitea.wildfiregames.com/0ad/0ad/pulls/8898)  
  Optimized the progressive resource loading system by implementing a dynamic CPU budget linked to the refresh rate (VSync).
* [Script namespace refactoring – PR #8948](https://gitea.wildfiregames.com/0ad/0ad/pulls/8948)  
  Massive reorganization of the `Script` namespace – Renamed classes and files, updated over 200 engine files.
* [Consistent typing for turns – PR #9017](https://gitea.wildfiregames.com/0ad/0ad/pulls/9017)  Proposed and implemented `turn_id_t` as an alias for `std::int32_t`, unifying the type used for turn counters across the simulation, network, and replay systems (previously a mix of `int`, `uint32_t`, and `u32`).
  
 **Work Methodology:** Remote collaboration under professional standards. Handling iterative reviews, Jenkins log analysis, and build verification on Linux, macOS, Windows, and FreeBSD.

#### [Credits](https://gitea.wildfiregames.com/0ad/0ad/src/branch/main/binaries/data/mods/public/gui/credits/texts/programming.json#:~:text=%7B%20%22nick%22%3A%20%22vyordan%22%2C%20%22name%22%3A%20%22Yordan%20Vasquez%22%20%7D) Nick: vyordan, Name: Yordan Vasquez

## My Tech Stack
*   **Languages:** C++, Java, SQL.
*   **Tools:** Git, CMake - Make/Ninja, Spring Boot, Repositories (Gitea, Github).
*   **Infrastructure:** Docker, Linux/Terminal (Arch and Fedora).
*   **CI/CD familiarity:** Reading and interpreting Jenkins logs for multi-platform build verification.
*   **Areas of Interest:** Engine Dev, Algorithm Optimization, Software Architecture.

## What I'm currently learning
*   **LLVM:** Intermediate Representation (IR) and compilers [KEM - JIT Compiler](https://github.com/vyordan/Kem).
*   **gRPC:** Efficient communication between microservices [Compresor](https://github.com/vyordan/Compresor).
