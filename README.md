# 🚀 REST API Template

A production-ready REST API template built with Node.js, Express, and MongoDB.

## ✨ Features
- User authentication (JWT)
- Role-based access control
- Input validation
- Error handling
- Rate limiting
- API documentation (Swagger)
- Logging
- Database migrations
- Unit & integration tests
- Docker support

## 🛠️ Tech Stack
- **Runtime:** Node.js 18+
- **Framework:** Express.js
- **Database:** MongoDB with Mongoose
- **Auth:** JWT + bcrypt
- **Validation:** Joi
- **Testing:** Jest + Supertest
- **Documentation:** Swagger/OpenAPI

## 🚀 Quick Start

```bash
# Clone
git clone https://github.com/YOUR_USERNAME/rest-api-template.git

# Install dependencies
npm install

# Set environment variables
cp .env.example .env

# Run development server
npm run dev

# Run tests
npm test
```

## 📡 API Endpoints

### Authentication
| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | /api/auth/register | Register user |
| POST | /api/auth/login | Login user |
| POST | /api/auth/refresh | Refresh token |
| POST | /api/auth/logout | Logout user |

### Users
| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | /api/users | Get all users |
| GET | /api/users/:id | Get user by ID |
| PUT | /api/users/:id | Update user |
| DELETE | /api/users/:id | Delete user |

### Resources (Example)
| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | /api/resources | Get all resources |
| POST | /api/resources | Create resource |
| GET | /api/resources/:id | Get resource |
| PUT | /api/resources/:id | Update resource |
| DELETE | /api/resources/:id | Delete resource |

## 📁 Project Structure
```
rest-api-template/
├── src/
│   ├── config/
│   │   └── database.js
│   ├── middleware/
│   │   ├── auth.js
│   │   ├── errorHandler.js
│   │   └── validator.js
│   ├── models/
│   │   └── User.js
│   ├── routes/
│   │   ├── auth.js
│   │   └── users.js
│   ├── controllers/
│   │   ├── authController.js
│   │   └── userController.js
│   ├── services/
│   │   ├── authService.js
│   │   └── userService.js
│   ├── utils/
│   │   ├── ApiError.js
│   │   └── logger.js
│   └── app.js
├── tests/
│   ├── auth.test.js
│   └── users.test.js
├── .env.example
├── package.json
└── README.md
```

## 🔧 Environment Variables
```env
PORT=3000
MONGODB_URI=mongodb://localhost:27017/api
JWT_SECRET=your-secret-key
JWT_EXPIRE=30d
NODE_ENV=development
```

## 📚 API Documentation
After starting server, visit: `http://localhost:3000/api-docs`

## 🐳 Docker
```bash
# Build and run
docker-compose up -d

# Run tests in Docker
docker-compose run api npm test
```

## 🤝 Contributing
1. Fork the repository
2. Create a feature branch
3. Commit changes
4. Push to branch
5. Create a Pull Request

## 📄 License
MIT License

---

Made with ❤️ by [Your Name]
