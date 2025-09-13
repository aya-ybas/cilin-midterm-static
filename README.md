# Coffee World - Static Website

A beautiful, responsive coffee-themed website showcasing different types of coffee and coffee facts.

## Files Structure

- `index.html` - Main HTML file (converted from index.php)
- `styles.css` - CSS styles for the website
- `Dockerfile` - Docker configuration for deployment
- `nginx.conf` - Nginx configuration for serving static files

## Deployment to Coolify

### Option 1: Docker Deployment (Recommended)

1. **Push your code to a Git repository** (GitHub, GitLab, etc.)

2. **In Coolify:**
   - Create a new application
   - Choose "Docker" as the deployment type
   - Connect your Git repository
   - Coolify will automatically detect the Dockerfile

3. **Deploy:**
   - Coolify will build the Docker image using the provided Dockerfile
   - The application will be served using Nginx on port 80

### Option 2: Static Site Deployment

If you prefer not to use Docker:

1. **In Coolify:**
   - Create a new application
   - Choose "Static Site" as the deployment type
   - Upload your files: `index.html` and `styles.css`
   - Set the entry point to `index.html`

### Option 3: Simple HTTP Server

For local testing or simple deployments:

```bash
# Using Python (if installed)
python -m http.server 8000

# Using Node.js (if installed)
npx serve .

# Using PHP (if installed)
php -S localhost:8000
```

## Features

- **Responsive Design**: Works on desktop, tablet, and mobile devices
- **Smooth Scrolling**: Navigation with smooth scroll effects
- **Interactive Elements**: Hover effects and animations
- **Modern UI**: Clean, coffee-themed design with gradients and shadows
- **Performance Optimized**: Compressed assets and efficient CSS

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## Customization

To customize the website:

1. **Colors**: Modify the CSS variables in `styles.css`
2. **Content**: Edit the HTML content in `index.html`
3. **Styling**: Update the CSS classes and styles in `styles.css`

## Troubleshooting

### Common Issues:

1. **CSS not loading**: Ensure `styles.css` is in the same directory as `index.html`
2. **Images not showing**: Check file paths and ensure images are in the correct directory
3. **Deployment issues**: Verify that all files are included in your deployment

### Coolify Specific:

- Make sure your repository is public or you have proper access configured
- Check the build logs in Coolify for any error messages
- Ensure the Dockerfile is in the root directory of your repository
