# Star Wars Characters and Starships Visualization

This project provides a visualization of Star Wars characters, their appearances in movies, and the starships they've flown on. It is built using React and React Flow and uses the [Starnavi SW API](https://sw-api.starnavi.io/) to fetch and display data in an interactive flowchart format.

## Table of Contents
- [Features](#features)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Environment Variables](#environment-variables)
- [Usage](#usage)
- [Testing](#testing)
  - [Running Tests](#running-tests)
  - [Example Test Cases](#example-test-cases)
- [Deployment](#deployment)
  - [Deploying to Netlify](#deploying-to-netlify)
- [Additional Information](#additional-information)

## Features
- **Data Integration**: Fetches Star Wars data from [Starnavi SW API](https://sw-api.starnavi.io/) to display information about characters, movies, and starships.
- **Interactive Visualization**: Uses React Flow to provide a dynamic, interactive graph that illustrates relationships between characters, movies, and starships.
- **Custom Hooks**: Includes custom hooks to handle API requests and data processing for smooth, maintainable code.
- **Error Handling**: Implements robust error handling to manage network issues or failed API calls gracefully.

## Project Structure
- `src/api/`: Contains functions to handle API calls, such as `fetchFilms` to get data about Star Wars movies.
- `src/components/`: Houses reusable React components used across the project.
- `src/hooks/`: Includes custom hooks for managing API data and other logic.
- `src/interfaces/`: Defines TypeScript interfaces to enforce data structures and improve type safety.
- `src/pages/`: Contains main pages rendered by the application.
- `src/tests/`: Holds test cases, written with Jest and Testing Library, covering functionality and error handling for the project.

## Getting Started

### Prerequisites
Before starting, ensure that you have the following installed:
- [Node.js and npm](https://nodejs.org/)

### Installation
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/danikua/star-wars.git
   cd star-wars
   ```

2. **Install Dependencies**:
   ```bash
   npm install
   ```

### Environment Variables
No additional configuration or environment variables are required for this project.

## Usage
To start the application on a local development server, run:
```bash
npm start
```
The project will be accessible at [http://localhost:3000](http://localhost:3000).

## Testing
This project uses Jest and React Testing Library for unit and integration tests. Tests include cases for API calls, error handling, and data transformation.

### Running Tests
To execute all tests, use the following command:
```bash
npm test
```

### Example Test Cases
- **Successful API Call**: Ensures that `fetchFilms` returns the correct film data from the API.
- **Error Handling**: Verifies that `fetchFilms` returns null if an API call fails or encounters an error.
- **Empty Data Handling**: Checks that `fetchFilms` returns an empty array when no film data is available.

## Deployment

### Deploying to Netlify
To deploy this project to Netlify, follow these steps:
1. Log in to Netlify.
2. Create a New Site from Git, linking it to your GitHub repository.
3. Configure Build Settings:
   - Set the build command to `npm run build`.
   - Set the publish directory to `build/`.
4. Deploy the site, and Netlify will handle the rest of the deployment process.

## Additional Information
**Dependencies**:
- `axios`: For making HTTP requests to the SW API.
- `react-flow-renderer`: For the interactive flowchart.
- `jest` and `react-testing-library`: For writing and executing tests.

**API Documentation**:
- [Starnavi SW API](https://sw-api.starnavi.io/): Provides information about characters, movies, and starships from the Star Wars universe.

**Repository Link**:
Find the complete source code, tests, and this README file on GitHub: [https://github.com/danikua/star-wars](https://github.com/danikua/star-wars)
