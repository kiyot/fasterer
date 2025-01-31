# Changelog

## 0.8.0

- Dropped support for ruby versions below 2.2.0 and locks ruby_parser to be above or equal to 1.14.1. The new ruby_parser version 1.14.1 explicitly [requires ruby versions above 2.2.0](https://github.com/seattlerb/ruby_parser/issues/298#issuecomment-539795933), so this affects fasterer as well.

## 0.7.1

- Fix `check_symbol_to_proc` rule from crashing when there is no receiver [#67](https://github.com/DamirSvrtan/fasterer/pull/67)

## 0.7.0

- More inclusive `check_symbol_to_proc` rule - don't only look at #each but any method that could leverage the symbol to proc rule. Merged through [#41](https://github.com/DamirSvrtan/fasterer/pull/41)

## 0.6.0

- Enable placing the `.fasterer.yml` file not just in the current dir, but in any parent directory as well.

## 0.5.1

- Upgrade to ruby_parser 3.13.0 that fully supports Ruby 2.6

## 0.5.0

- New style of outputting offenses: `spec/support/output/sample_code.rb:1 For loop is slower than using each.`

## 0.4.1
- Upgrade ruby parser version to 3.11.0 (to stop warnings)

## 0.4.0
- Better error message on each_key
- Update Ruby Parser to ~> 3.9
- Support Ruby 2.3
