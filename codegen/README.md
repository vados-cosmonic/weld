# Code generation from Smithy IDL models

Code generation is implemented in Rust, and output languages currently include Rust and Html (for documentation). We are expecting to add more languages in the future.

The code generator can be invoked:
- as a library
- from build.rs file: to build project sources according to a plan in [`codegen.toml`](https://wasmcloud.com/docs/hosts/abis/wasmbus/interfaces/codegen-toml)
- from the [`wash` cli](https://github.com/wasmcloud/wash)

Documentation on how the code generator works, how to use it with wasmCloud, and how to extend it, can be found in the [developer documentation](https://wasmcloud.com/docs/hosts/abis/wasmbus/interfaces/).

## Environment Variables

Here are some environment variables that control the operation of code generation:

| ENV variable           | Example | Description                                                 |
|------------------------|---------|-------------------------------------------------------------|
| `SMITHY_BINDGEN_DEBUG` | `true`  | If this is set to any value, debug messages will be printed |
