# React-Coding-Standards-and-Practices

Reference: 
https://medium.com/@navitasinghal77/react-coding-standards-and-practices-3b133bcaea8


## Naming Conventions

1. React UI component’s names should be PascalCase.

```bash
Example: LoginScreen.js
```

2. All other helper files should be camelCase. (non-component files)

```bash
Example: commonUtils.js
```


3. All the folder names should be camelCase. 

```bash
Example: components
```

4. CSS files should be named the same as the component PascalCase. Global CSS which applies to all components should be placed in global.css and should be named in camelCase.

```bash
Example: LoginScreen.css(for components), global.css(for global styles)
```

5. Test files should be named the same as the component or non-component file.

```bash
Example: LoginScreen.test.js
```

## Some Best Practices for Clean Code

1. Use the DRY principle (Don't repeat yourself).

2. Create multiple files instead of writing a big file. (Componentization of code: fix to small functionality for each file).

3. Avoid Inline CSS when possible.

4. Use a linter to make your code easier to review. Follow strict linting rules. This in turn helps you write clean, consistent code.

5. Split your code into multiple smaller functions. Each with a single responsibility.

6. Separate all your service calls into a separate file. If it’s a big project try to split the services into multiple files. (name convention module_name.service.js).

7. Always write test cases for your code. Keep tests files in sync with the files they are testing.

8. Destructuring your props is a good way to help make your coder cleaner and more maintainable.








