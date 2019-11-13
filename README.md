# python-indent-parser

[![Build Status](https://travis-ci.com/DSpeckhals/python-indent-parser.svg?branch=master)](https://travis-ci.com/DSpeckhals/python-indent-parser)

This package is the base parser for the following text editor packages:
- Atom [python-indent](https://github.com/DSpeckhals/python-indent)
- VS Code [vsc-python-indent](https://github.com/kbrose/vsc-python-indent)

It helps the editor to automatically indent in typical Python fashion after new line events.

## Indent Types
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

## Contributing

1. [Fork this repository](https://github.com/DSpeckhals/python-indent-parser)

2. Clone your forked repository and create a new feature branch.

`git clone https://github.com/<you>/python-indent-parser`

3. Install the dependencies

`npm install`

4. Contribute

5. Make sure that all tests pass.

`npm run test`

6. Lint and correct as necessary.

`npm run lint`

7. Push your changes and create a pull request.

8. After a PR has been merged, and if you help maintain the package, run the following.

```sh
npm version <patch|minor|major>
npm publish
```

