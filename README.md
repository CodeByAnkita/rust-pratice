# Rust Practice

This repository is a collection of exercises, projects, and activities designed to help you learn the Rust programming language. It includes various activities, a sample project (`ClipStash`), and related solutions to enhance your Rust programming skills.

---

## Activities

The `activities` directory contains hands-on exercises to help you practice Rust concepts.

### How to Run Activities
1. Open your editor/IDE to the `activities` directory.
2. Use the following command to run a specific activity:
   ```bash
   cargo run --bin a1
   ```
   Replace `a1` with the name of the activity file you want to execute.

---

## ClipStash Project

The `clipstash` directory contains the `ClipStash` project, which is a practical example of applying Rust concepts in a real-world scenario.

### Commands for Working with `ClipStash`
- To check the project code:
  ```bash
  cargo check
  ```
- To test the project:
  ```bash
  cargo test
  ```
- To run specific binaries within the project:
  ```bash
  cargo run --bin <name>
  ```
  Replace `<name>` with the name of the binary you wish to run.

### Resolving Compilation Errors
If you encounter errors related to `rocket::response::content::Html` or `rocket::response::content::RawHtml`, update specific dependencies using these commands:
```bash
cargo update --package rocket --precise 0.5.0-rc.1
cargo update --package rocket_codegen --precise 0.5.0-rc.1
cargo update --package rocket_http --precise 0.5.0-rc.1
```

---

## Setting Up the Database for `ClipStash`

To build and configure the database for the `ClipStash` project, follow these steps:

1. Install the `sqlx-cli` tool:
   ```bash
   cargo install sqlx-cli
   ```
2. Set up the database:
   ```bash
   sqlx database setup
   ```

---

## Solutions

Solutions to activities and the `ClipStash` project are available in the `solutions` branch. To access them, switch to the solutions branch using:
```bash
git checkout solutions
```

---

## Additional Notes

- Ensure you have the Rust toolchain installed. If not, you can install it using:
  ```bash
  rustup default stable
  ```
- Use the `cargo` commands above to build, run, and test projects efficiently.

---

Happy Coding! 🚀
