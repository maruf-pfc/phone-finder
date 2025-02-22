# Phone Finder

Phone Finder is a mobile e-commerce platform that helps user find products through personal recommendations and community insights. Built with Next.js and React, this platform delivers a seamless shopping experience with intelligent product matching and social features.

## Description

Phone Finder revolutionizes mobile phone shopping by combining e-commerce with crowd-sourced insights. Our platform features:
- Personalized product recommendations based on user preferences
- Community-driven reviews and insights
- Smart price comparison and tracking
- Seamless e-commerce experience for mobile phone purchases
- Active community engagement and discussion features

## Installation

To get started with Phone Finder, follow these steps:

1. Clone the repository:
```bash
git clone https://github.com/yourusername/phone-finder.git
cd phone-finder
```

2. Install dependencies using pnpm:
```bash
pnpm install
```

3. Set up environment variables:
```bash
cp .env.example .env.local
```
Then edit `.env.local` with your configuration values.

## Technologies

This project is built using modern tools and technologies:

- **Frontend Framework**: Next.js 15.1.7
- **UI Library**: React 19
- **Language**: TypeScript
- **Styling**: TailwindCSS
- **Database**: MongoDB with Mongoose ORM
- **Testing**: Jest
- **Code Quality**: ESLint

### Additional Packages
- Stripe for payment processing
- Nodemailer for email notifications
- Axios for HTTP requests
- React Query for server state management
- Zod for schema validation

## Development Scripts

Run the project locally with the following commands:

```bash
# Start development server
pnpm dev

# Build for production
pnpm build

# Start production server
pnpm start

# Run tests
pnpm test

# Run linting
pnpm lint
```

The development server will be available at [http://localhost:3000](http://localhost:3000).

## Contributing

Contributions are welcome! Please read our contributing guidelines before submitting a pull request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
