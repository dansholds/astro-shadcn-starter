# Astro + Shadcn Starter

Welcome to the Astro + Shadcn Starter Template! This project is designed to help you get started quickly with [Astro](https://astro.build) and [Shadcn UI](https://ui.shadcn.com). It includes Tailwind CSS for styling and React for building interactive components.

![astroxshadcn](https://github.com/user-attachments/assets/99b0b2a1-3ef9-4f28-a347-91c665279c2d)

## Table of Contents

- [Features](#features)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Usage](#usage)
- [Important Notes About Astro & Shadcn](#important)

## Features

- 🚀 **Astro** - Modern static site generator.
- 🎨 **Shadcn UI** - Beautifully designed components built with Radix UI and Tailwind CSS.
- 📦 **Tailwind CSS** - Utility-first CSS framework.
- 🔥 **React** - Library for building user interfaces.

## Getting Started

Follow these instructions to set up the project locally.

### Prerequisites

Ensure you have the following installed:

- [Node.js](https://nodejs.org/en/download/)
- [npm](https://www.npmjs.com/get-npm)

### Installation

1. **Clone the repository**:

    ```sh
    git clone https://github.com/your-username/astro-shadcn-starter.git
    cd astro-shadcn-starter
    ```

2. **Install dependencies**:

    ```sh
    npm install
    ```

3. **Start the development server**:

    ```sh
    npm run dev
    ```

    Open [http://localhost:3000](http://localhost:3000) in your browser to see the result.

## Project Structure
```
├── public # Static assets
├── src
│ ├── components # React components
│ ├────ui # Shadcn installed components
│ ├── layouts # Layout components
│ ├── pages # Astro pages
│ ├── styles # Global styles
│ └── utils # Utility functions
├── astro.config.mjs # Astro configuration
├── tailwind.config.mjs # Tailwind CSS configuration
└── package.json # Project metadata and dependencies
```

## Usage

### Adding a New Page

To add a new page, create a new `.astro` file in the `src/pages` directory.

Example:

```astro
---
import Layout from '../layouts/Layout.astro';
---

<Layout title="New Page">
  <h1>New Page</h1>
  <p>This is a new page.</p>
</Layout>
```

## Important

Due to the static and island based nature of Astro, a lot of Shadcn components won't work out of the box, 
some components such as the Avatar require more work on your side to enable them to work (see `src/components/Avatar.tsx`).

You can find useful information on this from the following links:

- [Issues with Astro Islands when using Shadcn](https://github.com/shadcn-ui/ui/issues/2249)
- [Abstract components into react, ts components](https://github.com/shadcn-ui/ui/issues/2890)
