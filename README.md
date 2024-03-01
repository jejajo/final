# Travel Agency Matayev Alibek SE-2208


## Installation

1. Clone the repository to your local machine:

    ```bash
    git clone https://github.com/your-username/travel-agency.git
    ```

2. Navigate to the project directory:

    ```bash
    cd travel-agency
    ```

3. Install the project dependencies using npm:

    ```bash
    npm install
    ```

## Configuration

1. Ensure that MongoDB is installed and running on your machine.

2. Update the MongoDB connection string in `server.js`:

    ```javascript
    mongoose.connect('mongodb://localhost:27017/travel');
    ```

    Change `localhost:27017` to the appropriate MongoDB server address if needed.

3. Obtain an API key from [WeatherAPI](https://www.weatherapi.com/) and replace the placeholder in `server.js`:

    ```javascript
    const apiKey = 'your-weatherapi-key';
    ```

## Running the Application

1. Start the server

2. Open your web browser and navigate to http://localhost:3000

## NPM Packages Used

- **express**: Web application framework for Node.js.
- **path**: Module for handling file paths.
- **mongoose**: MongoDB object modeling tool.
- **body-parser**: Middleware for parsing incoming request bodies.
- **ejs**: Embedded JavaScript templates for rendering views.
- **axios**: Promise-based HTTP client for making API requests.

## Application Structure

- **server.js**: Main server file that initializes the Express application, connects to MongoDB, and sets up routes.
- **routes/travelRoutes.js**: Defines the routes for handling tours, adding new tours, deleting tours, and serving other pages.
- **models/Tour.js**: MongoDB model for the Tour collection.
- **public/...**: HTML pages.

## Important Notes

- The server runs on the default port 3000. Ensure that this port is available and not in use by another application.
- The MongoDB connection assumes a local server running on the default port (localhost:27017). Update the connection string accordingly if using a different MongoDB setup.

With these instructions, you should have the travel agency project up and running on your local machine.
