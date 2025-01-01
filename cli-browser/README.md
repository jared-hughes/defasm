# DefAssembler - Command-line Utility

This package is a bastardized version of @defasm/cli. It removes all of the CLI and file manipulation stuff. All that's left is a way to assemble into ELF executables or object files. The two functions are `createExecutable` and `createObject`. Their sole parameter is an `AssemblyState` as obtained from @defasm/core. The return value is a `Buffer` object, which is an instance of a `Uint8Array` with an extended prototype.

This package is not stable -- just a prototype test for the purpose of [DefCPU](https://github.com/jared-hughes/defcpu). Plan is to eventually bring this into the real @defasm/core and point @defasm/cli towards that.
