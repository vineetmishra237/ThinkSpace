# ThinkSpace

ThinkSpace is a collaborative canvas application for visual thinking, planning, and real-time collaboration. It allows users to sketch ideas, map flows, drop notes, and build together in one shared space.

## Features

- **Real-time Collaboration**: Work together with team members in real-time on shared canvases
- **Rich Text Editor**: Built with EditorJS, supporting headers, lists, checklists, and warnings
- **Interactive Canvas**: Powered by Excalidraw for freeform drawing and diagramming
- **Team Management**: Create and manage teams for collaborative workspaces
- **File Organization**: Organize your documents and canvases efficiently
- **Authentication**: Secure user authentication powered by Kinde Auth
- **Dark Mode Support**: Built-in dark mode for comfortable viewing
- **Responsive Design**: Works seamlessly across desktop and mobile devices

## Tech Stack

- **Frontend**:
  - [Next.js 14](https://nextjs.org/) - React framework
  - [TypeScript](https://www.typescriptlang.org/) - Type safety
  - [Tailwind CSS](https://tailwindcss.com/) - Styling
  - [shadcn/ui](https://ui.shadcn.com/) - UI components
  - [Excalidraw](https://excalidraw.com/) - Canvas drawing
  - [EditorJS](https://editorjs.io/) - Rich text editing

- **Backend & Database**:
  - [Convex](https://www.convex.dev/) - Backend and real-time database

- **Authentication**:
  - [Kinde](https://kinde.com/) - User authentication

## Getting Started

### Prerequisites

- Node.js (v18 or higher)
- npm or yarn
- A Convex account
- A Kinde account

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/vineetmishra237/ThinkSpace.git
   cd ThinkSpace
   ```

2. Install dependencies:
   ```bash
   npm install
   # or
   yarn install
   ```

3. Set up environment variables:
   Create a `.env.local` file in the root directory with the following variables:
   ```
   NEXT_PUBLIC_CONVEX_URL=your_convex_deployment_url
   NEXT_PUBLIC_KINDE_CLIENT_ID=your_kinde_client_id
   NEXT_PUBLIC_KINDE_DOMAIN=your_kinde_domain
   NEXT_PUBLIC_GOOGLE_ADS_CLIENT_ID=your_google_ads_client_id
   ```

4. Start the development server:
   ```bash
   npm run dev
   # or
   yarn dev
   ```

5. Open [http://localhost:3000](http://localhost:3000) in your browser.

### Project Structure

```
app/
├── (routes)/                # Application routes
│   ├── dashboard/          # Dashboard components and layout
│   ├── teams/             # Team management
│   └── workspace/         # Canvas and editor workspace
├── _components/           # Shared components
├── _constant/            # Application constants
├── _context/            # React context providers
└── api/                 # API routes

components/              # UI components
├── ui/                 # Reusable UI components

convex/                 # Convex backend
├── _generated/        # Generated Convex types
├── files.tsx         # File management
├── teams.tsx        # Team management
└── user.tsx        # User management
```

## Features in Detail

### Document Editor
- Rich text editing with support for:
  - Headers
  - Lists (ordered and unordered)
  - Checklists
  - Warning blocks
  - Paragraphs

### Canvas
- Free-form drawing
- Shape tools
- Text annotations
- Real-time collaboration
- Export capabilities

### Team Management
- Create and join teams
- Manage team members
- Shared workspaces
- File permissions

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [Excalidraw](https://excalidraw.com/) for the amazing drawing library
- [EditorJS](https://editorjs.io/) for the rich text editing capabilities
- [shadcn/ui](https://ui.shadcn.com/) for the beautiful UI components
