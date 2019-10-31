# python-indent-parser

[![Build Status](https://travis-ci.com/DSpeckhals/python-indent-parser.svg?branch=master)](https://travis-ci.com/DSpeckhals/python-indent-parser)

This package is the base parser for Atom's [python-indent](https://github.com/DSpeckhals/python-indent)
package to better handle Python indentation after a new line.

### Indent Types
Both indent types for continuing lines as described in
[PEP 0008 -- Style Guide for Python Code](https://www.python.org/dev/peps/pep-0008/#indentation)
are auto-detected and applied by this package.

  - Aligned with Opening Delimiter

    ```python
    def function_with_lots_of_params(param_1, param_2,
                                     param_3, param_4,
                                     very_long_parameter_name,
                                     param_6)
    ```
  - Hanging

      ```python
      def function_with_lots_of_params(
          param_1, param_2,
          param_3, param_4,
          very_long_parameter_name,
          param_6)
      ```
