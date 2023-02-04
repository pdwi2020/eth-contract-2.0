# The Solidity Contract-Oriented Programming Language

Solidity is a statically typed, contract-oriented, high-level language for implementing smart contracts on the Ethereum platform.

For a good overview and starting point, please check out the official [Solidity Language Portal](https://soliditylang.org).

## Table of Contents

- [Background](#background)
- [Build and Install](#build-and-install)
- [Example](#example)
- [Documentation](#documentation)
- [Development](#development)
- [Maintainers](#maintainers)
- [License](#license)
- [Security](#security)

## Background

Solidity is a statically-typed curly-braces programming language designed for developing smart contracts
that run on the Ethereum Virtual Machine. Smart contracts are programs that are executed inside a peer-to-peer
network where nobody has special authority over the execution, and thus they allow anyone to implement tokens of value,
ownership, voting, and other kinds of logic.

When deploying contracts, you should use the latest released version of
Solidity. This is because breaking changes, as well as new features and bug fixes, are
introduced regularly. We currently use a 0.x version
number [to indicate this fast pace of change](https://semver.org/#spec-item-4).

## Build and Install

Instructions about how to build and install the Solidity compiler can be
found in the [Solidity documentation](https://docs.soliditylang.org/en/latest/installing-solidity.html#building-from-source).


## Example

A "Hello World" program in Solidity is of even less use than in other languages, but still:

```solidity
// SPDX-License-Identifier: MIT
pragma solidity >=0.6.0 <0.9.0;

contract HelloWorld {
    function helloWorld() external pure returns (string memory) {
        return "Hello, World!";
    }
}
```

To get started with Solidity, you can use [Remix](https://remix.ethereum.org/), which is a
browser-based IDE. Here are some example contracts:

1. [Voting](https://docs.soliditylang.org/en/latest/solidity-by-example.html#voting)
2. [Blind Auction](https://docs.soliditylang.org/en/latest/solidity-by-example.html#blind-auction)
3. [Safe remote purchase](https://docs.soliditylang.org/en/latest/solidity-by-example.html#safe-remote-purchase)
4. [Micropayment Channel](https://docs.soliditylang.org/en/latest/solidity-by-example.html#micropayment-channel)

## Documentation

The Solidity documentation is hosted using [Read the Docs](https://docs.soliditylang.org).

## Development

Solidity is still under development. Contributions are always welcome!
Please follow the
[Developers Guide](https://docs.soliditylang.org/en/latest/contributing.html)
if you want to help.

You can find our current feature and bug priorities for forthcoming
releases in the [projects section](https://github.com/ethereum/solidity/projects).

## Maintainers
The Solidity programming language and compiler are open-source community projects governed by a core team.
The core team is sponsored by the [Ethereum Foundation](https://ethereum.foundation/).

## License
Solidity is licensed under [GNU General Public License v3.0](LICENSE.txt).

Some third-party code has its [own licensing terms](cmake/templates/license.h.in).

# Getting Started with Next.js

Welcome to the Next.js documentation!

If you're new to Next.js, we recommend starting with the learn course. The interactive course with quizzes will guide you through everything you need to know to use Next.js.

If you have questions about anything related to Next.js, you're always welcome to ask our community on GitHub Discussions.

System Requirements
- Node.js 14.6.0 or newer
- MacOS, Windows (including WSL), and Linux are supported
- Automatic Setup

We recommend creating a new Next.js app using create-next-app, which sets up everything automatically for you. (You don't need to create an empty directory. create-next-app will make one for you.) To create a project, run:

### 'npx create-next-app@latest'

# or

### 'yarn create next-app'

# or

### 'pnpm create next-app'

If you want to start with a TypeScript project you can use the --typescript flag:

### 'npx create-next-app@latest --typescript'

# or

### 'yarn create next-app --typescript'

# or

### 'pnpm create next-app --typescript'

After the installation is complete:

- Run npm run dev or yarn dev or pnpm dev to start the development server on http://localhost:3000
- Visit http://localhost:3000 to view your application
- Edit pages/index.js and see the updated result in your browser
- For more information on how to use create-next-app, you can review the create-next-app documentation.

Manual Setup
- Install next, react and react-dom in your project:

### 'npm install next react react-dom'

# or

### 'yarn add next react react-dom'

# or

### 'pnpm add next react react-dom'

Open package.json and add the following scripts:
```
"scripts": {
"dev": "next dev",
"build": "next build",
"start": "next start",
"lint": "next lint"
}
```
These scripts refer to the different stages of developing an application:

- dev - Runs next dev to start Next.js in development mode
- build - Runs next build to build the application for production usage
- start - Runs next start to start a Next.js production server
- lint - Runs next lint to set up Next.js' built-in ESLint configuration
- Create two directories pages and public at the root of your application:

- pages - Associated with a route based on their file name. For example, pages/about.js is mapped to /about
- public - Stores static assets such as images, fonts, etc. Files inside public directory can then be referenced by your code starting from the base URL (/).

Next.js is built around the concept of pages. A page is a React Component exported from a .js, .jsx, .ts, or .tsx file in the pages directory. You can even add dynamic route parameters with the filename.

Inside the pages directory, add the index.js file to get started. This is the page that is rendered when the user visits the root of your application.

Populate pages/index.js with the following contents:
```
function HomePage() {
return <div>Welcome to Next.js!</div>
}

export default HomePage
```
After the set up is complete:

- Run ```npm run dev``` or ```yarn dev``` or ```pnpm dev``` to start the development server on http://localhost:3000
- Visit http://localhost:3000 to view your application
- Edit pages/index.js and see the updated result in your browser

So far, we get:

- Automatic compilation and bundling
- React Fast Refresh
- Static generation and server-side rendering of pages/
- Static file serving through public/ which is mapped to the base URL (/)
- In addition, any Next.js application is ready for production from the start. Read more in our Deployment documentation.
