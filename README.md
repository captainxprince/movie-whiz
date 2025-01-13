# Movie Whiz

Movie Whiz is a web application designed to provide personalized movie recommendations to users. By leveraging a curated database of movies, it offers suggestions based on user preferences and interactions.

## Features

- **Personalized Recommendations**: Receive movie suggestions tailored to your tastes.
- **Interactive Interface**: Engage with an intuitive and user-friendly web interface.
- **Database Integration**: Access a curated list of movies stored in a SQLite database.

## Getting Started

Follow these instructions to set up and run Movie Whiz on your local machine.

### Prerequisites

Ensure you have the following installed:

- **Python 3.x**: The application is built using Python.
- **Flask**: A lightweight WSGI web application framework for Python.
- **SQLite**: A C-language library that provides a lightweight, disk-based database.

### Installation

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/captainxprince/movie-whiz.git
   cd movie-whiz
   ```

2. **Set Up a Virtual Environment** (Optional but recommended):

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**:

   ```bash
   pip install -r requirements.txt
   ```

4. **Initialize the Database**:

   Ensure the SQLite database is set up correctly:

   - If `database.db` is not present, create it by running the provided SQL scripts:

     ```bash
     sqlite3 database.db < initialise.sql
     sqlite3 database.db < mytable.sql
     ```

   - Verify that the database contains the necessary tables and data.

5. **Run the Application**:

   ```bash
   python run_app.py
   ```

   Access the application by navigating to `http://localhost:5000` in your web browser.

## Project Structure

- **`run_app.py`**: The main entry point of the application. It initializes and runs the Flask web server.
- **`media.py`**: Contains the `Movie` class, representing movie objects with attributes like title, storyline, poster image URL, and trailer URL.
- **`entertainment_center.py`**: Script to create instances of the `Movie` class and store them in a list.
- **`fresh_tomatoes.py`**: Generates the HTML file to display movies, creating a static webpage showcasing the movie instances.
- **`models.py`**: Defines the database models and handles interactions with the SQLite database.
- **`static/`**: Directory containing static files such as CSS, JavaScript, and images.
- **`templates/`**: Directory containing HTML templates rendered by Flask.

## Usage

Upon running the application:

1. **Homepage**: View a list of recommended movies.
2. **Movie Details**: Click on a movie to see its details, including storyline and trailer.
3. **Add to Favorites**: Mark movies as favorites for future reference.

## Contributers

- Sayandeep
- Parvez
- Sarika
- Saumya

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

## Acknowledgments

- Inspired by the need for personalized movie recommendations.
- Built with Flask and SQLite for efficient web development and data management.

Thank you 😊