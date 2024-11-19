# Event-Showcase
Welcome to the Event Showcase! This is a Node.js-based web application designed to display and manage events. It features a homepage where users can view featured events, upcoming events, and a gallery of past events. 
 The admin dashboard provides easy management of event content, including the ability to add, edit, or delete events. The gallery showcases events with their images, and each event has a detailed modal view that users can open to get more information.
#Getting started
To get started, you will need to have Node.js and MySQL installed on your system. 

### Prerequisites

- Install [Node.js](https://nodejs.org/) on your machine.
- Install [MySQL](https://www.mysql.com/) on your machine.
 ##Installing

You can clone this repository using `git clone https://github.com/FaithGikura/event-showcase.git` and run `npm install` to install the necessary dependencies. 
Once the dependencies are installed, configure your MySQL database by creating a new database called `event_showcase` and setting up a table for events with the following SQL: `CREATE TABLE events (id INT AUTO_INCREMENT PRIMARY KEY, name VARCHAR(255) NOT NULL, description TEXT NOT NULL, date DATETIME NOT NULL, image_url VARCHAR(255), featured BOOLEAN DEFAULT FALSE);`.
You will also need to update the database connection details in `app.js` to match your MySQL credentials.
After everything is set up, run the app with `npm start` and navigate to `http://localhost:3000` in your browser. The admin dashboard is accessible at `http://localhost:3000/admin`, where you can add new events, edit or delete existing ones. For adding events, images are uploaded through the admin form using the `Multer` middleware, and images are stored in the `public/uploads` folder.
##Other details
The homepage displays the featured event, nearest upcoming event, and past event gallery. The event gallery allows users to click on an image to view more details in a modal, including the event’s name, date, and description.
If you want to contribute to this project, feel free to fork the repository and submit pull requests for new features or bug fixes.
This project uses Node.js, Express.js, MySQL, EJS for templating, and Multer for image uploading.
It is licensed under the MIT License, and you can view the full license details in the `LICENSE` file.
If you'd like to deploy this application or have any questions, feel free to reach out.
Thank you for using Event Showcase! 

