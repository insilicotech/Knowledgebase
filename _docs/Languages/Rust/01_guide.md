---
title: "Guide of Rust"
permalink: /docs/languages/Rust/Introduction
excerpt: ""
last_modified_at: 2018-01-02T16:28:04-05:00
toc: false
---

```bash
$ apm install language-rust
$ apm install ide-rust
```

```bash
curl -L https://sh.rustup.rs | sh -s -- -y --default-toolchain=nightly
source ~/.cargo/env
rustup target add asmjs-unknown-emscripten
rustup target add wasm32-unknown-emscripten
```

## Lifetime

In Go, you can do this

```go
func example_function() *int {
  b := 3;
  return &b
}

func main() {
  fmt.Println(*example_function());
}
```

However, you can not do that in Rust:

```rust
fn example_function<'a>() -> &'a i32 {
    let b = 3;
    &b
}

fn main() {
  println!("{}", example_function());
}
```

Why is this important? Because this is what happend in C:

```c
int* example_function() {
  int a = 2;
  return &a;
}

void do_something(int b) {

}

int main(void){
  int *c = example_function();
  do_something()
  int d = 4;
  printf("%i\n", *c);
}
```

In C this is Undefined Behavior. When I run this, it just prints “3”.But Rust prevents crazy things like that from taking place!

## Reference

### Official sites

-   [official pacakges repository](https://crates.io/)

### Guide

-   [Unofficial Patterns](https://github.com/rust-unofficial/patterns)
-   [Learning Rust: Too many lists](http://cglab.ca/~abeinges/blah/too-many-lists/book/)

    ### Awesome Rust

-   [awesome-rust](https://github.com/rust-unofficial/awesome-rust)
-   [aswsome-embeded-rust](https://github.com/berkus/awesome-embedded-rust)
-   [rust-libhunt](https://rust.libhunt.com/)

### Utilities

-   [xsv](https://github.com/BurntSushi/xsv)
-   [ripgrep](https://github.com/BurntSushi/ripgrep)

### Libraries

-   [csv reader/writer](https://github.com/BurntSushi/rust-csv)
-   [serde](https://github.com/serde-rs/serde)

### Workflow

-   [Rust workflow by usingı VSCode](https://mobiarch.wordpress.com/category/rust/)

### Blogs

-   [Julai Evans](https://jvns.ca/)

### github

- [Steve Klabnik](https://github.com/steveklabnik)

### Database

- [Rust <-> SQL Server](https://github.com/steffengy/tiberius)
