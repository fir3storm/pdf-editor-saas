# PDF Editor SaaS

A modern SaaS application that allows users to upload and edit PDF files. Free tier users can edit one PDF, while premium users get unlimited edits for $40/year.

## Features

- PDF upload and editing
- Free tier with one edit
- Premium subscription ($40/year) with unlimited edits
- Secure file handling
- Modern, responsive UI
- Stripe integration for payments

## Tech Stack

- Next.js 14 with App Router
- TypeScript
- Tailwind CSS
- Shadcn UI Components
- Stripe for payments
- PDF.js for PDF handling

## Getting Started

1. Clone the repository:
\`\`\`bash
git clone <repository-url>
cd pdf-editor-saas
\`\`\`

2. Install dependencies:
\`\`\`bash
npm install
\`\`\`

3. Set up environment variables:
Create a .env.local file with the following variables:
\`\`\`
STRIPE_SECRET_KEY=your_stripe_secret_key
STRIPE_WEBHOOK_SECRET=your_stripe_webhook_secret
NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY=your_stripe_publishable_key
NEXT_PUBLIC_APP_URL=http://localhost:8000
\`\`\`

4. Start the development server:
\`\`\`bash
npm run dev
\`\`\`

The application will be available at http://localhost:8000

## Project Structure

- `/src/app` - Next.js app router pages and API routes
- `/src/components` - React components including UI components
- `/src/lib` - Utility functions and shared logic
- `/public/uploads` - Directory for uploaded PDF files

## API Routes

- `POST /api/upload` - Upload PDF files
- `POST /api/subscription` - Handle subscription creation
- `POST /api/subscription/webhook` - Handle Stripe webhooks

## Environment Variables

- `STRIPE_SECRET_KEY` - Your Stripe secret key
- `STRIPE_WEBHOOK_SECRET` - Stripe webhook secret for verifying webhook events
- `NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY` - Your Stripe publishable key
- `NEXT_PUBLIC_APP_URL` - The base URL of your application

## Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a new Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.
