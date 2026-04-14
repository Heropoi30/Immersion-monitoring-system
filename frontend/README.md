# Work Immersion System - Frontend

A comprehensive web application for managing student work immersion programs, built with React and Vite. This frontend provides intuitive dashboards for students, teachers, and administrators to track attendance, submit reports, and manage program activities.

## Features

### Student Dashboard
- **Attendance Tracking**: Mark AM/PM time-in and time-out with automated session management
- **Report Management**: Create, edit, submit, and track progress reports with file attachments
- **Profile Management**: Update personal information and profile pictures
- **Analytics**: View attendance rates, total hours, and progress visualizations
- **Notifications**: Real-time updates for important events

### Teacher Dashboard
- **Student Oversight**: View and manage assigned students
- **Attendance Monitoring**: Track student attendance across sessions
- **Report Grading**: Review and grade submitted student reports
- **Session Management**: Start AM/PM attendance sessions
- **Analytics**: View attendance summaries and student performance metrics

### Admin Dashboard
- **User Management**: Create, update, and manage student and teacher accounts
- **System Reports**: Generate attendance reports and user statistics
- **Configuration**: Manage system settings and permissions
- **Data Export**: Export reports and analytics data

## Tech Stack

- **Frontend Framework**: React 18 with Hooks
- **Build Tool**: Vite for fast development and optimized production builds
- **Styling**: Custom CSS with responsive design
- **HTTP Client**: Axios for API communication
- **State Management**: React Context for global state
- **Routing**: React Router for navigation
- **Icons**: Custom SVG icons and illustrations

## Installation

1. **Prerequisites**
   - Node.js 18+ and npm
   - Backend API server running (see backend README)

2. **Clone and Install**
   ```bash
   cd frontend
   npm install
   ```

3. **Environment Setup**
   Create a `.env` file in the frontend directory:
   ```env
   VITE_API_BASE_URL=http://localhost:3000/api/v1
   ```

4. **Start Development Server**
   ```bash
   npm run dev
   ```

5. **Build for Production**
   ```bash
   npm run build
   ```

## Usage

### Authentication
- Students, teachers, and admins use separate login portals
- JWT tokens are used for session management
- Automatic logout on token expiration

### Navigation
- Responsive sidebar navigation with hover effects
- Mobile-friendly burger menu
- Keyboard navigation support

### Dark Mode
- Toggle between light and dark themes
- Preference saved in localStorage
- Consistent theming across all components

## API Integration

This frontend communicates with a REST API built with Express.js. See `../API_DOCUMENTATION.md` for detailed endpoint documentation including:

- Authentication endpoints
- User management APIs
- Attendance tracking APIs
- Report management APIs

## Project Structure

```
frontend/
├── src/
│   ├── components/
│   │   ├── common/          # Reusable UI components
│   │   └── layout/          # Layout components
│   ├── context/             # React Context providers
│   ├── pages/               # Page components
│   ├── routes/              # Route configurations
│   ├── services/            # API service functions
│   └── styles/              # CSS stylesheets
├── public/                  # Static assets
└── README.md
```

## Development

### Available Scripts
- `npm run dev` - Start development server with hot reload
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint

### Code Style
- Follows React best practices
- Uses functional components with hooks
- Consistent naming conventions
- Responsive design principles

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Support

For support and questions, please open an issue in the GitHub repository or contact the development team.
