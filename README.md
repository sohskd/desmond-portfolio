# Desmond Soh - Portfolio Website

A modern, responsive portfolio website for freelance software engineer Desmond Soh.

## Features

- **Responsive Design**: Works perfectly on all devices and screen sizes
- **Contact Form**: Functional contact form powered by Resend API
- **Portfolio Showcase**: Display of recent projects and work
- **Professional Services**: Clear presentation of offered services
- **Modern UI**: Clean, professional design with smooth interactions

## Technologies Used

- HTML5, CSS3, JavaScript
- Resend API for email functionality
- Vercel for deployment
- Font Awesome icons
- Google Fonts (Inter)

## Setup Instructions

### 1. Clone the Repository
```bash
git clone <repository-url>
cd desmond-portfolio
```

### 2. Install Dependencies
```bash
npm install
```

### 3. Environment Variables
1. Copy `.env.example` to `.env.local`
2. Get your Resend API key from [https://resend.com/api-keys](https://resend.com/api-keys)
3. Add your API key to `.env.local`:
```
RESEND_API_KEY=your_actual_api_key_here
```

### 4. Domain Setup (Important!)
- For production: Verify your domain at [https://resend.com/domains](https://resend.com/domains)
- For testing: You can use `resend.dev` domain
- Update the `from` field in `/api/contact.js` with your verified domain

### 5. Run Development Server
```bash
npm run dev
```

### 6. Deploy to Vercel
```bash
vercel --prod
```

## Contact Form Configuration

The contact form sends emails to: `DSOH005@e.ntu.edu.sg`

To change the recipient email, update the `to` field in `/api/contact.js`.

## File Structure

```
├── api/
│   └── contact.js          # Resend API endpoint
├── images/
│   ├── profile.jpg         # Profile picture
│   └── ember-&-oak.jpg     # Portfolio project image
├── index.html              # Main HTML file
├── styles.css              # CSS styles
├── script.js               # JavaScript functionality
├── package.json            # Dependencies
├── .env.example            # Environment variables template
└── README.md               # This file
```

## Customization

### Adding New Portfolio Items
1. Add project details in the portfolio section of `index.html`
2. Add project images to the `images/` directory
3. Update the portfolio grid CSS if needed

### Modifying Services
Edit the services section in `index.html` to add/remove/modify offered services.

### Styling Changes
All styles are in `styles.css`. The design uses a modern color scheme with:
- Primary: #2563eb (blue)
- Background: #f8fafc (light gray)
- Text: #1e293b (dark gray)

## Contact Information

- **Email**: DSOH005@e.ntu.edu.sg
- **Phone**: +6598772276
- **Location**: Singapore

## License

MIT License - feel free to use this template for your own portfolio!
