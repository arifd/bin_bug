is this considered a bug? https://github.com/arifd/bin_bug

Basically, if i have bins in `src/bins/`  they can use `env!("CARGO_BIN_NAME")` but lib.rs can not ("error: environment variable `CARGO_BIN_NAME` not defined"). Thus I can't define a function in lib.rs which uses it and then have a bin call it

(...only bins will ever call it!)