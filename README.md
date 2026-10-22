# 📦 dickmanpious

A simple, lightweight Node.js package published to the npm registry, created to demonstrate the full lifecycle of building, versioning, and publishing an npm package.

[![npm version](https://img.shields.io/badge/npm-1.0.2-blue.svg)](https://www.npmjs.com/package/dickmanpious)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## 🚀 Installation

You can install this package directly from the npm registry using `npm` or `yarn`:

npm install dickmanpious

## 💻 Usage

Here is how you can import and use this package in your JavaScript or Node.js project:

const dickmanpious = require('dickmanpious');

dickmanpious();

**Expected Output:**

Hello from dickmanpious!

## 🛠️ Local Development & Testing

If you want to clone this repository and test it locally:

1. Clone the repository:
git clone https://github.com/dickmanpiouscyber/npm-dickmanpious.git

2. Navigate into the directory:
cd npm-dickmanpious

3. Run the script directly:
node index.js

## 📁 Project Structure

- index.js — The main entry point containing the package logic.
- package.json — Package metadata, version, and configuration.
- .github/workflows/publish.yml — GitHub Actions automation for CI/CD publishing.

## 🚀 Publishing Pipeline

This repository is configured with GitHub Actions. Whenever code is pushed to the main branch, the action automatically triggers an npm stage publish workflow. This ensures that every new version is securely scanned and validated by npm before being released.

## 🔄 How to Publish an Update

1. Edit files inside the dickmanpious folder.
2. Open package.json and bump the version number (e.g., from 1.0.2 to 1.0.3).
3. Commit and push the changes to GitHub.
4. GitHub Actions will automatically run the publish workflow.
5. Go to npmjs.com -> Staged Packages to approve the new version.

## 🔐 Environment Variables & Tokens

If you are running the publish locally, you must create a .npmrc file in the root of the project folder with your npm token:

//registry.npmjs.org/:_authToken=YOUR_NPM_TOKEN

Run the publish command:

npm publish --access public

Important: Delete the .npmrc file immediately after publishing so your token is never exposed:

Remove-Item .npmrc -Force

## 👨‍💻 Author

Dickman Pious
- GitHub: @dickmanpiouscyber

## 📄 License

This project is licensed under the MIT License.
