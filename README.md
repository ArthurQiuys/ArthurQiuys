```rust
fn main() {
    let me = Person {
        name: "Arthur",
        role: "backend / systems engineer",
        loves: &["rust", "small tools", "reading source code"],
        learning: &["async runtimes", "compilers", "low-latency networking"],
        contact: "arthurqiuy@outlook.com",
    };

    println!("{me:#?}");
}

#[derive(Debug)]
struct Person {
    name: &'static str,
    role: &'static str,
    loves: &'static [&'static str],
    learning: &'static [&'static str],
    contact: &'static str,
}
```
