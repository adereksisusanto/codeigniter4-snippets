### Alternate Snippets for Controllers

### `[ProjectRoot]/app/Controllers/*.php`

### Table of Content

- [Controllers](#controllers) [new]
- [Controller Resources](#controller-resources) [new]

#### Controllers

- Command
  ```code
  ci4:controller
  ```
- Output
  ```php
  public function index()
  {
      // code
  }
  ```

#### Controller Resources

- Command
  ```code
  ci4:controller:resources
  ```
- Output

  ```php
  public function __construct()
  {
      // __construct code
  }

  public function index()
  {
      // index code
  }

  public function create()
  {
      // create code
  }

  public function read($id)
  {
      // read code
  }

  public function update($id)
  {
      // update code
  }

  public function delete($id)
  {
      // delete code
  }
  ```
