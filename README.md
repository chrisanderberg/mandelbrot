# Mandelbrot

My derivative version of the Mandelbrot set example presented in “Programming Rust by Jim Blandy and Jason Orendorff (O’Reilly). Copyright 2018 Jim Blandy and Jason Orendorff, 978-1-491-92728-1.”

Before learning Rust, I've actually implemented 3 previous Mandelbrot set renderers in Python, Scala, and C. I was pleasantly surprised to see "Programming Rust" used the Mandelbrot set as an intro to Rust's concurrency. Since I was already familiar with the problem, I could just focus on the language concepts.

## Todo

In addition to the example, I'll be implementing some of the features my previous Mandelbrot projects included such as coloration. The Mandelbrot set is infinitely elaborate, and tightening the interaction loop so that it's faster to adjust parameters and to see a new result will make it easier to explore the set for visually interesting features.

## Getting Started

To try out the code and render some fractals, you'll need all the prerequisites. Once that's done you can clone this repo and use the typical cargo commands to test, build and run.

### Prerequisites

The following prerequisites need to be installed before building and running the code.

* [Rust](https://www.rust-lang.org/tools/install) - using rustup is easiest
* [Git](https://git-scm.com/downloads) - it may be better to install Git using using your distro's repositories if you use Linux, or install the Xcode Command Line Tools if you're using a Mac. If you're using Windows, you may try [Git for Windows](https://gitforwindows.org/) or install if via [Chocolately](https://chocolatey.org/packages/git) if that's your tool of choice.

### Installing

First clone this repo:
```
git clone git@github.com:chrisanderberg/mandelbrot.git
```

Then build the project:
```
cargo build --release
```

Finally you can run it. The arguments shown here are the arguments used in the example from the "Progamming Rust" book.
```
target/release/mandelbrot mandel.png 4000x3000 -1.20,0.35 -1,0.20
```

## Running the tests

Tests are run in Rust's conventional way.

```
cargo test
```

## Authors

* **[Chris Anderberg](https://github.com/chrisanderberg)**


## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* **[Jim Blandy](https://github.com/jimblandy)** - for co-authoring the very useful ["Programming Rust"](https://www.oreilly.com/library/view/programming-rust/9781491927274/) book and [original code](https://github.com/ProgrammingRust/mandelbrot) from which this project is derived
* **[Jason Orendorff](https://github.com/jimblandy)** - for co-authoring the very useful ["Programming Rust"](https://www.oreilly.com/library/view/programming-rust/9781491927274/) book and [original code](https://github.com/ProgrammingRust/mandelbrot) from which this project is derived
* **[Billie Thompson (PurpleBooth)](https://github.com/PurpleBooth)** - for an awesome [README template](https://gist.github.com/PurpleBooth/109311bb0361f32d87a2)

