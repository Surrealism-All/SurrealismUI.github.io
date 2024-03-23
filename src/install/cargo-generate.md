# Cargo-Generate

## 1. Install cargo-generate

you can use the following command to install cargo-generate

```bash
cargo install cargo-generate
```

## 2. generate your own project

**input your project name to replace `{project_name}`**

```bash
cargo generate --git https://github.com/Surrealism-All/surrealism-ui-template.git --name {project_name}
```

```bash
🔧   Destination: E:\Rust\test-surrealism ...
🔧   project-name: test-surrealism ...
🔧   Generating template ...
🔧   Moving generated files into: `E:\Rust\test-surrealism`...
🔧   Initializing a fresh Git repository
✨   Done! New project created E:\Rust\test-surrealism
```

## 3. run project

```bash
cargo run
```