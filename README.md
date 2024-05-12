
# EmployIT

The Job Application Management System is a web application built with Node.js and Express.js that allows users to post job openings, apply for jobs, and manage job applications. It provides functionality for both employers and job seekers to interact with the platform.

## Features

- User registration and authentication
- Authorization based on user roles (Employer, Job Seeker)
- Posting job openings
- Applying for jobs with resume uploads
- Viewing job applications
- Managing job applications (for employers)
- Viewing own posted jobs (for employers)
- Updating and deleting posted jobs (for employers)
- Viewing own job applications (for job seekers)
- Deleting own job applications (for job seekers)


## Installation

To install EmployIT, follow these steps:

1. Clone the repository:
```bash
  git clone <repository-url>
```
2. Install dependencies:
```bash
  npm install
```
3. Set up environment variables:
- Create a .env file in the root directory
- Add the following environment variables:

```makefile
PORT=<port-number>
FRONTEND_URL=<frontend-url>
COOKIE_EXPIRE=<cookie-expiration-time>
JWT_SECRET_KEY=<jwt-secret-key>
CLOUDINARY_CLIENT_NAME=<cloudinary-client-name>
CLOUDINARY_CLIENT_API=<cloudinary-client-api>
CLOUDINARY_CLIENT_SECRET=<cloudinary-client-secret>

```
4. Start the server
```bash
npm start
```
## API ENDPoints

### User Routes

- `POST /api/v1/user/register` : Register a new user.
- `POST /api/v1/user/login` : Login as a user.
- `GET /api/v1/user/logout` : Logout the current user.
- `GET /api/v1/user/getuser` : Get user details.

### Application Routes
- `POST /api/v1/application/post` : Post a job application.
- `GET /api/v1/application/employer/getall` : Get all job applications for employers.
- `GET /api/v1/application/jobseeker/getall` : Get all job applications for job seekers.
- `DELETE /api/v1/application/delete/:id` : Delete a job application by ID.
### Job Routes
- `GET /api/v1/job/getall` : Get all job openings.
- `POST /api/v1/job/post` : Post a new job opening.
- `GET /api/v1/job/getmyjobs` : Get jobs posted by the current user.
- `PUT /api/v1/job/update/:id` : Update a job opening by ID.
- `DELETE /api/v1/job/delete/:id` : Delete a job opening by ID.
- `GET /api/v1/job/:id` : Get a single job opening by ID.
## Technologies Used 

- Node.js
- Express.js
- MongoDB (with Mongoose)
- JWT (JSON Web Tokens)
- Cloudinary (for file uploads)
- React.js (for the frontend)
## Support

For support, email sahs82341@gmail.com 

