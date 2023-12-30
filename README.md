# Project README

## What is NPM?
NPM (Node Package Manager) is the default package manager for Node.js, used for installing, managing, and sharing JavaScript packages.

## What is Parcel/Webpack? Why do we need it?
Parcel and Webpack are bundlers for web applications. They bundle and optimize assets like JavaScript, CSS, and images, streamlining the deployment process and improving performance.

## What is `.parcel-cache`?
`.parcel-cache` is a directory where Parcel stores cached data to speed up the build process. It can be safely deleted if needed.

## What is npx?
`npx` is a tool that comes with NPM, allowing you to run binaries from Node.js packages without installing them globally or locally.

## What is the difference between dependencies vs devDependencies?
`dependencies` are packages required for the application to run, while `devDependencies` are tools and libraries needed only during development.

## What is Tree Shaking?
Tree Shaking is a technique to eliminate dead (unused) code during the build process, reducing the size of the final bundle.

## What is Hot Module Replacement?
Hot Module Replacement (HMR) is a feature that replaces modules in the running application without a full page reload, allowing for faster development.

## List down your favourite 5 superpowers of Parcel and describe any 3 of them in your own words.
1. **Zero Configuration:** Parcel requires minimal setup.
2. **Automatic Asset Handling:** Handles various assets without explicit configuration.
3. **Fast Build Times:** Focuses on quick development and build iteration.

## What is `.gitignore`? What should we add and not add into it?
`.gitignore` specifies files and directories to be ignored by Git. Add files like build artifacts, logs, and dependencies. Don't add sensitive data like API keys.

## What is the difference between `package.json` and `package-lock.json`?
`package.json` lists project metadata and dependencies. `package-lock.json` stores the exact versions of dependencies to ensure reproducibility.

## Why should I not modify `package-lock.json`?
Avoid modifying `package-lock.json` manually. It's autogenerated and reflects the state of your `node_modules` directory.

## What is `node_modules`? Is it a good idea to push that on git?
`node_modules` is a directory where NPM stores project dependencies. It's not recommended to push it to Git due to its size; instead, include a `.gitignore` entry.

## What is the `dist` folder?
The `dist` (distribution) folder contains the optimized and bundled files ready for deployment.

## What is `browserlist`?
`browserslist` is a configuration file defining the target browsers for compatibility. It helps tools like Babel and Autoprefixer adjust output accordingly.

# Web Development Essentials

## Bundlers:

### 1. Vite
- **Description:** Vite is a build tool specifically designed for modern web development. It focuses on fast development by leveraging ES Module imports and providing an optimized development server.
- **Key Features:**
  - Lightning-fast HMR (Hot Module Replacement).
  - Out-of-the-box support for Vue.js, React, and TypeScript.
  - Dependency pre-bundling for faster production builds.

### 2. Webpack
- **Description:** Webpack is a widely-used JavaScript module bundler. It takes assets, such as JavaScript, CSS, and images, and transforms them into a format suitable for the web.
- **Key Features:**
  - Powerful and configurable with a rich plugin ecosystem.
  - Code splitting for efficient loading.
  - Loaders for processing various types of files.

### 3. Parcel
- **Description:** Parcel is a zero-configuration web application bundler. It automatically handles assets, requires minimal setup, and provides fast build times.
- **Key Features:**
  - Zero configuration, making it easy to get started.
  - Automatic asset handling without explicit configuration.
  - Fast development server and build times.

## Version Range Operators:

### 1. Caret (^)
- **Description:** The caret allows updates to the most recent minor or patch version while keeping the same major version.
- **Example:** `^1.2.3` allows updates to `1.2.4`, `1.3.0`, etc.

### 2. Tilde (~)
- **Description:** The tilde restricts updates to the same major version but allows updates to the latest patch version.
- **Example:** `~1.2.3` allows updates to `1.2.4` but not to `1.3.0`.

## Script Types in HTML (MDN Docs):

### 1. `<script>`
- **Description:** The standard script element used to embed or reference executable code, typically JavaScript.
- **Attributes:**
  - `src`: Specifies an external script file.
  - `type`: Specifies the MIME type of the script.

### 2. `<script type="module">`
- **Description:** Introduces ECMAScript modules to a page, allowing for better organization and encapsulation of code.
- **Attributes:**
  - `src`: Specifies an external module script file.
  - `type="module"`: Declares the script as an ECMAScript module.

### 3. `<script type="text/javascript">`
- **Description:** Deprecated way of specifying JavaScript. It's recommended to use `<script>` without the `type` attribute or use `<script type="module">`.
- **Note:** Explicitly specifying JavaScript is no longer necessary in HTML5.



