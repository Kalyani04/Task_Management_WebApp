# Task_Management_WebApp

A simple and efficient Task Management Web Application built using Django and React.

**Features**
  	Task Creation: Easily create tasks with titles and descriptions.

  Task Status: Mark tasks as completed or incompleted.

  Task Editing: Edit task details, including title and description.

  Task Deletion: Remove tasks when they are no longer needed.

  View Options: Filter tasks by completed and incompleted status.

  User-Friendly Interface: A clean and intuitive user interface for managing tasks.

**Technologies Used :-**

  1.Backend: Django (Python)

  2.Frontend: React (JavaScript)

  3.Database: SQLite (Included with Django)

  4.HTTP Requests: Axios

**Getting Started:-**

  cd Task-Management-App-Using-Django-React

**Backend Setup**

  Navigate to the backend directory and create a virtual environment.

  cd backend

  python -m venv venv

  source venv/bin/activate   # On Windows

  Install backend dependencies and run the Django server.

  pip install -r requirements.txt

  python manage.py migrate

  python manage.py runserver

**Frontend Setup**:

  Navigate to the frontend directory.

  cd frontend

  Install frontend dependencies and start the development server.

  npm install

  npm start

  Access the Application:

  Open your web browser and access the Task Management Web Application at http://localhost:3000/.

**Usage**:-

  Create, edit, and delete tasks as needed.

  Filter tasks by completed and incompleted status.

  Enjoy a streamlined task management experience!


  ## API Endpoints

This Django REST framework application provides the following API endpoints:

 **Task Endpoints**

- **List all tasks**
  - **URL:** `/api/tasks/`
  - **HTTP Method:** GET
  - **Description:** Retrieves a list of all tasks.
  - **Response:**
    ```json
    [
      {
        "id": 1,
        "title": "Task 1",
        "description": "Description of Task 1",
        "completed": false
      },
      {
        "id": 2,
        "title": "Task 2",
        "description": "Description of Task 2",
        "completed": true
      }
    ]
    ```

- **Create a new task**
  - **URL:** `/api/tasks/`
  - **HTTP Method:** POST
  - **Description:** Creates a new task.
  - **Request Body:**
    ```json
    {
      "title": "New Task",
      "description": "Description of the new task",
      "completed": false
    }
    ```
  - **Response:**
    ```json
    {
      "id": 3,
      "title": "New Task",
      "description": "Description of the new task",
      "completed": false
    }
    ```

- **Retrieve a specific task**
  - **URL:** `/api/tasks/{task_id}/`
  - **HTTP Method:** GET
  - **Description:** Retrieves details of a specific task.
  - **Response:**
    ```json
    {
      "id": 1,
      "title": "Task 1",
      "description": "Description of Task 1",
      "completed": false
    }
    ```

- **Update a task**
  - **URL:** `/api/tasks/{task_id}/`
  - **HTTP Method:** PUT
  - **Description:** Updates the details of a specific task.
  - **Request Body:**
    ```json
    {
      "title": "Updated Task",
      "description": "Updated description",
      "completed": true
    }
    ```
  - **Response:**
    ```json
    {
      "id": 1,
      "title": "Updated Task",
      "description": "Updated description",
      "completed": true
    }
    ```

- **Delete a task**
  - **URL:** `/api/tasks/{task_id}/`
  - **HTTP Method:** DELETE
  - **Description:** Deletes a specific task.
  - **Response:**
    ```json
    {
      "message": "Task deleted successfully"
    }
    ```

These are the main endpoints provided by the API. You can use these endpoints to manage tasks within the application.

