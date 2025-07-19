# AnimeTVStream - Anime Streaming Website Clone

A fully functional anime streaming website built with Next.js 15, TypeScript, and Tailwind CSS. This project is a modern clone of 9animetv.to with enhanced features, SEO optimization, and a clean, responsive design.

## 🚀 Features

### Core Functionality
- **Responsive Design**: Mobile-first approach with Tailwind CSS
- **Dynamic Routing**: Genre, type, and anime detail pages
- **Search Functionality**: Real-time anime search with filters
- **User Authentication**: Login, registration, and password reset
- **Modern UI/UX**: Clean, minimalist design with smooth animations

### Pages & Components
- **Homepage**: Hero section, featured anime grid, about section, FAQ
- **Genre Pages**: Filter anime by 40+ genres (Action, Adventure, Romance, etc.)
- **Type Pages**: Filter by anime types (Movies, TV Series, OVAs, ONAs, Specials)
- **Anime Detail Pages**: Complete anime information with streaming interface
- **Search Results**: Advanced search with pagination and sorting
- **Authentication Modals**: Login, register, and password reset forms

### Technical Features
- **Next.js 15**: Latest features with App Router and Server Components
- **TypeScript**: Full type safety throughout the application
- **Tailwind CSS**: Utility-first CSS framework for rapid development
- **SEO Optimized**: Meta tags, Open Graph, and structured data
- **API Routes**: RESTful API for authentication and data management
- **Mock Data**: Comprehensive anime database with 8+ sample anime
- **Ad Integration**: Ready-to-use ad banner components for monetization

## 🛠️ Tech Stack

- **Framework**: Next.js 15.4.2
- **Language**: TypeScript
- **Styling**: Tailwind CSS 4.x
- **Authentication**: JWT with bcryptjs
- **HTTP Client**: Axios
- **Fonts**: Inter (Google Fonts)
- **Development**: ESLint, Turbopack

## 📦 Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd animetvstream
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up environment variables**
   ```bash
   cp .env.local.example .env.local
   ```
   
   Update `.env.local` with your configuration:
   ```env
   JWT_SECRET=your-super-secret-jwt-key-here
   NEXTAUTH_SECRET=your-nextauth-secret-here
   NEXTAUTH_URL=http://localhost:3000
   ```

4. **Run the development server**
   ```bash
   npm run dev
   ```

5. **Open your browser**
   Navigate to [http://localhost:3000](http://localhost:3000)

## 🏗️ Project Structure

```
animetvstream/
├── src/
│   ├── app/                    # Next.js App Router
│   │   ├── api/               # API routes
│   │   │   ├── auth/          # Authentication endpoints
│   │   │   └── anime/         # Anime data endpoints
│   │   ├── anime/[id]/        # Dynamic anime detail pages
│   │   ├── genre/[slug]/      # Dynamic genre pages
│   │   ├── type/[type]/       # Dynamic type pages
│   │   ├── search/            # Search results page
│   │   ├── layout.tsx         # Root layout
│   │   ├── page.tsx           # Homepage
│   │   └── globals.css        # Global styles
│   ├── components/            # Reusable components
│   │   ├── Header.tsx         # Navigation header
│   │   ├── Footer.tsx         # Site footer
│   │   ├── AuthModal.tsx      # Authentication modals
│   │   ├── AnimeCard.tsx      # Anime display card
│   │   └── AdBanner.tsx       # Advertisement component
│   ├── lib/                   # Utility functions
│   │   ├── auth.ts            # Authentication utilities
│   │   └── mockData.ts        # Sample anime data
│   └── types/                 # TypeScript type definitions
│       └── index.ts           # Global types
├── public/                    # Static assets
├── .env.local                 # Environment variables
└── package.json              # Dependencies and scripts
```

## 🎯 Key Features Explained

### Authentication System
- **JWT-based authentication** with secure password hashing
- **Modal-based UI** for seamless user experience
- **Password reset functionality** with email simulation
- **Form validation** with error handling

### Dynamic Routing
- **Genre pages**: `/genre/[slug]` - Filter anime by genre
- **Type pages**: `/type/[type]` - Filter by anime type
- **Anime details**: `/anime/[id]` - Individual anime pages
- **Search results**: `/search?q=query` - Search functionality

### Data Management
- **Mock anime database** with 8 sample anime
- **40+ anime genres** with proper categorization
- **Multiple anime types** (Movies, TV Series, OVAs, etc.)
- **Comprehensive anime metadata** (ratings, episodes, year, etc.)

### SEO & Performance
- **Server-side rendering** with Next.js App Router
- **Meta tags optimization** for each page
- **Open Graph support** for social media sharing
- **Responsive images** and lazy loading
- **Clean URLs** and proper sitemap structure

## 🔧 API Endpoints

### Authentication
- `POST /api/auth/login` - User login
- `POST /api/auth/register` - User registration
- `POST /api/auth/reset-password` - Password reset

### Anime Data
- `GET /api/anime/list` - Get anime list with filters
- Query parameters: `genre`, `type`, `search`, `limit`, `offset`

## 🎨 Customization

### Styling
- Modify `src/app/globals.css` for global styles
- Update Tailwind configuration in `tailwind.config.js`
- Customize components in `src/components/`

### Data
- Add more anime in `src/lib/mockData.ts`
- Extend genres and types as needed
- Integrate with real anime APIs

### Features
- Add user profiles and watchlists
- Implement video streaming
- Add comment systems
- Integrate payment systems

## 🚀 Deployment

### Vercel (Recommended)
1. Push your code to GitHub
2. Connect your repository to Vercel
3. Set environment variables in Vercel dashboard
4. Deploy automatically

### Other Platforms
- **Netlify**: Configure build settings for Next.js
- **Railway**: Use the Next.js template
- **DigitalOcean**: Deploy with App Platform

## 📝 Environment Variables

```env
# Authentication
JWT_SECRET=your-jwt-secret-key
NEXTAUTH_SECRET=your-nextauth-secret
NEXTAUTH_URL=your-domain-url

# Database (if using real database)
DATABASE_URL=your-database-connection-string

# External APIs (if integrating)
ANIME_API_KEY=your-anime-api-key
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Original Design**: Inspired by 9animetv.to
- **Next.js Team**: For the amazing framework
- **Tailwind CSS**: For the utility-first CSS framework
- **Anime Community**: For the inspiration and content

## 📞 Support

If you have any questions or need help with the project:

1. Check the [Issues](../../issues) page
2. Create a new issue if needed
3. Join our community discussions

---

**Note**: This is a demonstration project. For production use, ensure you have proper licensing for anime content and comply with copyright laws.
