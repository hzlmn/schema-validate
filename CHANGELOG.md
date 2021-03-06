[1.0.0]

  - Added `flow` type annotations
  - Added `jest` for tests
  - Added API docs

  - Added feature for passing validators as `Array`
    
    Example
    ```js
    const Schema = {
      value: ['string', customValidator]
    }
    ```

  - Added aliases for builtin validators
  
    `string`, `number`, `object`, `array`, `nullable`

    Aliases just a string reference to corresponding validator function

[1.0.1]

  - Minor doc improvements

[1.0.2]

  - Changed `validator` api
    
    * validators should return `null` if validation passed and `Error` object if validation failed

  - Validators are now chainable. You can use it like `arrayOf(string).required`
