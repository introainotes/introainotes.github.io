These notes are based on CSC384: Introduction to Artificial Intelligence taught by [Kuldeep S. Meel](https://www.cs.toronto.edu/~meel/) in Winter 2024 (AY23/24 Semester 2).

## Contributing

This material is still under construction! Although most of the notes have been written up in Markdown, you will probably find several typos. If you do, please inform us under GitHub issues or submit a pull request with your fixes via GitHub.


To make any changes to this repo,

1. Fork this repo by clicking the "fork" button in the top right.
1. Make the changes you want and push them to your own forked copy of this repo.
   - The .md files for the lecture notes can be located under `/files/<lecture_name>.md`.
1. Go back to GitHub to creata a pull request to bring your changes into this repo.

## To run locally (not on GitHub Pages, to serve on your own computer)

1. Clone the repository and made updates as detailed above
1. Make sure you have ruby-dev, bundler, and nodejs installed: `sudo apt install ruby-dev ruby-bundler nodejs`
    * Note that nodeJS might have to be installed separately.
    * Note that the latest version of ruby may not be compatible; ruby version 2.7 may be needed.
1. Run `bundle clean` to clean up the directory (no need to run `--force`)
1. Run `bundle install` to install ruby dependencies. If you get errors, delete Gemfile.lock and try again.
1. Run `bundle exec jekyll serve` to generate the HTML and serve it from `localhost:4000` the local server will automatically rebuild and refresh the pages on change.

## Remarks about writing math equations in markdown

* Basic syntax for markdown can be found [here](https://www.markdownguide.org/basic-syntax/).
* Start and end math equations with `$$` **for both inline and display equations**.
    * To make a display equation, put one newline before the starting `$$` a newline after the ending `$$`.
* To convert the LaTeX algorithms to markdown algorithms, you may enclose the math statements with `$` symbols.
* `$~~~~~$` can be used to create spaces for alignment purposes.
* Avoid vertical bars `|` in any inline math equations (i.e., within a paragraph of text). Otherwise, the GitHub Markdown compiler will interpret it as a table cell element (see GitHub Markdown spec [here](https://github.github.com/gfm/)). Instead, use one of `\mid`, `\vert`, `\lvert`, or `\rvert` instead. For double bar lines, write `\|` instead of `||`.
* Remember to remove the `&` and `_/` symbols as well because they may cause the markdown parser to crash.
* If for some reason the parser cannot handle symbols inside the `$ math $` statements, so you have to add a `\` next to your symbols, i.e. (`\_` instead of `_`).

<!-- ## Acknowledgements

The handwritten notes were compiled into LaTeX by [Priyanka Golia](https://priyanka-golia.github.io), with help from students including [Ang Zheng Yong](https://github.com/arsatis), [Guo Yichao](https://github.com/gycc7253), Khiew Zhi Kai, and [Vincent Neo](https://github.com/tenvinc).

They were later compiled into Markdown by the teaching team of AY21/22 Semester 1, including [Gabriel Sim](https://github.com/GabrielSimbingyang), [Pang Zhanzhong](https://github.com/pangzhan27), [Priyanka Golia](https://priyanka-golia.github.io), and [Yang Suwei](https://github.com/swxsw). -->

