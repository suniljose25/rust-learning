## Cargo
Cargo is rust's build system.

Create a new rust project with Cargo using the following command
`cargo new hello_cargo`

By default it create a binary project.

There are two types of projects that cargo can initilize.
1. Binary Project - A project where the output of the project is a binary.
2. Library Project - A project which does not give a binary output and instead is used as a library.

When cargo initializes a rust project, it creates a toml Cargo.toml file which contains the information about the project and also it's dependencies.

### Build a Rust project with Cargo
The following command is used to build a rust project with cargo
`cargo build`

This by default build the rust project in unoptimized development/debug mode which is relatively fast.
It produces a target folder withing which the build files as well as the final binary file is produced.

### Running a Rust project with Cargo
The following command is used to build and run the rust project with cargo.
`cargo run`

This command is the same as the `build` command with the extra step of running the executable after building it.

### Only check the project without building the project?
The `cargo check` command will only check the project for errors and warnings with actually building the project. This is much faster way of getting a feedback from the compiler about any issues instead of building the project with takes time.

### Ready for production? Then build for production...
The rust cargo project can be built with all the optimizations for the production using the command `cargo build --release`.

This flag is only used when we are deploying the application as the build time is very high.

### Clean up build files?
Use `cargo clean` to remove all build releated files.
