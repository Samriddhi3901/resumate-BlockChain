# Resumate - VIT Bhopal Resume Builder📄✨
A specialized resume building web application designed specifically for VIT Bhopal students, featuring the official institutional template and streamlined resume creation process.

## 🌟 Overview

Resumate is a full-stack web application tailored exclusively for VIT Bhopal students. It provides an intuitive interface to create professional resumes using the official VIT Bhopal template, ensuring consistency and professionalism for all students during placement and job application processes.

## ✨ Features

- **🏛️ Official VIT Bhopal Template**: Pre-designed resume format following institutional guidelines
- **📝 Easy Form Interface**: Simple, step-by-step resume creation process
- **📱 Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **💾 Auto-Save**: Automatic saving of progress to prevent data loss
- **📤 Multiple Export Options**: Download as PDF or share via link
- **🎓 Academic Integration**: Pre-filled VIT Bhopal academic structure and courses
- **📊 Real-time Preview**: Live preview of resume as you build it
- **🔄 Version Control**: Save and manage multiple versions of your resume
- **📧 Direct Sharing**: Share resume link directly with recruiters
- **👤 User Profiles**: Personal dashboard to manage multiple resumes
- **📈 Analytics**: Track resume views and download statistics

## 🎯 Target Audience

- VIT Bhopal undergraduate students
- VIT Bhopal postgraduate students
- VIT Bhopal alumni
- Career services department
- Campus placement coordinators

## 🛠️ Technology Stack

### Frontend
- **Framework**: React.js
- **Styling**: Tailwind CSS / CSS3
- **State Management**: React Context API / Redux
- **Form Handling**: Formik / React Hook Form
- **PDF Generation**: jsPDF / React-PDF
- **Icons**: Lucide React / Font Awesome

### Backend
- **Runtime**: Node.js
- **Framework**: Express.js
- **Database**: MongoDB / PostgreSQL
- **Authentication**: JWT (JSON Web Tokens)
- **File Storage**: Cloudinary / AWS S3
- **Email Service**: Nodemailer / SendGrid

### Development Tools
- **Version Control**: Git
- **Package Manager**: npm / yarn
- **Code Formatting**: Prettier
- **Linting**: ESLint
- **Testing**: Jest, React Testing Library

## 🚀 Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn
- MongoDB (for local development) or MongoDB Atlas
- Git

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Samriddhi3901/resumate-BlockChain.git
   cd resumate-BlockChain
   ```

2. **Install backend dependencies**
   ```bash
   cd backend
   npm install
   ```

3. **Install frontend dependencies**
   ```bash
   cd ../frontend
   npm install
   ```

4. **Environment Setup**
   
   **Backend (.env)**
   ```env
   PORT=5000
   NODE_ENV=development
   MONGODB_URI=mongodb://localhost:27017/resumate
   JWT_SECRET=your_jwt_secret_key
   JWT_EXPIRE=7d
   EMAIL_HOST=smtp.gmail.com
   EMAIL_PORT=587
   EMAIL_USER=your_email@gmail.com
   EMAIL_PASS=your_email_password
   CLOUDINARY_NAME=your_cloudinary_name
   CLOUDINARY_API_KEY=your_cloudinary_key
   CLOUDINARY_API_SECRET=your_cloudinary_secret
   ```

   **Frontend (.env)**
   ```env
   REACT_APP_API_URL=http://localhost:5000/api
   REACT_APP_APP_NAME=Resumate VIT Bhopal
   ```

5. **Start the development servers**
   
   **Backend**
   ```bash
   cd backend
   npm run dev
   ```
   
   **Frontend** (in new terminal)
   ```bash
   cd frontend
   npm start
   ```

6. **Open your browser**
   Navigate to `http://localhost:3000`

## 📖 How to Use

### Step 1: Registration/Login
- Sign up with your VIT Bhopal email ID
- Verify your account via email
- Login to access the resume builder

### Step 2: Personal Information
- Fill in your basic details (Name, Email, Phone, Address)
- Upload your profile photo
- Enter your VIT Bhopal registration number

### Step 3: Academic Details
- Select your program (B.Tech, M.Tech, MBA, etc.)
- Choose your specialization/branch
- Enter your CGPA and semester details
- Add relevant coursework and academic projects

### Step 4: Experience & Internships
- Add internships and work experience
- Include company details, duration, and responsibilities
- Mention technologies used and key achievements

### Step 5: Projects & Skills
- Add academic and personal projects
- List technical and soft skills
- Include certifications and online courses

### Step 6: Achievements & Activities
- Add awards and recognitions
- Include extracurricular activities
- Mention leadership roles and volunteer work

### Step 7: Generate & Export
- Preview your resume in real-time
- Make final adjustments to formatting
- Download as PDF or share via unique link
- Save multiple versions for different applications

## 🏗️ Project Structure

```
resumate-BlockChain/
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   │   ├── Auth/           # Login/Register components
│   │   │   ├── Dashboard/      # User dashboard
│   │   │   ├── ResumeBuilder/  # Step-by-step form components
│   │   │   ├── ResumePreview/  # Live preview component
│   │   │   ├── Templates/      # VIT Bhopal template
│   │   │   └── Shared/         # Reusable UI components
│   │   ├── pages/
│   │   │   ├── Home.js         # Landing page
│   │   │   ├── Builder.js      # Main resume builder
│   │   │   ├── Dashboard.js    # User dashboard
│   │   │   └── Preview.js      # Resume preview page
│   │   ├── context/            # React Context for state management
│   │   ├── utils/
│   │   │   ├── api.js          # API calls
│   │   │   ├── pdfGenerator.js # PDF generation
│   │   │   └── validation.js   # Form validations
│   │   ├── styles/
│   │   │   └── vitTemplate.css # VIT template styles
│   │   └── assets/
│   │       ├── vit-logo.png    # Official VIT Bhopal logo
│   │       └── images/         # Other assets
│   ├── public/
│   └── package.json
├── backend/
│   ├── controllers/            # Route controllers
│   │   ├── auth.js            # Authentication logic
│   │   ├── resume.js          # Resume CRUD operations
│   │   └── user.js            # User management
│   ├── models/                # Database schemas
│   │   ├── User.js            # User model
│   │   └── Resume.js          # Resume model
│   ├── routes/                # API routes
│   │   ├── auth.js            # Auth routes
│   │   ├── resume.js          # Resume routes
│   │   └── user.js            # User routes
│   ├── middleware/            # Custom middleware
│   │   ├── auth.js            # JWT authentication
│   │   └── validation.js      # Request validation
│   ├── utils/                 # Utility functions
│   │   ├── database.js        # DB connection
│   │   ├── email.js           # Email utilities
│   │   └── fileUpload.js      # File handling
│   ├── config/                # Configuration files
│   └── server.js              # Main server file
├── docs/                      # Documentation
└── README.md
```

## 🎨 VIT Bhopal Template Features

### Official Branding
- VIT Bhopal logo and institutional colors
- Standardized header with university information
- Consistent typography and layout

### Academic Structure
- Pre-configured course codes for all programs
- Semester-wise grade display format
- CGPA calculation and display
- Branch-specific coursework templates

### Sections Layout
1. **Header**: Name, contact, and VIT registration details
2. **Objective/Summary**: Career objective section
3. **Education**: Academic background with VIT details
4. **Technical Skills**: Programming languages, tools, technologies
5. **Projects**: Academic and personal project details
6. **Experience**: Internships and work experience
7. **Achievements**: Awards, certifications, publications
8. **Extracurricular**: Activities, leadership roles, volunteering

## 🔧 API Endpoints

### Authentication
- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login
- `POST /api/auth/verify-email` - Email verification
- `POST /api/auth/forgot-password` - Password reset

### Resume Management
- `GET /api/resumes` - Get user's resumes
- `POST /api/resumes` - Create new resume
- `GET /api/resumes/:id` - Get specific resume
- `PUT /api/resumes/:id` - Update resume
- `DELETE /api/resumes/:id` - Delete resume
- `GET /api/resumes/:id/pdf` - Generate PDF

### User Profile
- `GET /api/users/profile` - Get user profile
- `PUT /api/users/profile` - Update profile
- `POST /api/users/upload-photo` - Upload profile photo

## 🧪 Testing

### Backend Tests
```bash
cd backend
npm run test
npm run test:watch
```

### Frontend Tests
```bash
cd frontend
npm run test
npm run test:coverage
```

### Integration Tests
```bash
npm run test:integration
```

## 🚀 Deployment

### Development Build
```bash
# Build frontend
cd frontend
npm run build

# Start production server
cd ../backend
npm start
```

### Production Deployment

**Using Docker**
```bash
docker build -t resumate-vit .
docker run -p 3000:3000 resumate-vit
```

**Using PM2**
```bash
npm install -g pm2
pm2 start ecosystem.config.js
```

## 🔒 Security Features

- JWT-based authentication
- Password hashing with bcrypt
- Input validation and sanitization
- Rate limiting on API endpoints
- CORS configuration
- File upload restrictions
- XSS and injection attack prevention

## 🤝 Contributing

We welcome contributions from VIT Bhopal students and developers!

### How to Contribute
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Make your changes
4. Write or update tests
5. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
6. Push to the branch (`git push origin feature/AmazingFeature`)
7. Open a Pull Request

### Contribution Guidelines
- Follow the existing code style
- Write meaningful commit messages
- Add tests for new features
- Update documentation as needed
- Ensure all tests pass

## 📞 Support & Contact

### For Students
- **Email**: support@resumate-vit.com
- **Campus**: Visit Career Services Department
- **GitHub Issues**: [Create an issue](https://github.com/Samriddhi3901/resumate-BlockChain/issues)

### Technical Support
- Include your VIT registration number
- Provide browser and device information
- Describe the issue with screenshots if possible

## 📋 Roadmap

### Phase 1 (Completed)
- [x] User authentication system
- [x] Basic resume builder with VIT template
- [x] PDF generation and download
- [x] Responsive design

### Phase 2 (In Progress)
- [ ] Advanced template customization
- [ ] Resume analytics dashboard
- [ ] Email integration for sharing
- [ ] Mobile application

### Phase 3 (Planned)
- [ ] Integration with VIT placement portal
- [ ] Faculty recommendation system
- [ ] Company-specific resume templates
- [ ] AI-powered content suggestions
- [ ] Bulk resume generation for placement drives

## 📊 Features Overview

| Feature | Status | Description |
|---------|--------|-------------|
| User Registration | ✅ | Email-based account creation |
| Resume Builder | ✅ | Step-by-step form interface |
| VIT Template | ✅ | Official institutional format |
| PDF Export | ✅ | High-quality PDF generation |
| Auto-Save | ✅ | Automatic progress saving |
| Multiple Versions | ✅ | Save different resume versions |
| Analytics | 🚧 | View and download tracking |
| Mobile App | 📝 | Native mobile application |

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **VIT Bhopal** - For institutional support and template guidelines
- **Career Services Department** - For requirements and feedback
- **Student Community** - For testing and feature suggestions
- **Open Source Libraries** - All the amazing
