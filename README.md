# Spotify 2.0 Clone - Modern Music Streaming App

A complete, responsive, and dynamic music streaming web application built with Next.js that replicates and enhances the essential functionalities of Spotify.

## 🚀 Features

### Core Functionality
- **Homepage**: Featured playlists, new releases, and trending albums
- **Search**: Real-time search with suggestions and categorized results
- **Playlists**: Full playlist management with cover art and metadata
- **Music Player**: Persistent bottom player with full controls
- **Genre Exploration**: Browse music by genre with curated playlists
- **Library**: Personal music library with liked songs and playlists

### Player Features
- Play/Pause, Previous/Next, Shuffle, Repeat controls
- Progress bar with scrubbing capability
- Volume control with mute toggle
- Persistent playback across route changes
- Queue management and autoplay

### UI/UX
- Spotify-inspired dark theme design
- Fully responsive layout (mobile, tablet, desktop)
- Smooth animations and hover effects
- Loading states and error handling
- Accessible keyboard navigation

## 🛠 Tech Stack

- **Frontend**: Next.js 14 with App Router
- **Styling**: Tailwind CSS with custom components
- **State Management**: Zustand for global music state
- **UI Components**: shadcn/ui component library
- **Icons**: Lucide React
- **Audio**: HTML5 Audio API
- **TypeScript**: Full type safety

## 📁 Project Structure

\`\`\`
spotify-clone/
├── app/                    # Next.js App Router pages
│   ├── page.tsx           # Homepage
│   ├── search/            # Search functionality
│   ├── playlist/[id]/     # Dynamic playlist pages
│   ├── genre/[id]/        # Genre-specific pages
│   ├── library/           # User library
│   └── liked/             # Liked songs
├── components/            # Reusable UI components
│   ├── sidebar.tsx        # Navigation sidebar
│   ├── music-player.tsx   # Bottom music player
│   ├── track-card.tsx     # Individual track component
│   └── playlist-card.tsx  # Playlist display component
├── lib/                   # Utilities and state management
│   ├── music-store.tsx    # Zustand store for music state
│   ├── api.ts            # Mock API functions
│   └── utils.ts          # Utility functions
└── hooks/                 # Custom React hooks
    └── use-debounce.ts    # Debounced search hook
\`\`\`

## 🎵 Key Components

### Music Player
- Persistent bottom player that works across all pages
- Full playback controls with visual feedback
- Progress tracking and seeking
- Volume control and mute functionality
- Queue management with shuffle and repeat

### State Management
- Zustand store for global music state
- Track current song, playback status, and queue
- Persistent state across route changes
- Reactive updates to UI components

### Search System
- Debounced search input for performance
- Real-time results filtering
- Search across songs, artists, albums, and playlists
- Browse by genre functionality

## 🚀 Getting Started

1. **Clone the repository**
   \`\`\`bash
   git clone <repository-url>
   cd spotify-clone
   \`\`\`

2. **Install dependencies**
   \`\`\`bash
   npm install
   \`\`\`

3. **Run the development server**
   \`\`\`bash
   npm run dev
   \`\`\`

4. **Open your browser**
   Navigate to `http://localhost:3000`

## 🎨 Customization

### Adding Real Music API
Replace the mock data in `lib/api.ts` with real API calls:
- Deezer API
- Spotify Web API
- JioSaavn API
- Last.fm API

### Theming
Customize colors and styling in:
- `app/globals.css` for global styles
- `tailwind.config.js` for theme configuration
- Individual components for specific styling

### Adding Features
- User authentication with Firebase/Auth0
- Playlist creation and management
- Social features (following, sharing)
- Offline playback support
- Advanced audio features (equalizer, crossfade)

## 📱 Responsive Design

The application is fully responsive with breakpoints for:
- Mobile: 320px - 768px
- Tablet: 768px - 1024px
- Desktop: 1024px+

## ♿ Accessibility

- Semantic HTML structure
- ARIA labels and roles
- Keyboard navigation support
- Screen reader compatibility
- High contrast support

## 🔧 Performance Optimizations

- Next.js App Router for optimal loading
- Image optimization with Next.js Image component
- Lazy loading for better performance
- Debounced search to reduce API calls
- Efficient state management with Zustand

## 🚀 Deployment

The app is ready for deployment on:
- **Vercel** (recommended for Next.js)
- **Netlify**
- **AWS Amplify**
- **Docker containers**

### Environment Setup

The application currently uses mock data and doesn't require any API keys for basic functionality. When integrating with real music APIs in the future, you'll need to:

1. Create a `.env.local` file in the root directory
2. Add your API credentials (refer to the specific API documentation)
3. Update the API functions in `lib/api.ts` to use real endpoints

For development, the app works out of the box with the included mock data and sample audio tracks.

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests if applicable
5. Submit a pull request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- Spotify for design inspiration
- shadcn/ui for beautiful components
- Next.js team for the amazing framework
- Vercel for hosting and deployment tools

---

Built with ❤️ using Next.js and modern web technologies.
