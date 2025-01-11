# Installation Manual for Frontend Project

## Prerequisites
Ensure you have the following software installed:

1. **Node.js**: Download and install from [Node.js official website](https://nodejs.org/).
2. **npm or yarn**: Comes bundled with Node.js. Verify installation by running:
   ```bash
   node -v
   npm -v
   ```

## Downloading the Project

### 1. Clone the Repository
Clone the project repository to your local machine:
```bash
git clone <repository-url>
```
Navigate into the project directory:
```bash
cd frontend
```

Alternatively, you can download the project as a ZIP file:

1. Click on the "Code" button on the repository's page.
2. Select "Download ZIP."
3. Extract the ZIP file to your desired location.

### 2. Install Dependencies
Install the required dependencies using npm or yarn:

#### Using npm:
```bash
npm install
```

#### Using yarn:
```bash
yarn install
```

### 3. Start the Development Server
To start the development server, run:

#### Using npm:
```bash
npm run dev
```

#### Using yarn:
```bash
yarn dev
```

This will start the application, and you can access it at:
```
http://localhost:3000
```

### 4. Build for Production
To create a production build of the application, run:

#### Using npm:
```bash
npm run build
```

#### Using yarn:
```bash
yarn build
```

The optimized build files will be generated in the `build/` directory.

### 5. Run Tests
To execute tests, use:

#### Using npm:
```bash
npm test
```

#### Using yarn:
```bash
yarn test
```

## Configuration
### Browserslist
This project uses Browserslist to specify target browsers. The configurations are located in the `package.json` file under the `browserslist` key.

- **Production:**
  ```
  >0.2%
  not dead
  not op_mini all
  ```
- **Development:**
  ```
  last 1 chrome version
  last 1 firefox version
  last 1 safari version
  ```

## Tailwind CSS Integration
The project uses Tailwind CSS for styling. To customize Tailwind, modify the configuration file (`tailwind.config.js`). For more details, refer to the [Tailwind CSS documentation](https://tailwindcss.com/docs/configuration).

## Troubleshooting

- **Dependency Errors:** Run `npm install` or `yarn install` again to ensure all dependencies are installed.
- **Port Already in Use:** If the default port (3000) is occupied, specify an alternate port by setting the `PORT` environment variable:
  ```bash
  PORT=4000 npm run dev
  ```
- **Build Issues:** Ensure all dependencies are up-to-date by running:
  ```bash
  npm update
  ```

For additional help, consult the project documentation or contact the maintainers.

