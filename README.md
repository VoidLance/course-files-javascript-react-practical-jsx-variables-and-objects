# Practical JSX: Variables and Objects

A small React learning project that demonstrates how JavaScript variables, arrays,
booleans, and objects can be rendered in JSX. The example presents a Dragon Quest
review and uses conditional rendering and `map()` to display its data.

## Why this project is useful

- Shows the difference between rendering standalone variables and object properties.
- Demonstrates JSX expressions such as `{name}` and `{review.title}`.
- Uses a ternary expression to turn a boolean into readable UI text.
- Uses `map()` to render an array as a list with React keys.
- Provides a minimal Create React App structure that is easy to modify while learning.

## Getting started

### Prerequisites

- Node.js and npm
- A browser and a code editor

### Install and run

From the project directory:

```bash
npm install
npm start
```

Open <http://localhost:3000> in a browser. The development server reloads when
source files change.

### Build for production

```bash
npm run build
```

The optimized application is written to `build/`.

## Example

The main example lives in [`src/DisplayVariables.js`](src/DisplayVariables.js).
To add another review item, update the `pros` array and render it with the
existing pattern:

```jsx
const pros = ['Great Story', 'Engaging Gameplay'];

<ul>
  {pros.map((pro, index) => (
    <li key={index}>{pro}</li>
  ))}
</ul>
```

The application entry point is [`src/App.js`](src/App.js), and React mounts it
from [`src/index.js`](src/index.js).

## Available commands

| Command | Purpose |
| --- | --- |
| `npm start` | Run the development server |
| `npm test` | Run the test runner |
| `npm run build` | Create a production build |
| `npm run eject` | Eject from Create React App (irreversible) |

## Getting help

For React concepts, see the [React documentation](https://react.dev/learn).
For project tooling, see the [Create React App documentation](https://create-react-app.dev/docs/getting-started/).
If you find a problem with this example, open an issue in the repository with
the command you ran and the relevant error output.

## Contributing

Contributions are welcome. Please:

1. Create a focused branch for your change.
2. Keep examples beginner-friendly and consistent with the existing React structure.
3. Run the relevant npm commands before submitting a pull request.
4. Describe what changed and how it was tested.

The project is maintained by [VoidLance](https://github.com/VoidLance).
Refer to the repository's issue tracker for open improvements and questions.

## License

This repository does not currently include a license file. Add or consult the
repository license before redistributing the project.
