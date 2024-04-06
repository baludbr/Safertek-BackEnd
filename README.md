# Express File Management App(Safertek Backend)

This is a simple Express.js application for managing files. It provides basic CRUD (Create, Read, Update, Delete) operations on files stored in a specified directory.

## Installation

1. **Clone the repository:**
    ```bash
    git clone <https://github.com/baludbr/Safertek-BackEnd.git>
    ```
2. **Navigate to the project directory:**
    ```bash
    cd Safertek-BackEnd
    ```
3. **Install dependencies:**
    ```bash
    npm install
    ```

## Usage

1. **Start the server:**
    ```bash
    npm start
    ```
2. **Access the application in your web browser or through API requests.**

## API Endpoints

- `POST /createFile`: Create a new file with specified filename and content. Requires authentication with a password query parameter.
- `GET /getFiles`: Get a list of all files in the upload directory.
- `GET /getFile/:filename`: Get the content of a specific file. Requires authentication.
- `PUT /modifyFile/:filename`: Modify the content of a specific file. Requires authentication.
- `DELETE /deleteFile/:filename`: Delete a specific file. Requires authentication.

### Authentication

All endpoints except `GET /getFiles` require authentication with a password query parameter. The default password is `pwd123`.

## Project Structure

- `index.js`: Entry point of the application.
- `uploads/`: Directory where uploaded files are stored.
- `middleware/authenticate.js`: Authentication middleware.
- `middleware/logger.js`: Request logging middleware.
- `routes/files.js`: Route handlers for file operations.

## Dependencies

- [Express.js](https://expressjs.com/): Web application framework for Node.js.
- [fs](https://nodejs.org/api/fs.html): Node.js file system module for file operations.
- [path](https://nodejs.org/api/path.html): Node.js path module for working with file paths.

## Contributing

Contributions are welcome! Please feel free to submit issues or pull requests.

## License

This project is licensed under the [MIT License](LICENSE).

This work was done by 2100030140-D BALAJI REDDY
