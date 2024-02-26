<!-- Copyright (C) 2023-2024 by Jinwen XU -->

# `cleveref-forward` — Forward-referencing functionality for cleveref

`cleveref-forward` aims at providing the forward-referencing functionality for the package `cleveref`.

> This package is derived from the package [`cleveref-usedon`](https://ctan.org/pkg/cleveref-usedon), with several fixes and enhancements.

> Package dependencies: [`cleveref`](https://ctan.org/pkg/cleveref), [*`crefthe`*](https://ctan.org/pkg/crefthe), [`iflang`](https://ctan.org/pkg/iflang), [`regexpatch`](https://ctan.org/pkg/regexpatch).

## Regarding the usage

It might be a good idea to start with the [demo documents](https://github.com/Jinwen-XU/cleveref-forward/tree/main/demo).

> The [documentation](http://mirrors.ctan.org/macros/latex/contrib/cleveref-usedon/cleveref-usedon.pdf) and [examples](https://github.com/SvenPistre/cleveref-usedon/tree/main/examples) written by Sven Pistre for the original package `cleveref-usedon` are also very inspiring (but be aware that the usage has changed a lot, so some of the code there may no longer work here).

## Known issues / what to do next

- This package currently works for English, French, German, Italian and Spanish — certainly more languages would be added to this list in the future.
- The code is somewhat messy for now, and the naming of many macros could be improved.
- The support for displayed maths is still not perfect: currently, if you choose to print the forward-referencing message outside the math environment, then for `equation`, `multline` and `dmath`, it works nicely (you may need to configure `cleveref` to make it work with `dmath`); but for `align`, `flalign`, `alignat` and `gather`, it would only show the message for the last labeled line. The inside-math mode has no such limitation, but it would require sufficient margin width.
- Not all configuration yields nice result, more appealing examples are needed.

The original package [`cleveref-usedon`](https://ctan.org/pkg/cleveref-usedon) is nicer in terms of documentation, while the current package is slightly more advanced in terms of code. It is hoped that one day they can be combined into a better version.


## Acknowledgement

The author would like to thank:

- Sven Pistre, for originally developing the nice package [`cleveref-usedon`](https://ctan.org/pkg/cleveref-usedon), and for the friendly discussions with him that inspired many of the modifications later.
- Ulrich Diez, for his help in a key step of the new configuration command.

## License

This work is released under the LaTeX Project Public License, v1.3c or later.
