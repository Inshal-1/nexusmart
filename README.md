# NexusMart 🛒

NexusMart is a modern, multi-vendor e-commerce platform built with Next.js and Prisma. It empowers users to both shop for products and set up their own digital storefronts to sell directly to consumers.

## 🚀 Features

- **Multi-Vendor Architecture**: Users can register as sellers, create their own stores, and manage their own inventory.
- **Product Discovery**: Browse products through dynamic catalogs, best sellers, and latest arrivals.
- **Seamless Shopping Experience**: Robust cart management and checkout flows.
- **Order Management**: Track order statuses from processing to delivery.
- **Flexible Payments**: Support for multiple payment methods including Stripe and Cash on Delivery (COD).
- **Reviews & Ratings**: Verified buyers can leave reviews and ratings for products.
- **Coupon System**: Discount codes and promotional offers.
- **Responsive Design**: Fully responsive UI built with Tailwind CSS, ensuring a great experience on desktop and mobile.

## 🛠️ Tech Stack

- **Framework**: [Next.js 15](https://nextjs.org/) (App Router)
- **Frontend Library**: [React 19](https://react.dev/)
- **State Management**: [Redux Toolkit](https://redux-toolkit.js.org/)
- **Styling**: [Tailwind CSS v4](https://tailwindcss.com/)
- **Database**: [PostgreSQL](https://www.postgresql.org/)
- **ORM**: [Prisma](https://www.prisma.io/)
- **UI Components**: [Lucide React](https://lucide.dev/) for icons, [React Hot Toast](https://react-hot-toast.com/) for notifications, [Recharts](https://recharts.org/) for analytics dashboards.

## 📦 Getting Started

### Prerequisites

- Node.js (v18 or higher)
- npm or yarn
- PostgreSQL database

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/nexusmart.git
   cd nexusmart
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Configure Environment Variables:
   Create a `.env` file in the root directory based on `.env.example` and add your database credentials:
   ```env
   DATABASE_URL="postgresql://user:password@localhost:5432/nexusmart"
   DIRECT_URL="postgresql://user:password@localhost:5432/nexusmart"
   NEXT_PUBLIC_CURRENCY_SYMBOL="$"
   ```

4. Set up the Database:
   Generate Prisma client and push the schema to your database:
   ```bash
   npx prisma generate
   npx prisma db push
   ```

5. Start the development server:
   ```bash
   npm run dev
   ```

6. Open [http://localhost:3000](http://localhost:3000) in your browser to see the result.

## 📁 Project Structure

- `app/`: Next.js App Router routes (public pages, admin dashboards, store dashboards).
- `components/`: Reusable React components (Hero, BestSelling, Newsletter, etc.).
- `lib/`: Utility functions and shared logic.
- `prisma/`: Prisma schema and database configuration.
- `assets/`: Static assets like images.

## 📝 License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## 🤝 Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
