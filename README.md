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

### 1. Use the DRY principle (Don't repeat yourself).

### 2. Create multiple files instead of writing a big file. (Componentization of code: fix to small functionality for each file).

### 3. Avoid Inline CSS when possible.

### 4. Use a linter to make your code easier to review. Follow strict linting rules. This in turn helps you write clean, consistent code.

### 5. Split your code into multiple smaller functions. Each with a single responsibility.

### 6. Separate all your service calls into a separate file. If it’s a big project try to split the services into multiple files. (name convention module_name.service.js).

### 7. Always write test cases for your code. Keep tests files in sync with the files they are testing.

### 8. Destructuring your props is a good way to help make your coder cleaner and more maintainable.

### 9. Use Ternary Operators

```js
const { role } = user;

return role === ADMIN ? <AdminUser /> : <NormalUser />
```

### 10. Use React Fragments

Always use Fragment over Div. It keeps the code clean and is also beneficial for performance because one less node is created in the virtual DOM.

```js
return (
  <>
     <Component1 />
     <Component2 />
     <Component3 />
  </>  
)
```

### 11. Use Memo and Pure components

*React.PureComponent* and *UseMemo* can significantly improve the performance of your application. They help us to avoid unnecessary rendering.



### 12. Use Object Destructuring

Use object destructuring to your advantage. Let’s say you need to show a user’s details.

```js
const { name, age, profession } = user;

return (
  <>
    <div> {name} </div>
    <div> {age} </div>
    <div> {profession} </div>
  </>  
)
```

### 13. Use Template Literals

Use template literals to build large strings. Avoid using string concatenation. It’s nice and clean.


```js

const userDetails = `${user.name}'s profession is ${user.proffession}`

return (
  <div> {userDetails} </div>  
)
```

### 14. Quotes

Use double quotes for JSX attributes and single quotes for all other JS.


### 15. Prop Naming

Always use camelCase for prop names or PascalCase if the prop value is a React component.

```js
<MyComponent
  userName="hello"
  phoneNumber={12345678}
  Component={SomeComponent}
/>
```


### 16. JSX in Parentheses

If your component spans more than one line, always wrap it in parentheses.

```jsx
return (
    <MyComponent variant="long">
      <MyChild />
    </MyComponent>
);
```