# Spotifie

Spotifie is a music streaming application that allows users to discover, listen to, and share music with their friends.

## Features
- User authentication and profile management
- Search and explore music catalogs
- Create and manage playlists
- Share songs and playlists with friends
- Offline listening capabilities

## Architecture
Spotifie is built using a microservices architecture. Key components include:
- Frontend: Android application
- Backend: RESTful API service
- Database: PostgreSQL for data persistence

For a detailed architecture diagram, please refer to the [Arch Diagram](link_to_diagram).

## Quick Start Guide
To set up the project locally, follow these steps:
1. Clone the repository:
   ```
   git clone https://github.com/QernovraLabs/spotifie
   cd spotifie
   ```
2. Install dependencies:
   ```
   npm install
   ```
3. Start the application:
   ```
   npm start
   ```

## API Endpoints
| Method | Endpoint           | Description                |
|--------|--------------------|----------------------------|
| GET    | /api/music          | Retrieve music catalog      |
| POST   | /api/users/login    | User login                 |
| POST   | /api/playlists      | Create a new playlist      |

## Environment Variables
To run the project, you need the following environment variables:
- `DB_HOST`: Database host
- `DB_USER`: Database user
- `DB_PASS`: Database password
- `PORT`: Port to run the server

## Docker Deployment Instructions
To run Spotifie using Docker, use the following commands:
1. Build the Docker image:
   ```
   docker build -t spotifie .
   ```
2. Run the container:
   ```
   docker run -p 8080:8080 spotifie
   ```

## Android App Features
- Intuitive user interface
- Offline music playback
- Seamless integration with social media

## Security Details
- JWT authentication for API access
- HTTPS for secure data transmission
- Regular security audits

## Database Schema
The database schema consists of the following tables:
- **Users**: Stores user data
- **Songs**: Stores song metadata
- **Playlists**: Stores user-generated playlists

## Testing Commands
To run the test suite, use the following command:
```
npm test
```

## Project Roadmap
- [ ] Implement personalized music recommendations
- [ ] Enhance user experience with machine learning
- [ ] Expand to web application
