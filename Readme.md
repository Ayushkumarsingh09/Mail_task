# Mail_task: Mailing Scheduling Feature in Next.js

## Description
Mail_task is a Next.js-based application designed to manage and schedule email campaigns. A mailing is an email-based campaign sent to groups of users. Users can create, review, and schedule these mailings in advance for delivery at a specific date and time.

### Core Components of a Mailing
1. **Template (Mailer)**: Email templates fetched via an API, identified by `id` and `name`.
2. **Recipient List**: A group of recipients, fetched via an API, identified by `id` and `name`.
3. **Schedule**: The specific day and time when the email campaign is sent.

## Assumptions
- **Templates (Mailers)**: 
  - Fetched via an API call.
  - Only `id` and `name` are fetched; the actual content is handled by the mail-sending module.
- **Recipient Lists**:
  - Fetched via an API call.
  - Only `id` and `name` are fetched; the actual recipient details are handled by the mail-sending module.
- **CRUD API for Mailing**:
  - An API exists for creating, reading, updating, and deleting mailings, including mailer `id`, list `id`, and schedule details.

To showcase the functionality, mock APIs are used to simulate the required backend services.

## Features
1. **Mailing Scheduling**:
   - Create a new mailing by selecting a mailer template, a recipient list, and a schedule.
   - Edit or delete existing mailings.
   - View a list of scheduled mailings.

2. **API Integration**:
   - Fetch mailer templates and recipient lists via API calls.
   - Perform CRUD operations for managing mailings.

3. **UI Features**:
   - Modern and responsive user interface built with Next.js.
   - Form validation for scheduling inputs.

4. **Mock APIs**:
   - Mocked API endpoints simulate backend functionality for templates, recipient lists, and mailing operations.

## Installation and Setup

### Prerequisites
- Node.js (v16 or later)
- npm or yarn

## Installation and Setup

### Install Dependencies
```bash
npm install
### Steps to Run Locally
1. Clone the repository:
   ```bash
   git clone https://github.com/Ayushkumarsingh09/Mail_task.git && cd Mail_task

Start the Application
bash
Copy code
npm run dev
The app will be hosted locally at http://localhost:3000.

API Mocking
Mock APIs are used to simulate the following operations:

Fetch Mailers
Endpoint: /api/mailers
Description: Returns a list of mailers (id, name).
Fetch Recipient Lists
Endpoint: /api/lists
Description: Returns a list of recipient groups (id, name).
CRUD Operations for Mailings
Endpoint: /api/mailings
Description: Supports GET, POST, PUT, and DELETE.
Directory Structure
bash
Copy code
Mail_task/
├── components/      # Reusable UI components
├── pages/           # Next.js pages
│   ├── index.js     # Homepage listing scheduled mailings
│   ├── create.js    # Page for creating new mailings
│   └── api/         # Mock API endpoints
├── styles/          # Styling files
├── utils/           # Utility functions
└── README.md        # Project documentation
Deployment
To make the app publicly accessible:
Deploy the application on Vercel.
Configure the project for automatic deployment from the GitHub repository.
Repository
GitHub Link: Mail_task