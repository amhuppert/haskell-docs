Library API documentation is typically autogenerated from code comments, to create online interactive docs. For example, `gloss` is a package for 2D animation and games. [Here are its API docs](https://hackage.haskell.org/package/gloss), where you can find the following package list:

![Gloss on Hackage](/img/hackage.png)

For well-maintained packages, you should expect to find some explanation of the package's goals and uses either on this front page or in the top-level module (here `Graphics.Gloss`).

!!! Warning
    Many published packages are experimental code, not intended for serious use. To get a sense of which packages to use, see [this guide](https://github.com/Gabriella439/post-rfc/blob/main/sotu.md).

    In general, avoid packages if they have not been updated for a few years.

## How to read Haskell documentation

Haskell's expressive types are usually very helpful in understanding how to use a library. For example, the following function appears near the top of [the docs in the top level module](https://hackage.haskell.org/package/gloss-1.13.2.2/docs/Graphics-Gloss.html):

![Gloss docs](/img/gloss.png)

From the type signature, we see that we get a runnable process (i.e. a value of type `IO ()`) if we supply a few arguments, like `Color` and a function `#!haskell Float -> Picture`.

We can then understand what `Picture` is by following the link, to see its definition:

![Picture](/img/picture.png)

