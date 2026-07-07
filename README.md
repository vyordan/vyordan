# Hello! I'm Yordan Vásquez

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/vyordan)

I'm a 20-year-old Guatemalan student of Systems Engineering (6th semester).  
I enjoy efficient software development.  
I focus on native and system-level applications and development.  
Most of what I know I've learned through personal projects, self-taught.

## Open Source Contributions
### [0 A.D. Empires Ascendant](https://play0ad.com/) [(Wildfire Games)](https://wildfiregames.com/) – Contribution to the **Pyrogenesis** engine (C++)
* [Progressive loading optimization (VSync) – PR #8898](https://gitea.wildfiregames.com/0ad/0ad/pulls/8898)  
  Optimized the progressive resource loading system by implementing a dynamic CPU budget linked to the refresh rate (VSync).
* [Script namespace refactoring – PR #8948](https://gitea.wildfiregames.com/0ad/0ad/pulls/8948)  
  Massive reorganization of the `Script` namespace – Renamed classes and files, updated over 200 engine files.
* [Consistent typing for turns – Issue #8718](https://gitea.wildfiregames.com/0ad/0ad/issues/8718) / [PR #9017](https://gitea.wildfiregames.com/0ad/0ad/pulls/9017) (PR open)  Proposed and implemented `turn_id_t` as an alias for `std::int64_t`, unifying the type used for turn counters across the simulation, network, and replay systems (previously a mix of `int`, `uint32_t`, and `u32`).
* [Unified replay folder naming across multiplayer participants – PR #9037](https://gitea.wildfiregames.com/0ad/0ad/pulls/9037)  
Unified replay folder names across all participants by using the synced `matchID` instead of a local sequence counter, added a synced `startTime` attribute (via `std::chrono`) for the date prefix, and introduced a dedicated subdirectory method to handle rejoins gracefully.
* **Work Methodology:** Remote collaboration under professional standards. Handling iterative reviews, Jenkins log analysis, and build verification on Linux, macOS, Windows, and FreeBSD.

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
