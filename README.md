# Practical JSX: Variables and Objects

A small React learning project that demonstrates how JavaScript variables, arrays, objects, conditional expressions, and mapped lists can be rendered in JSX. The example displays a Dragon Quest review using both standalone variables and properties from a review object.

## Why this project is useful

This project provides a focused example for developers learning to:

- Embed JavaScript values in JSX with curly-brace expressions.
- Render strings, numbers, and boolean values in a component.
- Use a ternary expression to display a readable value for a boolean.
- Render an array as a list with `.map()` and React keys.
- Read nested properties from a JavaScript object in a React component.

## Getting started

### Prerequisites

- Node.js and npm
- A browser that supports the development build

### Installation

1. Clone the repository and move into the project directory:

   ```bash
   git clone https://github.com/VoidLance/course-files-javascript-react-practical-jsx-variables-and-objects.git
   cd course-files-javascript-react-practical-jsx-variables-and-objects
   ```

2. Install the dependencies:

   ```bash
   npm install
   ```

3. Start the development server:

   ```bash
   npm start
   ```

4. Open [http://localhost:3000](http://localhost:3000) in your browser. The page reloads automatically as you edit the source files.

## Example

The main lesson is implemented in `src/DisplayVariables.js`. JSX can interpolate variables and object properties directly:

```jsx
const name = 'Dragon Quest';
const review = {
  title: 'Dragon Quest Review',
  score: 100,
  isAwesome: true,
};

return (
  <>
    <p>Name: {name}</p>
    <p>Title: {review.title}</p>
    <p>Score: {review.score}</p>
    <p>Is Awesome: {review.isAwesome ? 'Yes' : 'No'}</p>
  </>
);
```

The complete example also maps the `pros` array into an unordered list.

## Available commands

Run these commands from the project directory:

| Command | Description |
| --- | --- |
| `npm start` | Starts the development server. |
| `npm test` | Runs the test suite in interactive watch mode. |
| `npm run build` | Creates an optimized production build in `build/`. |
| `npm run eject` | Exposes the Create React App configuration. This is irreversible and usually unnecessary. |

## Project structure

```text
src/
├── App.js                 # Root component
├── DisplayVariables.js    # JSX variables and objects example
├── App.test.js            # Component test
├── index.js               # Application entry point
└── *.css                  # Application styles
public/                    # Static assets and HTML shell
```

## Getting help

For questions about this example:

- Open an [issue](https://github.com/VoidLance/course-files-javascript-react-practical-jsx-variables-and-objects/issues).
- Review the [React documentation](https://react.dev/learn).
- Review the [Create React App documentation](https://create-react-app.dev/docs/getting-started/).

## Contributing

The project is maintained by [VoidLance](https://github.com/VoidLance). Contributions are welcome:

1. Fork the repository and create a focused branch.
2. Make your change and update related tests or documentation.
3. Run `npm test` and `npm run build`.
4. Open a pull request with a clear description of the change.

Keep examples focused on the JavaScript and JSX concepts demonstrated by this project.
