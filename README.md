<div align="center">
  <p>
    <a href="https://mruby.org/">
      <img src="https://avatars.githubusercontent.com/u/1796512?s=200&v=4"
        alt="The mruby programming language" title="mruby">
    </a>
  </p>
  <h1>mruby</h1>
  <a href="https://github.com/marketplace/actions/super-linter">
    <img src="https://github.com/mruby/mruby/workflows/Lint%20Code%20Base/badge.svg"
      alt="GitHub Super-Linter">
  </a>
</div>

## What is mruby

mruby is the lightweight implementation of the Ruby language complying to (part
of) the [ISO standard][ISO-standard] with more recent features provided by Ruby 3.x.
Also, its syntax is Ruby 3.x compatible except for pattern matching.

You can link and embed mruby within your application. The "mruby" interpreter
program and the interactive "mirb" shell are provided as examples. You can also
compile Ruby programs into compiled byte code using the "mrbc" compiler. All
these tools are located in the "bin" directory. "mrbc" can also generate
compiled byte code in a C source file. See the "mrbtest" program under the
"test" directory for an example.

This achievement was sponsored by the Regional Innovation Creation R&D Programs
of the Ministry of Economy, Trade and Industry of Japan.

## How to get mruby

To get mruby, you can download the stable version 3.2.0 from the official mruby
GitHub repository or clone the trunk of the mruby source tree with the "git
clone" command. You can also install and compile mruby using [ruby-install](https://github.com/postmodern/ruby-install), [ruby-build](https://github.com/rbenv/ruby-build) or [rvm](https://github.com/rvm/rvm).

The stable version 3.2.0 of mruby can be downloaded via the following URL: [https://github.com/mruby/mruby/archive/3.2.0.zip](https://github.com/mruby/mruby/archive/3.2.0.zip)

The latest development version of mruby can be downloaded via the following URL: [https://github.com/mruby/mruby/zipball/master](https://github.com/mruby/mruby/zipball/master)

The trunk of the mruby source tree can be checked out with the
following command:

```console
$ git clone https://github.com/mruby/mruby.git
```

## mruby homepage

The URL of the mruby homepage is: <https://mruby.org>.

## Mailing list

We don't have a mailing list, but you can use [GitHub issues](https://github.com/mruby/mruby/issues).

## How to compile, test, and install (mruby and gems)

For the simplest case, type

```console
rake all test
```

See the [compile.md](doc/guides/compile.md) file for the detail.

## Building documentation

There are two sets of documentation in mruby: the mruby API (generated by YARD) and C API (Doxygen and Graphviz)

To build both of them, simply go

```console
rake doc
```

You can also view them in your browser

```console
rake view_api
rake view_capi
```

## How to customize mruby (mrbgems)

mruby contains a package manager called "mrbgems" that you can use to create
extensions in C and/or Ruby. For a guide on how to use mrbgems, consult the
[mrbgems.md](doc/guides/mrbgems.md) file, and for example code, refer to the
[examples/mrbgems/](examples/mrbgems) folder.

## License

mruby is released under the [MIT License](LICENSE).

## Note for License

mruby has chosen a MIT License due to its permissive license allowing
developers to target various environments such as embedded systems.
However, the license requires the display of the copyright notice and license
information in manuals for instance. Doing so for big projects can be
complicated or troublesome. This is why mruby has decided to display "mruby
developers" as the copyright name to make it simple conventionally.
In the future, mruby might ask you to distribute your new code
(that you will commit,) under the MIT License as a member of
"mruby developers" but contributors will keep their copyright.
(We did not intend for contributors to transfer or waive their copyrights,
actual copyright holder name (contributors) will be listed in the [AUTHORS](AUTHORS)
file.)

Please ask us if you want to distribute your code under another license.

## How to Contribute

To contribute to mruby, please refer to the [contribution guidelines][contribution-guidelines] and send a pull request to the [mruby GitHub repository](https://github.com/mruby/mruby).
By contributing, you grant non-exclusive rights to your code under the MIT License.

[ISO-standard]: https://www.iso.org/iso/iso_catalogue/catalogue_tc/catalogue_detail.htm?csnumber=59579
[contribution-guidelines]: https://github.com/mruby/mruby/blob/master/CONTRIBUTING.md
