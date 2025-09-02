# Overview

Lubricentro R/18 is a Flask-based web application for an automotive lubricants and oils retail business. The system serves as a digital catalog and sales platform, showcasing various automotive products including motor oils, transmission fluids, greases, and hydraulic oils. The application provides multiple product viewing options (table and card layouts), detailed product information pages, and a purchase form system for customer orders.

# User Preferences

Preferred communication style: Simple, everyday language.

# System Architecture

## Frontend Architecture
- **Template Engine**: Jinja2 templating with Flask for server-side rendering
- **UI Framework**: Bootstrap 5 with dark theme for responsive design
- **Icon System**: Font Awesome for consistent iconography
- **Layout Strategy**: Base template inheritance pattern for consistent navigation and styling
- **View Modes**: Dual product display options (table view and card/box view) for different user preferences

## Backend Architecture
- **Web Framework**: Flask with minimal configuration for rapid development
- **Data Storage**: JSON file-based system (`data/products.json`) for product catalog
- **Session Management**: Flask's built-in session handling with configurable secret key
- **Error Handling**: Flash messaging system for user feedback and error communication
- **Logging**: Python's built-in logging module for debugging and monitoring

## Data Management
- **Product Data**: Static JSON file containing structured product information including specifications, pricing, and inventory
- **No Database**: File-based approach eliminates database complexity for small-scale deployment
- **Data Structure**: Products contain comprehensive details (ID, name, category, brand, price, specifications, stock levels)

## Application Structure
- **Route Organization**: RESTful URL patterns with clear separation of concerns
- **Static Assets**: CSS and JavaScript files organized in standard Flask static directory structure
- **Template Hierarchy**: Modular template system with base layout and specialized page templates

# External Dependencies

## Frontend Dependencies
- **Bootstrap 5**: CSS framework loaded via CDN for responsive design and components
- **Font Awesome 6.4.0**: Icon library via CDN for consistent iconography
- **Bootstrap Agent Dark Theme**: Specialized dark theme variant optimized for code environments

## Python Dependencies
- **Flask**: Core web framework for routing, templating, and request handling
- **Standard Library**: Uses built-in modules (os, json, logging) minimizing external dependencies

## Development Environment
- **Replit Integration**: Configured for Replit hosting environment with appropriate CDN resources
- **Environment Variables**: Session secret configuration through environment variables for security
- **Static File Serving**: Flask's built-in static file serving for CSS, JavaScript, and image assets

## No External Services
- No database connections required
- No external API integrations
- No payment processing systems
- No email services
- Self-contained application suitable for simple hosting environments