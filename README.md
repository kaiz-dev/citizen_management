# Citizen Management System

> Software Engineering Introduction - Course Project

A web application designed to manage resident information, household registration, and fee collection within residential areas. The system features an intuitive interface that enables local administrators to efficiently track and update citizen data.

---

## Key Features

### Resident Management
- Add new residents to the system
- Edit and update personal information
- Register temporary residence and absence
- Process death certificates and archive records
- Search residents using multiple criteria

### Household Management
- View household list and detailed information
- Handle household separation requests
- Manage family members within each household
- Search by address or head of household

### Fee Collection Management
- Set up recurring fees (electricity, water, sanitation, etc.)
- Edit or remove fee items as needed
- Track automatic billing cycles
- Search and filter by fee type

### Contribution Management
- Record voluntary contributions
- Collect payments and update payment status
- View aggregated statistics over time
- Export detailed reports

---

## Tech Stack

### Frontend
| Technology | Description |
|------------|-------------|
| React 17 | UI component library |
| MobX | State management |
| React Router | Client-side routing |
| Styled Components | CSS-in-JS styling |
| DevExtreme | Professional UI components |
| Recharts | Statistical chart visualization |
| Axios | HTTP client for API calls |

### Backend
| Technology | Description |
|------------|-------------|
| Node.js | Server-side JavaScript runtime |
| Express | REST API framework |
| MongoDB | NoSQL database |
| Mongoose | MongoDB ODM |
| Swagger | API documentation |
| bcrypt | Password encryption |

---

## Installation

### Prerequisites
- Node.js version 14 or higher
- MongoDB installed and running
- npm or yarn

### Step 1: Clone the repository
```bash
git clone <repository-url>
cd citizen_management
```

### Step 2: Configure environment variables
Create a `.env` file in the `server` directory:
```env
PORT=8080
MONGODB_URL=mongodb://localhost:27017/citizen_management
```

### Step 3: Install dependencies

**Backend:**
```bash
cd server
npm install
```

**Frontend:**
```bash
cd ui/citizen_management
npm install
```

### Step 4: Run the application

**Start Backend:**
```bash
cd server
npm start
```
Server will run at `http://localhost:8080`

**Start Frontend:**
```bash
cd ui/citizen_management
npm start
```
Application will open at `http://localhost:3000`

---

## API Documentation

Once the server is running, access the Swagger UI for detailed endpoint documentation:

```
http://localhost:8080/api-docs
```

---

## Project Structure

```
citizen_management/
├── server/                     # Node.js Backend
│   ├── controllers/            # Business logic handlers
│   ├── models/                 # MongoDB schemas
│   ├── routers/                # API route definitions
│   └── index.js                # Server entry point
│
└── ui/citizen_management/      # React Frontend
    ├── public/                 # Static assets
    └── src/
        ├── components/         # React components
        │   ├── People/         # Resident management
        │   ├── Household/      # Household management
        │   ├── MoneyManagement/# Fee management
        │   └── ...
        ├── stores/             # MobX stores
        └── services/           # API services
```

---

## Screenshots

*Dashboard with overview statistics*

*Resident list management screen*

*Add new resident form*

---

## Contributing

Contributions are welcome. Please open an issue or submit a pull request if you would like to improve this project.

---

## License

This project was developed for educational purposes.
