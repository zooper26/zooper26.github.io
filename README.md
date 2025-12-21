# zooper26.github.io

## Secure Editor with SSL

A barebones secure login interface built with open source technologies for easy user editing.

### Features

- 🔒 **SSL/HTTPS Encryption**: Automatically enabled via GitHub Pages
- 🛡️ **Security Headers**: Content Security Policy, XSS Protection, and more
- 👤 **User Authentication**: Secure login interface with session management
- ✏️ **Content Editor**: Simple text editor with auto-save functionality
- 💾 **Local Storage**: Content persists between sessions
- 📱 **Responsive Design**: Works on all devices

### Demo Credentials

- **Username**: `admin`
- **Password**: `demo123`

### SSL Certificate Configuration

GitHub Pages automatically provides SSL certificates for custom domains. To enable HTTPS:

1. **Configure Custom Domain**:
   - Go to Repository Settings → Pages
   - Enter your custom domain (e.g., `triadsystems.tech`)
   - Save the configuration

2. **Update DNS Records**:
   - Add an A record pointing to GitHub Pages IPs:
     - `185.199.108.153`
     - `185.199.109.153`
     - `185.199.110.153`
     - `185.199.111.153`
   - Or add a CNAME record pointing to `zooper26.github.io`

3. **Enable HTTPS**:
   - GitHub Pages will automatically provision an SSL certificate
   - Check "Enforce HTTPS" in Repository Settings → Pages
   - Certificate issuance may take up to 24 hours

### Security Features

- **Automatic HTTPS Redirect**: Forces secure connections
- **Content Security Policy**: Prevents XSS attacks
- **Session Management**: Secure 24-hour sessions
- **Input Sanitization**: All user input is sanitized
- **XSS Protection Headers**: Additional security layer

### Technologies Used

- Pure HTML5, CSS3, and JavaScript (no dependencies)
- localStorage API for data persistence
- Open source and fully customizable

### Local Development

Simply open `index.html` in a web browser. For full SSL testing, deploy to GitHub Pages.

### License

Open Source - Free to use and modify