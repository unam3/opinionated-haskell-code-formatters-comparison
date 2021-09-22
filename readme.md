# Haskell code formatters opinionated comparison

Scoped formatters:

- brittany 0.13.1.2
- hindent 5.3.1
- ormolu 0.1.4.1
- fourmolu 0.3.0.0
- stylish-haskell 0.12.2.0


## Methodology
Original source file will be processed by code formatter with default options and then with options to address my personal needs.


## hindent

- [doesn't preserve newlines](https://github.com/unam3/opinionated-haskell-code-formatters-comparison/commit/bdd64cc8d1791434316d4204897693dd78c9e711#diff-f163797eb9bf32d5a19d13bcb576de2cad6f0d4965f20b42e6b838436d21118aL57-R104)
- [splits creation of value with records into several lines](https://github.com/unam3/opinionated-haskell-code-formatters-comparison/commit/bdd64cc8d1791434316d4204897693dd78c9e711#diff-f163797eb9bf32d5a19d13bcb576de2cad6f0d4965f20b42e6b838436d21118aR131-R136)
- [doesn't align comments](https://github.com/unam3/opinionated-haskell-code-formatters-comparison/commit/bdd64cc8d1791434316d4204897693dd78c9e711#diff-f163797eb9bf32d5a19d13bcb576de2cad6f0d4965f20b42e6b838436d21118aR160-R163)
- [unnecessary newline after `->`](https://github.com/unam3/opinionated-haskell-code-formatters-comparison/commit/bdd64cc8d1791434316d4204897693dd78c9e711#diff-f163797eb9bf32d5a19d13bcb576de2cad6f0d4965f20b42e6b838436d21118aR165-R166)
- [giant function arguments definition-oneliner](https://github.com/unam3/opinionated-haskell-code-formatters-comparison/commit/bdd64cc8d1791434316d4204897693dd78c9e711#diff-f163797eb9bf32d5a19d13bcb576de2cad6f0d4965f20b42e6b838436d21118aR185) and [original one](https://github.com/unam3/opinionated-haskell-code-formatters-comparison/commit/bdd64cc8d1791434316d4204897693dd78c9e711#diff-f163797eb9bf32d5a19d13bcb576de2cad6f0d4965f20b42e6b838436d21118aL162-L175)
- [removes double newlines](https://github.com/unam3/opinionated-haskell-code-formatters-comparison/commit/bdd64cc8d1791434316d4204897693dd78c9e711#diff-f163797eb9bf32d5a19d13bcb576de2cad6f0d4965f20b42e6b838436d21118aL225-L226)
- [dangling operators if line overflows (bigger than --line-length value) and unpadded chained expressions](https://github.com/unam3/opinionated-haskell-code-formatters-comparison/commit/bdd64cc8d1791434316d4204897693dd78c9e711#diff-f163797eb9bf32d5a19d13bcb576de2cad6f0d4965f20b42e6b838436d21118aL240-R242)
- [doesn't preserve indentation of operators in multiline expressions](https://github.com/unam3/opinionated-haskell-code-formatters-comparison/commit/bdd64cc8d1791434316d4204897693dd78c9e711#diff-f163797eb9bf32d5a19d13bcb576de2cad6f0d4965f20b42e6b838436d21118aL239-R242)
- [removes space between `\` and argument name in lambda](https://github.com/unam3/opinionated-haskell-code-formatters-comparison/commit/bdd64cc8d1791434316d4204897693dd78c9e711#diff-f163797eb9bf32d5a19d13bcb576de2cad6f0d4965f20b42e6b838436d21118aL278-R284)
- [one space indent despite all other indentation cases in brackets on newline](https://github.com/unam3/opinionated-haskell-code-formatters-comparison/commit/bdd64cc8d1791434316d4204897693dd78c9e711#diff-f163797eb9bf32d5a19d13bcb576de2cad6f0d4965f20b42e6b838436d21118aR296-R297)
- [groups several lines into one](https://github.com/unam3/opinionated-haskell-code-formatters-comparison/commit/8ea2812fb3a11d7a7b8a4dda91810029fb2ba9fd#diff-f163797eb9bf32d5a19d13bcb576de2cad6f0d4965f20b42e6b838436d21118aR167) and [original](https://github.com/unam3/opinionated-haskell-code-formatters-comparison/commit/8ea2812fb3a11d7a7b8a4dda91810029fb2ba9fd#diff-f163797eb9bf32d5a19d13bcb576de2cad6f0d4965f20b42e6b838436d21118aL193-L194)


## ormolu

- [doesn't preserve import groups](https://github.com/unam3/opinionated-haskell-code-formatters-comparison/commit/c1ee9704a1ec5ad6c4c1940545618d744e5cf03e#diff-f163797eb9bf32d5a19d13bcb576de2cad6f0d4965f20b42e6b838436d21118aL12-L41)
- [puts Prelude import at the end from other modules](https://github.com/unam3/opinionated-haskell-code-formatters-comparison/commit/c1ee9704a1ec5ad6c4c1940545618d744e5cf03e#diff-f163797eb9bf32d5a19d13bcb576de2cad6f0d4965f20b42e6b838436d21118aR43)
- [dangling `->` in type annotations](https://github.com/unam3/opinionated-haskell-code-formatters-comparison/commit/c1ee9704a1ec5ad6c4c1940545618d744e5cf03e#diff-f163797eb9bf32d5a19d13bcb576de2cad6f0d4965f20b42e6b838436d21118aL51-R55)
- [doesn't preserve two empty lines](https://github.com/unam3/opinionated-haskell-code-formatters-comparison/commit/c1ee9704a1ec5ad6c4c1940545618d744e5cf03e#diff-f163797eb9bf32d5a19d13bcb576de2cad6f0d4965f20b42e6b838436d21118aL225-L226)
- [splits creation of value with records into several lines](https://github.com/unam3/opinionated-haskell-code-formatters-comparison/commit/c1ee9704a1ec5ad6c4c1940545618d744e5cf03e#diff-f163797eb9bf32d5a19d13bcb576de2cad6f0d4965f20b42e6b838436d21118aL105-R106)
- [doesn't preserve indentation of operators in multiline expressions](https://github.com/unam3/opinionated-haskell-code-formatters-comparison/commit/c1ee9704a1ec5ad6c4c1940545618d744e5cf03e#diff-f163797eb9bf32d5a19d13bcb576de2cad6f0d4965f20b42e6b838436d21118aL239-R246)

## fourmolu

- [dangling `->` in type annotations](https://github.com/unam3/opinionated-haskell-code-formatters-comparison/commit/8b3e8f17541d04d69fc29f9124640fbe58268696#diff-f163797eb9bf32d5a19d13bcb576de2cad6f0d4965f20b42e6b838436d21118aL51-R54)
- [unnecessary indentation of when after do (bug?)](https://github.com/unam3/opinionated-haskell-code-formatters-comparison/commit/8b3e8f17541d04d69fc29f9124640fbe58268696#diff-f163797eb9bf32d5a19d13bcb576de2cad6f0d4965f20b42e6b838436d21118aL139-R148)
- [splits creation of value with records into several lines](https://github.com/unam3/opinionated-haskell-code-formatters-comparison/commit/8b3e8f17541d04d69fc29f9124640fbe58268696#diff-f163797eb9bf32d5a19d13bcb576de2cad6f0d4965f20b42e6b838436d21118aL105-R106)
- [doesn't preserve indentation of operators in multiline expressions](https://github.com/unam3/opinionated-haskell-code-formatters-comparison/commit/8b3e8f17541d04d69fc29f9124640fbe58268696#diff-f163797eb9bf32d5a19d13bcb576de2cad6f0d4965f20b42e6b838436d21118aL242-R247)

## stylish-haskell

- [`list_padding: module_name` doesn't work bug?](https://github.com/unam3/opinionated-haskell-code-formatters-comparison/commit/68e769f416af0bb951e2e2409fae66b862f1414e#diff-f163797eb9bf32d5a19d13bcb576de2cad6f0d4965f20b42e6b838436d21118aL36-R37)
