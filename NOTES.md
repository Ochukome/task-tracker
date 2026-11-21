
cat > NOTES.md <<'EOF'
# Week 1 Assessment: Starter App Exploration

## 1. App Overview

The Task Tracker is a task management application built with React, Express and SQLite.

The React frontend allows users to create, view, edit, delete and complete tasks. Users can also assign priorities and due dates and filter tasks by their completion status.

The Express backend handles API requests from the frontend, while the SQLite database stores task information.

## 2. Features I Tested

I tested the following features by interacting with the application:

- Creating new tasks.
- Marking tasks as completed.
- Filtering tasks using All, Active and Done.
- Editing existing tasks.
- Deleting tasks.
- Assigning task priorities.
- Setting due dates.

The features worked as expected during my testing.

## 3. Improvements I Would Make

### 1. Add a Delete Confirmation

Currently, clicking the Delete button removes a task immediately without asking the user to confirm.

I would add a confirmation dialog to prevent accidental deletion of tasks.

### 2. Improve Mobile Responsiveness

The frontend uses a fixed width of 900px for its main container and task table.

This can make the application difficult to use on smaller screens, especially mobile devices.

I would introduce responsive layouts so that the application works properly across different screen sizes.

### 3. Add Better Error Handling and User Feedback

The application does not provide clear feedback when an API request fails.

I would add error messages and loading indicators when tasks are being created, updated or deleted. This would help users understand what is happening and know when an action fails.

## 4. AI Tools and Prompts Used

AI tool used: ChatGPT.

I used ChatGPT to help me explore and understand the application.

Some of the prompts and questions I used included:

- Help me understand how to run the Task Tracker application.
- What happens when I mark a task as completed?
- Explain what the React code in App.jsx does.
- Explain how useState and useEffect work in this application.
- Explain how the frontend communicates with the Express backend.
- Help me understand the API routes in server.js.
- Explain how the SQLite database stores task information.
- What improvements would make this application better?

I also compared the AI explanations with the actual application behaviour and source code.

## 5. One Thing AI Initially Missed

When discussing the database, AI initially gave a general explanation of SQLite without explaining the specific implementation used in this project.

After inspecting server/db.js, I noticed that the project uses sql.js, which keeps the database in memory and exports it to a database file when changes are saved.

This helped me understand that the project does not interact with SQLite in exactly the same way as a traditional SQLite database connection.

I noticed this by reading the actual database implementation instead of relying only on the AI explanation.

## 6. What I Learned

Through this exploration, I learned how the different parts of a full-stack application work together.

I understood that:

- React handles the user interface.
- Express handles backend requests and API routes.
- SQLite stores application data.
- Fetch API allows the frontend to communicate with the backend.
- HTTP methods such as GET, POST, PUT and DELETE are used for different operations.

I also learned the importance of testing an application and checking AI explanations against the actual source code.

EOF
