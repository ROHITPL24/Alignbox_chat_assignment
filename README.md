# Alignbox - Chat UI Assignment (Full Project)

## What this contains
- `public/` - Frontend files (index.html, styles.css, client.js)
- `server.js` - Node.js + Express backend
- `package.json` - Node dependencies
- `db.sql` - SQL to create the messages table
- `.env.example` - example environment variables
- `README.md` - this file

## Features implemented
- Simple chat UI (HTML/CSS/Vanilla JS) inspired by provided Figma.
- Backend API endpoints to save and fetch messages (MySQL).
- No image/attachment upload (skipped as permitted).
- Simple sample data and easy setup instructions.

## Quick setup (on your machine)
1. Install Node.js (v16+ recommended) and MySQL.
2. Create a MySQL database and run `db.sql`:
   ```sql
   CREATE DATABASE alignbox_chat;
   USE alignbox_chat;
   -- then run the contents of db.sql
   ```
3. Copy `.env.example` to `.env` and fill your DB credentials:
   ```
   DB_HOST=localhost
   DB_PORT=3306
   DB_USER=root
   DB_PASS=your_password
   DB_NAME=alignbox_chat
   PORT=4000
   ```
4. Install server dependencies:
   ```bash
   npm install
   ```
5. Start the server:
   ```bash
   node server.js
   ```
6. Open `http://localhost:4000` in your browser.

## Notes
- The server uses `mysql2` package with a simple connection pool.
- The frontend stores messages by calling `/api/messages`.
- For production use, sanitize and validate inputs more strictly and implement authentication.

Good luck with the assignment! If you want, I can customize strings, UI colors,
or produce a short demo GIF. 
# Alignbox_chat_assignment
