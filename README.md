
This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`]

# Thinkspace

Thinkspace is a collaborative workspace web application built with Next.js, React, and Convex. It allows users to create, edit, and manage collaborative whiteboards in real-time, with authentication powered by Kinde and data storage handled by Convex.

## Features

- User authentication (Kinde)
- Dashboard with file management
- Collaborative document editor
- Collaborative whiteboard/canvas
- Team file support (free and premium plans)
- Responsive UI with modern design

## Tech Stack

- [Next.js](https://nextjs.org/)
- [React](https://react.dev/)
- [Convex](https://convex.dev/) (backend/database)
- [Kinde](https://kinde.com/) (authentication)
- [Tailwind CSS](https://tailwindcss.com/) (styling)
- TypeScript

## Getting Started

### Prerequisites

- Node.js (v18+ recommended)
- npm or yarn

### Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/yourusername/thinkspace.git
   cd thinkspace
   ```

2. **Install dependencies:**

   ```bash
   npm install
   # or
   yarn install
   ```

3. **Set up environment variables:**

   Create a `.env.local` file in the root directory and add your configuration:

   ```
   # Example (replace with your actual values)
   NEXT_PUBLIC_KINDE_CLIENT_ID=your_kinde_client_id
   NEXT_PUBLIC_KINDE_DOMAIN=your_kinde_domain
   NEXT_PUBLIC_CONVEX_URL=your_convex_url
   ```

4. **Run the development server:**

   ```bash
   npm run dev
   # or
   yarn dev
   ```

   Open [http://localhost:3000](http://localhost:3000) in your browser.

## Usage

- **Dashboard:** Manage your files and access workspaces.
- **Workspace:** Edit documents and use the collaborative canvas.
- **Authentication:** Sign in/up using Kinde.

## Project Structure

```
app/
  (routes)/
    dashboard/
      _components/
        FileList.tsx
        WorkspaceHeader.tsx
        ...
    workspace/
      [fileId]/
        page.tsx
      _components/
        Editor.tsx
        Canvas.tsx
        ...
  _components/
    Header.tsx
    Hero.tsx
    ...
convex/
  _generated/
    api.ts
components/
  ui/
    dialog.tsx
    ...
```

## Customization

- **Styling:** Uses Tailwind CSS, customize in `tailwind.config.js`.
- **Authentication:** Configured via Kinde, update credentials in `.env.local`.
- **Database:** Uses Convex, see [Convex docs](https://docs.convex.dev/) for schema and queries.

## License

MIT

---

**Note:**

- The pricing feature has been removed from this codebase.
- For any issues or contributions, please open an issue or pull request.