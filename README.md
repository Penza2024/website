# Mapalo Musonda - Portfolio Website

A modern, responsive portfolio website built with HTML, Tailwind CSS, and vanilla JavaScript.

## Features

- 📱 Fully responsive design
- 🎨 Modern UI with smooth animations
- 📝 Blog & Publications section
- 🏆 Certificates showcase
- 💼 Project portfolio
- 🛠️ Skills & technologies display
- 📧 Contact form with newsletter subscription
- 🌓 Theme toggle (light/dark mode)
- ⬆️ Scroll to top button

## Structure

```
website/
├── index.html          # Main portfolio page
├── images/            # Images and assets
│   ├── profilePicture.jpg
│   ├── blog.pdf
│   ├── certificate1.png
│   ├── certificate4.png
│   └── Chart.png
└── README.md          # This file
```

## Technologies Used

- HTML5
- Tailwind CSS (via CDN)
- JavaScript (Vanilla)
- Remix Icons
- Google Fonts (Inter, Pacifico)

## Deployment

This website is deployed on Cloudflare Pages.

### Deploy to Cloudflare Pages

1. Create a GitHub repository and push this code
2. Log in to [Cloudflare Pages](https://pages.cloudflare.com/)
3. Connect your GitHub account
4. Select this repository
5. Configure the build settings:
   - Build command: (leave empty)
   - Build output directory: `/`
6. Deploy!

Alternatively, you can use Wrangler CLI:

```bash
npm install -g wrangler
wrangler pages deploy .
```

## Local Development

Simply open `index.html` in your web browser to view the website locally.

Alternatively, you can use a local server:

```bash
# Using Python
python3 -m http.server 8000

# Using Node.js http-server
npx http-server -p 8000
```

Then visit `http://localhost:8000` in your browser.

## Contact

- Email: mapalomusondapenza@gmail.com
- GitHub: [@Penza2024](https://github.com/Penza2024)
- LinkedIn: [Mapalo Musonda](https://www.linkedin.com/in/mapalo-musonda-731815226)
- Dev.to: [@mapalo_musonda_ad42ad37a8](https://dev.to/mapalo_musonda_ad42ad37a8)

## License

© 2025 Mapalo Penza. All rights reserved.
