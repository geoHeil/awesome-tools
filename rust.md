# rust

## learning rust

- **https://www.zero2prod.com/index.html?country=Austria&discount_code=VAT20** truely awesome!
- **https://www.howtocodeit.com/** really great!
- prototyping with rust https://corrode.dev/blog/prototyping/
- https://github.com/rust-lang/rustlings
- https://rust-exercises.com/
- https://github.com/sger/RustBooks
  - https://rust-unofficial.github.io/patterns/idioms/coercion-arguments.html
  - https://www.lurklurk.org/effective-rust/
  - https://rustwasm.github.io/docs/book/introduction.html
  - https://burn.dev/book/overview.html
  - https://www.manning.com/books/rust-design-patterns
  - https://nnethercote.github.io/perf-book/introduction.html
 
- https://antithesis.com/blog/is_something_bugging_you/
- https://joshlf.com/files/talks/Safety%20in%20an%20Unsafe%20World.pdf

### wow presentations

- https://www.youtube.com/watch?v=Lc8lBMEJQdo

### Tips
- https://blog.sdf.com/p/fast-development-in-rust-part-one
- https://blog.sdf.com/p/fast-development-in-rust-part-2
- named function arguments https://elastio.github.io/bon/blog/how-to-do-named-function-arguments-in-rust
- project generator
  - https://github.com/mainmatter/gerust

### macros
- https://veykril.github.io/tlborm/

## rust and python
- https://pyo3.rs/v0.21.2/


## toolchain

- https://github.com/Canop/bacon
- multi project build with workspaces https://doc.rust-lang.org/book/ch14-03-cargo-workspaces.html
- optimize build config https://github.com/Kobzol/cargo-wizard
- `cargo-watch` with `cargo watch -x check`
- sort cargo dependencies https://github.com/DevinR528/cargo-sort
- releasese
  - https://github.com/MarcoIeni/release-plz
  - example https://github.com/deepcausality-rs/deep_causality
 
### cross compilation

- https://burgers.io/cross-compile-rust-from-arm-to-x86-64
- https://github.com/rust-cross/cargo-zigbuild
- https://github.com/cross-rs/cross
- https://github.com/messense/homebrew-macos-cross-toolchains
- https://github.com/clux/muslrust/issues/142#issuecomment-2152638811

### static builds

> In the case of MUSL ensure to:
> - use an alternative allocator such as mimalloc by patching MSUL
> - or directly compile it together (may be simpler for bazel) https://github.com/linkerd/linkerd2/commit/aaa6091ea86eb988e68eda16bdc9b59db9d96076#diff-63a2e5c64764a441fcbc73dc27b1a8e684df057ffd54ad39e66e2a643020eb0d

### scaling the build beyond cargo

- https://mmapped.blog/posts/17-scaling-rust-builds-with-bazel
- https://users.rust-lang.org/t/static-linking-for-rust-without-glibc-scratch-image/112279/8
- https://github.com/marvin-hansen/fluvio-examples and https://github.com/deepcausality-rs/deep_causality
- faster linker
  - https://blog.rust.careers/post/compile_rust_faster/

### ci-cd examples

- https://gist.github.com/FedericoPonzi/873aea22b652572f5995f23b86543fdb
- https://github.com/f2calv/multi-arch-container-rust
- https://blog.urth.org/2023/03/05/cross-compiling-rust-projects-in-github-actions/
- https://github.com/dirien/rust-cross-compile

  
### dependencies
- https://www.lurklurk.org/effective-rust/dep-graph.html cargo-udeps/cargo-deny
- sbom
  - https://github.com/rust-secure-code/cargo-auditable
  - https://github.com/CycloneDX/cyclonedx-rust-cargo/

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
- semver https://github.com/obi1kenobi/cargo-semver-checks
- `cargo-udeps` to delete unused dependencies

### databases & ORM

- https://github.com/launchbadge/sqlx

### testing

- https://github.com/la10736/rstest
- https://github.com/rust-lang/miri
- https://github.com/rust-fuzz/cargo-fuzz
- https://github.com/obi1kenobi/cargo-semver-checks
- https://crates.io/crates/criterion
- https://nexte.st/
- coverage
  - https://docs.rs/cargo-tarpaulin/latest/cargo_tarpaulin/ `cargo install cargo-tarpaulin` ` cargo tarpaulin --ignore-tests`
- fuzzer
  - grammar
    - https://github.com/R9295/autarkie
 
#### mocking
- https://docs.rs/mockall/latest/mockall/

## learnings

### macros

- automatically derive macros i.e. for equality https://rust-exercises.com/04_traits/04_derive
  ```
  #[derive(PartialEq)]
  ```
- https://docs.rs/derive_more/latest/derive_more/

### architecture in rust

- https://alexis-lozano.com/hexagonal-architecture-in-rust-1/
- project plan for successful rust https://corrode.dev/blog/successful-rust-business-adoption-checklist/

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
- https://github.com/hyperium/tonic and https://github.com/actix/actix-web/issues/2853

### web utils (built with rust)

- https://exograph.dev/

### template engines

- https://github.com/djc/askama
  
### security

(not only rust specific)

- https://owasp.org/www-project-application-security-verification-standard/
- https://cheatsheetseries.owasp.org/cheatsheets/Password_Storage_Cheat_Sheet.html

#### security-web

- authorization
  - https://github.com/resyncgg/dacquiri
  - https://github.com/authzed/spicedb
  - acticx RBAC https://github.com/casbin/casbin-rs and https://github.com/casbin-rs/actix-casbin
- request validation
  - https://github.com/ranger-ross/actix-web-validation
- tools https://github.com/osirislab/awesome-rust-security/blob/master/README.md

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
- language models
  - https://docs.rs/kalosm/latest/kalosm/
### data engineering and rust

- https://blog.duyet.net/2023/06/fossil-data-platform-written-rust.html
- https://rustfordata.com/chapter_1.html
## embedded

- https://github.com/rust-embedded/rust-raspberrypi-OS-tutorials

## artifact handling

- https://github.com/cenotelie/cratery

## logging & observability

- https://signoz.io/

### profiling
- https://github.com/tikv/pprof-rs

## frameworks

- actor
  - https://github.com/elfo-rs/elfo


## verification

- https://github.com/verus-lang/verus


## learning steps

explore

- https://github.com/howtocodeit/hexarch
- https://doc.rust-lang.org/book/ch14-03-cargo-workspaces.html
- https://leptos.dev/
- https://github.com/leptos-rs/leptos/tree/main/examples/tailwind_actix
- https://github.com/bazelbuild/examples/tree/main/rust-examples#examples-to-build-rust-code
