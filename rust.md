# rust

## learning rust

- **https://www.zero2prod.com/index.html?country=Austria&discount_code=VAT20** truely awesome!
- https://github.com/rust-lang/rustlings
- https://rust-exercises.com/
- https://github.com/sger/RustBooks
  - https://rust-unofficial.github.io/patterns/idioms/coercion-arguments.html
  - https://www.lurklurk.org/effective-rust/
  - https://rustwasm.github.io/docs/book/introduction.html
  - https://burn.dev/book/overview.html
  - https://www.manning.com/books/rust-design-patterns
  - https://nnethercote.github.io/perf-book/introduction.html

### Tips
- https://blog.sdf.com/p/fast-development-in-rust-part-one
- https://blog.sdf.com/p/fast-development-in-rust-part-2

### macros
- https://veykril.github.io/tlborm/

## rust and python
- https://pyo3.rs/v0.21.2/


## toolchain

- multi project build with workspaces https://doc.rust-lang.org/book/ch14-03-cargo-workspaces.html
- optimize build config https://github.com/Kobzol/cargo-wizard
- `cargo-watch` with `cargo watch -x check`
- sort cargo dependencies https://github.com/DevinR528/cargo-sort
### scaling the build beyond kargo

- https://mmapped.blog/posts/17-scaling-rust-builds-with-bazel
- https://users.rust-lang.org/t/static-linking-for-rust-without-glibc-scratch-image/112279/8

### ci-cd examples

- https://gist.github.com/FedericoPonzi/873aea22b652572f5995f23b86543fdb
- https://github.com/f2calv/multi-arch-container-rust
- https://blog.urth.org/2023/03/05/cross-compiling-rust-projects-in-github-actions/
- https://github.com/dirien/rust-cross-compile

  
### dependencies
- https://www.lurklurk.org/effective-rust/dep-graph.html cargo-udeps/cargo-deny

### documentation
- https://www.lurklurk.org/effective-rust/documentation.html
  - `#![deny(broken_intra_doc_links)]`
  - `#![warn(missing_docs)]`
- `cargo doc`

### formatting

- https://github.com/rust-lang/rustfmt ` rustup component add rustfmt`, `cargo fmt`, ` cargo fmt -- --check`

### linters

- clippy https://doc.rust-lang.org/clippy/installation.html ` rustup component add clippy`, `cargo clippy`, `cargo clippy -- -D warnings`
- security audit ` cargo install cargo-audit`, `cargo audit`
- https://github.com/EmbarkStudios/cargo-deny `cargo install --locked cargo-deny && cargo deny init && cargo deny check`

### databases & ORM

- https://github.com/launchbadge/sqlx

### testing

- https://github.com/la10736/rstest
- https://github.com/rust-lang/miri
- https://github.com/rust-fuzz/cargo-fuzz
- https://github.com/obi1kenobi/cargo-semver-checks
- https://crates.io/crates/criterion
- coverage
  - https://docs.rs/cargo-tarpaulin/latest/cargo_tarpaulin/ `cargo install cargo-tarpaulin` ` cargo tarpaulin --ignore-tests`

## learnings

### macros

- automatically derive macros i.e. for equality https://rust-exercises.com/04_traits/04_derive
  ```
  #[derive(PartialEq)]
  ```

### architecture in rust

- https://alexis-lozano.com/hexagonal-architecture-in-rust-1/

### web frameworks

- https://github.com/LukeMathWalker/pavex
- https://actix.rs/
- https://github.com/tokio-rs/axum
- https://github.com/poem-web/poem
- https://leptos.dev/
- https://yew.rs/
- open api doc
  - https://docs.rs/utoipa/latest/utoipa/
  - https://github.com/paperclip-rs/paperclip

### security

(not only rust specific)

- https://owasp.org/www-project-application-security-verification-standard/
- https://cheatsheetseries.owasp.org/cheatsheets/Password_Storage_Cheat_Sheet.html

### useful crates

- errors
  - https://crates.io/crates/thiserror
- parallelism
  - https://github.com/rayon-rs/rayon
- frontend
  - Tauri https://tauri.app/ (electron like)
  - https://github.com/redbadger/crux
- IO
  - https://opendal.apache.org/
### data engineering and rust

- https://blog.duyet.net/2023/06/fossil-data-platform-written-rust.html
- https://rustfordata.com/chapter_1.html
## embedded

- https://github.com/rust-embedded/rust-raspberrypi-OS-tutorials
