# dotenvy-tauri

A fork of the [dotenvy](https://github.com/allan2/dotenvy) crate with a modified `dotenv!` macro that loads environment variables from a `.env` file one level above `CARGO_MANIFEST_DIR` in the directory tree.

This allows you to use the `dotenv!` macro in a Tauri project to load environment variables from the `.env` file in the project root, given the following project structure:

```plaintext
- project_root/
  - .env
  - src-tauri/
    - Cargo.toml
    - src/
      - main.rs
```
