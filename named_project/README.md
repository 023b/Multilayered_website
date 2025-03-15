# Project Selection Platform

A comprehensive web application that allows users to register and select from various project templates for rapid development.

## Project Overview

This platform provides a streamlined process for users to register their information and browse through different project templates including personal portfolios, blogs, e-commerce sites, and polling applications. Users can select their preferred project type and get started quickly with pre-designed templates.

## Directory Structure

```
named_project/
├── data/
│   └── formData.json        # Storage for user registration data
├── images/                  # Directory for project images and assets
├── README.md                # This documentation file
├── base.html                # Base template for other HTML files
├── blog.html                # Blog project template
├── documentation.pdf        # Detailed project documentation
├── e-commerce.html          # E-commerce project template
├── index.html               # Registration form landing page
├── personal_portfolio.html  # Personal portfolio template
├── polling.html             # Polling application template
├── project_selection.html   # Project selection interface
└── server.js                # Node.js server for handling form submissions
```

## Features

- **User Registration**: Collects user information through a form
- **Data Storage**: Saves registration data in JSON format
- **Multiple Project Templates**: 
  - Personal Portfolio
  - Blog
  - E-commerce
  - Polling Application
- **Project Selection Interface**: Easy browsing and selection of project templates
- **Backend Support**: Node.js server for data handling and storage

## Technology Stack

- **Frontend**: HTML5, CSS3, JavaScript
- **Backend**: Node.js, Express
- **Data Storage**: JSON file-based storage
- **Design**: Responsive design principles, modern UI/UX

## Getting Started

### Prerequisites

- Node.js (v12.0.0 or higher)
- NPM (v6.0.0 or higher)

### Installation

1. Clone the repository
   ```
   git clone https://github.com/yourusername/named_project.git
   cd named_project
   ```

2. Install dependencies
   ```
   npm install express body-parser cors fs
   ```

3. Start the server
   ```
   node server.js
   ```

4. Open your browser and navigate to:
   ```
   http://localhost:3000
   ```

## Usage Guide

### Registration Process

1. Open `index.html` in your browser
2. Fill out the registration form with your information
3. Click "Submit" to save your data
4. You will be redirected to the project selection page

### Project Selection

1. Browse through available project templates on `project_selection.html`
2. Click on any project card to view more details
3. Select your preferred project by clicking the associated button
4. Follow the on-screen instructions to initialize your selected project

### Available Templates

#### Personal Portfolio
A clean, responsive portfolio template designed for showcasing personal work, skills, and experiences.

#### Blog
A fully-featured blog template with article layout, commenting system, and category organization.

#### E-commerce
A complete online store template with product listings, shopping cart, and checkout process.

#### Polling Application
An interactive polling system for creating surveys, gathering votes, and visualizing results.

## Server Configuration

The `server.js` file manages backend operations including:

- Handling form submissions from the registration page
- Storing user data in `data/formData.json`
- Serving appropriate project templates based on user selection
- Managing static file delivery

Default configuration:
- Server port: 3000
- Data storage: `./data/formData.json`

## Customization

### Modifying Templates

Each project template can be customized by editing the corresponding HTML file:
- `personal_portfolio.html`
- `blog.html`
- `e-commerce.html`
- `polling.html`

All templates inherit styles and common elements from `base.html`.

### Adding New Templates

To add a new project template:

1. Create a new HTML file based on `base.html`
2. Add the template to the project selection interface in `project_selection.html`
3. Update the server routes in `server.js` if necessary

## Development

### Extending the Platform

For developers looking to extend the platform:

1. **Adding Backend Functionality**:
   - Extend server.js with additional routes
   - Implement database connections instead of file-based storage

2. **Enhancing UI/UX**:
   - Modify CSS styles in each template
   - Add JavaScript interactions and animations

3. **Implementing Authentication**:
   - Add user login/registration system
   - Implement session management

## Documentation

For detailed documentation on all features and implementation details, refer to `documentation.pdf` included in the project.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contributors

- [Your Name](https://github.com/yourusername)

## Acknowledgments

- Thanks to all open-source projects that inspired this work
- Special thanks to contributors and testers who helped refine this platform
