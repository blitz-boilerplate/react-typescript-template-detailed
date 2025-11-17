# React TypeScript Template - Detailed

A comprehensive React TypeScript template with extensive starter code and configurations to help you get started quickly. This template includes testing setup, TypeScript configuration, and all the essentials you need to begin building React applications immediately.

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Demo Dashboard

This template includes a demo dashboard page that demonstrates how to make API calls to a backend service. The dashboard allows users to enter their name and sends it to a backend API endpoint for testing purposes.

### What It Does

The dashboard (`src/pages/Dashboard.tsx`) displays a simple form that:
- Prompts the user with "Hi, what's your name?"
- Allows the user to enter their name in a text input field
- Sends a POST request to `http://localhost:8080/api/hello` with a JSON body matching the `HelloWorldDto` structure (`{ "name": "..." }`)
- Displays the response message from the backend server

### Testing the Demo

To test the demo dashboard:

1. **Start the backend server** - Ensure your backend API is running on `http://localhost:8080` with an endpoint at `/api/hello` that accepts POST requests with a `HelloWorldDto` body.

2. **Start the React app**:
   ```bash
   npm start
   ```

3. **Open the browser** - Navigate to [http://localhost:3000](http://localhost:3000)

4. **Test the form** - Enter your name and click "Send" to see the API response.

### Removing the Demo Code

When you're ready to start building your actual application, you can remove the demo dashboard code:

1. **Delete the demo files**:
   - `src/pages/Dashboard.tsx`
   - `src/pages/Dashboard.css`
   - `src/services/api.ts` (if you don't need the API service structure)
   - `src/types/dto.ts` (if you don't need the DTO structure)

2. **Update `src/App.tsx`** - Replace the Dashboard import and usage with your own application components.

3. **Optional**: Keep the folder structure (`src/pages/`, `src/services/`, `src/types/`) as a reference for organizing your own code, or remove them if you prefer a different structure.

The demo code serves as a reference implementation showing:
- How to structure TypeScript interfaces/DTOs
- How to create API service functions
- How to build React components with form handling and API integration
- How to handle loading states and errors

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.\
You will also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).
