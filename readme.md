# Haskell code formatters opinionated comparison

Scoped formatters:

- brittany 0.13.1.2
- hindent 5.3.1
- ormolu 0.1.4.1
- stylish-haskell 0.12.2.0


## Methodology
Original source file will be processed by code formatter with default options and then with options to address my personal needs.

## hindent

- [doesn't preserve newlines](https://github.com/unam3/opinionated-haskell-code-formatters-comparison/commit/bdd64cc8d1791434316d4204897693dd78c9e711#diff-f163797eb9bf32d5a19d13bcb576de2cad6f0d4965f20b42e6b838436d21118aL57-R104)
- [doesn't align comments](https://github.com/unam3/opinionated-haskell-code-formatters-comparison/commit/bdd64cc8d1791434316d4204897693dd78c9e711#diff-f163797eb9bf32d5a19d13bcb576de2cad6f0d4965f20b42e6b838436d21118aR160-R163)
- [unnecessary newline after `->`](https://github.com/unam3/opinionated-haskell-code-formatters-comparison/commit/bdd64cc8d1791434316d4204897693dd78c9e711#diff-f163797eb9bf32d5a19d13bcb576de2cad6f0d4965f20b42e6b838436d21118aR165-R166)
- [giant function arguments definition-oneliner](https://github.com/unam3/opinionated-haskell-code-formatters-comparison/commit/bdd64cc8d1791434316d4204897693dd78c9e711#diff-f163797eb9bf32d5a19d13bcb576de2cad6f0d4965f20b42e6b838436d21118aR185) and [original one](https://github.com/unam3/opinionated-haskell-code-formatters-comparison/commit/bdd64cc8d1791434316d4204897693dd78c9e711#diff-f163797eb9bf32d5a19d13bcb576de2cad6f0d4965f20b42e6b838436d21118aL162-L175)
- [removes double newlines](https://github.com/unam3/opinionated-haskell-code-formatters-comparison/commit/bdd64cc8d1791434316d4204897693dd78c9e711#diff-f163797eb9bf32d5a19d13bcb576de2cad6f0d4965f20b42e6b838436d21118aL225-L226)
- [dangling operators and unpadded chained expressions](https://github.com/unam3/opinionated-haskell-code-formatters-comparison/commit/bdd64cc8d1791434316d4204897693dd78c9e711#diff-f163797eb9bf32d5a19d13bcb576de2cad6f0d4965f20b42e6b838436d21118aL240-R242)
- [removes space between `\` and argument name in lambda](https://github.com/unam3/opinionated-haskell-code-formatters-comparison/commit/bdd64cc8d1791434316d4204897693dd78c9e711#diff-f163797eb9bf32d5a19d13bcb576de2cad6f0d4965f20b42e6b838436d21118aL278-R284)
- [one space indent despite all other indentation cases in brackets on newline](https://github.com/unam3/opinionated-haskell-code-formatters-comparison/commit/bdd64cc8d1791434316d4204897693dd78c9e711#diff-f163797eb9bf32d5a19d13bcb576de2cad6f0d4965f20b42e6b838436d21118aR296-R297)
