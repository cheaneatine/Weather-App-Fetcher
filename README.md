# Simple Weather Information Retrieval Application  

This project is a simple tool designed to provide users with basic weather information for a specific city. It integrates the **OpenWeatherMap API** to fetch accurate, real-time weather data and displays it in a user-friendly interface. The application is designed to be lightweight, efficient, and easy to use.  

---

## Project Overview  

### Objective  
The primary goal of this project is to create a straightforward system where users can quickly and easily access key weather details without unnecessary complexity.

### Key Features  
- **Basic Weather Information**: Input a city name to retrieve temperature, humidity, and general weather conditions.  
- **User-Friendly Interface**: Minimal and intuitive design for effortless interaction.  
- **Error Handling**: Displays clear error messages if the city name is invalid or data retrieval fails.  
- **API Integration**: Utilizes the OpenWeatherMap API for up-to-date weather data.  
- **Lightweight Design**: Focused on core functionality, ensuring fast performance.

---

## System Architecture  

### Client (Front-end)  
- **Interface**: Users input a city name and view the weather details fetched from the backend.  
- **Technology**: Built with **Flask**, utilizing HTML templates for rendering data.  

### Server (Back-end)  
- **Functionality**: Fetches weather data from the OpenWeatherMap API based on user input.  
- **Technology**: Built in **Python**, leveraging the `socket` module for communication and `requests` for API calls.  

### Protocol (TCP/IP)  
- Ensures reliable communication between the client and server.  
- Manages request transmission and data delivery using TCP/IP.  

---

## Installation  

### Prerequisites  
- **Python 3.x** installed on your system.  
- Required Python libraries:  
  ```bash
  pip install flask requests
  ```

### Steps  
1. **Clone the repository**:  
   ```bash
   git clone https://github.com/your-username/weather-app.git
   ```
2. **Navigate to the project directory**:  
   ```bash
   cd weather-app
   ```
3. **Set up the server**:  
   - Open `server.py` and replace the placeholder `api_key` with your OpenWeatherMap API key.  
   - Start the server:  
     ```bash
     python server.py
     ```
4. **Run the Flask application**:  
   - Start the client:  
     ```bash
     flask run
     ```
5. Open your browser and go to `http://127.0.0.1:5000/`.

---

## Usage  

1. On the homepage, input a city name (e.g., "New York") and click "Get Weather."  
2. The application will display:  
   - Temperature  
   - Feels Like  
   - Humidity  
   - Weather Description  
   - Wind Speed  
   - Local Time  

---

## Testing  

### Unit Testing  
- **Client-Server Communication**: Ensures data is transmitted correctly between the client and server.  
- **Error Handling**: Tests edge cases like invalid city names and network issues.  

Run tests using Python's `unittest` framework:  
```bash
python test_server.py
python test_client_server.py
```

---

## Documentation  

### API Functions  
- **convert_to_local_time**: Converts Unix timestamps to readable local time.  
- **fetch_weather**: Fetches and formats weather data from the OpenWeatherMap API.  

### Flask Routes  
- **`/`**: Displays the homepage.  
- **`/weather`**: Processes user input and fetches weather data from the server.

---

## Authors  

- [Cherry Lee Jimenez](https://github.com/cheaneatine)
- [Eros P. Lucagbo](https://github.com/Eros628)
- [Zayq Rashid F. Maulod](https://github.com/zayqrashid)

Developed as part of the Computer Science program at the **University of Science and Technology of Southern Philippines**.
```

### Key Enhancements:
1. **Structured Sections**: Clear organization of the README, including project overview, installation, and usage.
2. **Professional Formatting**: Markdown formatting for better readability and a polished look.
3. **Detailed Instructions**: Step-by-step setup and usage instructions to guide users.
