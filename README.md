# Angular 21 Boilerplate

A complete Angular 21 boilerplate application with authentication, admin dashboard, and user account management.

## Prerequisites

Before running this project, make sure you have the following installed:

- **Node.js** (v14.0.0 or higher) - [Download](https://nodejs.org/)
- **npm** (v6.0.0 or higher) - Comes with Node.js
- **Angular CLI** (v21.0.0 or higher)

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/johnpaultaray/angular-21-boilerplate.git
   cd angular-21-boilerplate
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Install Angular CLI globally** (if not already installed)
   ```bash
   npm install -g @angular/cli
   ```

## Running the Application

### Development Server

Start the development server with hot-reload:

```bash
ng serve
```

or

```bash
npm start
```

The application will be available at **http://localhost:4200**

### Production Build

Create an optimized production build:

```bash
ng build --prod
```

The build artifacts will be stored in the `dist/` directory.

### Running Tests

Execute unit tests via Karma:

```bash
ng test
```

## Project Structure

```
src/app/
├── _components/          # Shared components (e.g., alert component)
├── _helpers/             # Utility helpers (guards, interceptors, validators)
├── _models/              # Data models (Account, Alert, Role)
├── _services/            # Services (Account service, Alert service)
├── account/              # Account module (login, register, password reset, etc.)
├── admin/                # Admin module (account management)
├── home/                 # Home module
└── profile/              # Profile module
```

## Key Features

- ✅ User Authentication & Authorization
- ✅ JWT Token Management
- ✅ Role-based Access Control
- ✅ Admin Dashboard
- ✅ Account Management
- ✅ Error Handling & Interceptors
- ✅ Form Validation
- ✅ Alert/Notification System

## Configuration Files

- `angular.json` - Angular CLI configuration
- `tsconfig.json` - TypeScript compiler options
- `package.json` - Project dependencies and scripts
- `styles.less` - Global styles

## Troubleshooting

### Port Already in Use
If port 4200 is already in use, specify a different port:
```bash
ng serve --port 4300
```

### Dependencies Issues
Clear npm cache and reinstall:
```bash
npm cache clean --force
rm -rf node_modules package-lock.json
npm install
```

### Angular CLI Version Mismatch
Update Angular CLI globally:
```bash
npm install -g @angular/cli@latest
```

## License

This project is open source and available under the MIT License.
