# BoilerPlate React Vite

BoilerPlate React Vite Build Tool System and having configuration of Husky, Prettier, ESLint and TypeScript.

# Use Case

-   You don't need to waste your time to install specific packages but instead just fork the repo or download this into your system and just plug and play.

# Packages

-   **Husky** is a tool used in software development that enables the implementation of pre-commit and pre-push hooks in a Git repository. Hooks are scripts that run automatically at key points in the Git workflow, such as before committing or pushing changes. Husky allows developers to enforce certain checks and tasks before allowing commits or pushes, ensuring code quality and adherence to project-specific standards. Common use cases include running linters, formatting code, or executing tests before changes are committed or pushed to the repository.
-   **Prettier** is a code formatting tool that automatically analyzes and rewrites code to ensure consistent styling across a codebase. It supports multiple programming languages, including JavaScript, TypeScript, HTML, CSS, and more. Prettier helps maintain a standardized and readable code style by automatically applying formatting rules, such as indentation, line breaks, and spacing. Developers can define or customize these rules based on project preferences. By integrating Prettier into a development workflow, teams can reduce debates over code formatting, enhance code review processes, and maintain a more consistent and visually appealing codebase.
-   **ESLint** is a static code analysis tool used to identify and fix problems in JavaScript code. It helps developers enforce coding standards, catch common errors, and maintain a consistent coding style across a project.
-   **TypeScript** is a superset of JavaScript that adds static typing to the language. It provides developers with the ability to define and enforce types for variables, function parameters, and return values, enhancing code quality and catching potential errors during development.

# React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

-   [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
-   [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type aware lint rules:

-   Configure the top-level `parserOptions` property like this:

```js
export default {
    // other rules...
    parserOptions: {
        ecmaVersion: "latest",
        sourceType: "module",
        project: ["./tsconfig.json", "./tsconfig.node.json"],
        tsconfigRootDir: __dirname,
    },
};
```

-   Replace `plugin:@typescript-eslint/recommended` to `plugin:@typescript-eslint/recommended-type-checked` or `plugin:@typescript-eslint/strict-type-checked`
-   Optionally add `plugin:@typescript-eslint/stylistic-type-checked`
-   Install [eslint-plugin-react](https://github.com/jsx-eslint/eslint-plugin-react) and add `plugin:react/recommended` & `plugin:react/jsx-runtime` to the `extends` list
