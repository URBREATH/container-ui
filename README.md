URBREATH Container UI (Toolbox)
This project is a front-end component built for the EU URBREATH project that serves as a container UI that will integrate all URBREATH tools upon their completion.

Tech Stack
The URBREATH Container UI is built on the Material UI berry template and is implemented using:

React v18.2.0 Node.js v20.13.1 Material-UI v5.15.10 Next v14.1.0

Additional technologies used: - TypeScript for type safety - Redux Toolkit for state management
- Axios for API calls - Jest + React Testing Library for testing - ESLint + Prettier for code quality - Notistack for notifications

Building & Running the Application
To build and run the application, please follow the below instructions:

Prerequisites
Please ensure you have Node.js v20.13.1 or above installed on your machine. You can download and install it from the official Node.js website, following the installation instructions for your operating system.

Steps to Build and Run the Application:
Clone the repository:

git clone git@bitbucket.org:atc-code/ilab-urbreath-container-ui.git
Set up environmental variables:\ Ensure the .env file exists, with the required values set. An example of the .env file can be found in the .env.example file of this repository

Install project dependencies using npm:\ To install all project dependencies listed in the package.json file you need to run the command:

npm install
Check for linting or typescript errors (optional):\ In case you would like to analyze the code for potential errors (linting) in advance of building the app, please run the following command:

npm run lint
Similarly, to analyze the code for potential typescript errors, please run the command:

npm run type-check
To start the app locally:

npm run dev
For production deployment:\ For production deployment, first build the app:

npm run build
and then start the app on your production server:
npm run start
* Note: Open your web browser and navigate to http://localhost:3000 to view the application when running locally. If the application is deployed to a remote server, replace http://localhost:3000 with the appropriate domain or IP address.

Additional Notes:
Ensure that no other processes are using port 3000 on your machine before running the application. If port 3000 is already in use, you can specify a different port using the PORT environment variable:

npm run dev -- -p 3001
Available Scripts
The following scripts are available to manage the project:

npm run dev: Start development server with hot reload
npm run build: Create production build
npm run start: Start production server
npm run lint: Lint all files with ESLint
npm run lint:fix: Automatically fix linting errors
npm run type-check: Check for TypeScript errors
npm run prettier: Format code with Prettier
npm run test: Run tests with Jest
npm run test:watch: Run tests in watch mode
npm run coverage: Generate test coverage report
Testing
Run the test suite with:

npm test           # Run tests
npm run coverage   # Generate coverage report
Folder structure
ilab-urbreath-container-ui/
│
├── __mocks__               # Mocked components used in testing
├── __tests__               # Testing related files
├── public/                 # Static assets (images, fonts, etc.)
├── src/
│ ├── api/                  # API clients
│ ├── app/                  # Next.js App Router directory
│ │   ├── (dashboard)/      # Dashboard routes group
│ │   ├── (iframe)/         # i-frame related components routes group
│ │   ├── (minimal)/        # Minimal routes group
│ │   ├── (simple)/         # Simple routes group
│ │   ├── globals.css       # Global CSS file
│ │   ├── layout.tsx        # Root layout
│ │   └── page.tsx          # Home page
│ │
│ ├── components/           # Reusable UI components
│ ├── contexts/             # Contexts
│ ├── hooks/                # Custom hooks for various functionalities
│ ├── layout/               # Different layouts
| ├── menu-items/           # Navigation menu configuration
| ├── scss/                 # Styling scss files
│ ├── services/             # API services and business logic
│ ├── store/                # Redux store configuration and slices
│ ├── styles/               # Global styles
│ ├── test-utils/           # Testing utility/helper functions
│ ├── themes/               # Theme setup (palette, typography, etc.)
│ ├── types/                # TypeScript types & definitions used throughout the project
│ ├── utils/                # Utility/helper functions
│ ├── views/                # Main application pages/screens
|
├── .env.example            # Example environment variables
├── .prettierrc             # Prettier configuration
├── jest.config.ts          # Jest configuration
├── next.config.js          # Next.js configuration
├── tsconfig.json           # TypeScript configuration
│── jest.setup.ts           # Setup for the testing environment
└── README.md               # Documentation file
