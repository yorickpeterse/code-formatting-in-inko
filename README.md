# Code formatting in Inko

This repository showcases a basic code formatter written in [Inko](https://inko-lang.org/),
based on Inko's own code formatting implementation, which in turn is based on
[Prettier](https://prettier.io), which in turn is based on the paper
["A prettier printer"](https://homepages.inf.ed.ac.uk/wadler/papers/prettier/prettier.pdf)
by Philip Wadler.

The implementation is well documented, and prior knowledge of Inko shouldn't be
needed.

# Requirements

- Inko 0.15.0 or newer

# Usage

Using Inko 0.15.0 or newer, run the program like so, where `WIDTH` is the
desired line width:

```bash
inko run src/main.inko WIDTH
```

If you don't have or don't want to install Inko, you can also use Docker/Podman:

```bash
# When using Docker:
docker run --rm --volume ./src:/src:z ghcr.io/inko-lang/inko:latest inko run /src/main.inko WIDTH

# When using Podman:
podman run --rm --volume ./src:/src:z ghcr.io/inko-lang/inko:latest inko run /src/main.inko WIDTH
```

The output should be something along the lines of the following:

![A screenshot of the expected output](https://github.com/yorickpeterse/code-formatting-in-inko/assets/86065/9225eabf-6052-4ea3-9268-db160383a364)

The vertical grey line indicates the line limit.

# License

The code in this repository is licensed under the
[Unlicense](https://unlicense.org/). A copy of this license can be found in the
file "LICENSE".
