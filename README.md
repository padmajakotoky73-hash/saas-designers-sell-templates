```markdown
# SaaS Designers - Sell Templates

![License](https://img.shields.io/badge/license-MIT-blue)
![Stack](https://img.shields.io/badge/stack-Next.js%20%2B%20FastAPI-orange)

A SaaS platform enabling designers to sell their templates with ease.

## Features

- Designer profile management
- Template upload & management
- Secure payment processing
- Responsive design for all devices
- Template preview functionality

## Quick Start

1. Clone the repo:
   ```bash
   git clone https://github.com/your-repo/saas-designers-sell-templates.git
   cd saas-designers-sell-templates
   ```

2. Install dependencies:
   ```bash
   # Frontend
   cd frontend && npm install
   
   # Backend
   cd ../backend && pip install -r requirements.txt
   ```

## Environment Setup

Create `.env` files in both `/frontend` and `/backend` with these variables:

**Frontend (.env):**
```env
NEXT_PUBLIC_API_URL=http://localhost:8000
NEXT_PUBLIC_STRIPE_KEY=your_stripe_key
```

**Backend (.env):**
```env
DATABASE_URL=postgresql://user:password@localhost:5432/template_db
SECRET_KEY=your_secret_key
STRIPE_SECRET_KEY=your_stripe_secret
```

## Deployment

1. **Frontend (Vercel):**
   ```bash
   vercel
   ```

2. **Backend (Render/DigitalOcean):**
   ```bash
   gunicorn main:app --workers 4 --worker-class uvicorn.workers.UvicornWorker
   ```

## License

MIT License - see [LICENSE](LICENSE) for details.
```