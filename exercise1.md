The language I chose is Rust and the app we are building is a digital audio workstation deployed to the web (using WebAssembly technology). You can make music and edit sound files with effects, etc. using the app. Rust is a compiled language so the CI process might be more difficult than with something like Javascript.

Clippy will be used as the linter for the project, which is the official Rust linter. Clippy is a part of the Rust compiler, so it is easy to use, and it is also highly customizable, so we could make it suit well for our project.

For testing, we will use the Rust testing framework, which is also a part of the Rust compiler. The inbuilt testing framework is quite barebones so we might have to use a third-party testing framework if we need more features for testing sound things.

As for building, we will simply use the Rust compiler which handles everything.

Github Actions would probably be the best choice for CI since it is so popular. Since our tests might be processor intensive, we might need more CPU power on the CI server. However, Github Actions recently released more powerful servers with up to 64-cores of CPU and 256GB of RAM, which definitely should be enough for our project.
