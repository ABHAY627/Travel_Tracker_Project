# Travel Tracker Project

Welcome to the **Travel Tracker Project**! This application is a learning project focused on using PostgreSQL databases, featuring a web interface built with EJS, JavaScript, and CSS.

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
- [Database Setup](#database-setup)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

---

## Project Overview

The Travel Tracker Project helps users keep track of their travels. Whether you want to log new destinations, update existing trips, or simply view a summary of your adventures, this application provides an intuitive interface to manage your travel history.

This project is designed as a practical exercise for learning how to integrate PostgreSQL databases with server-side rendering using EJS templates.

## Features

- **Add New Trips:** Log new travel destinations with details such as location, dates, and notes.
- **Edit and Update:** Modify trip information or update your notes as your journey progresses.
- **View All Travels:** Browse all the trips you've recorded in a clear, organized manner.
- **Delete Trips:** Remove trips you no longer want to keep in your records.
- **Responsive Design:** Clean and user-friendly interface for desktop and mobile devices.

## Tech Stack

- **Backend:** Node.js (Express.js)
- **Database:** PostgreSQL
- **Templating Engine:** EJS
- **Frontend:** HTML, CSS, JavaScript

## Getting Started

Follow these instructions to set up the project locally:

### Prerequisites

- [Node.js](https://nodejs.org/) (v14 or higher)
- [PostgreSQL](https://www.postgresql.org/) (v12 or higher)
- [npm](https://www.npmjs.com/)

### Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/ABHAY627/Travel_Tracker_Project.git
   cd Travel_Tracker_Project
   ```

2. **Install the dependencies:**

   ```bash
   npm install
   ```

3. **Configure Environment Variables:**

   Create a `.env` file in the root directory and add your database configuration:

   ```
   DB_HOST=localhost
   DB_USER=your_postgres_user
   DB_PASSWORD=your_postgres_password
   DB_NAME=your_database_name
   DB_PORT=5432
   ```

4. **Set up the database:**

   - Create the PostgreSQL database and tables as required (see [Database Setup](#database-setup)).

5. **Start the application:**

   ```bash
   npm start
   ```

   The app should now be available at [http://localhost:3000](http://localhost:3000).

## Database Setup

You need to create the necessary tables for the application. Here is an example schema for a simple travel tracking app:

```sql
CREATE TABLE trips (
    id SERIAL PRIMARY KEY,
    destination VARCHAR(100) NOT NULL,
    start_date DATE NOT NULL,
    end_date DATE,
    notes TEXT
);
```

You can modify this schema as per your requirements.

## Usage

- Visit [http://localhost:3000](http://localhost:3000) in your browser.
- Use the web interface to add, edit, view, or delete your travel records.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or suggestions.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is for learning purposes. You are free to use and modify it.

## Acknowledgements

- [Node.js](https://nodejs.org/)
- [Express.js](https://expressjs.com/)
- [PostgreSQL](https://www.postgresql.org/)
- [EJS](https://ejs.co/)
- Everyone who contributed to the open-source libraries used in this project

---

Happy Traveling! ✈️🌏
