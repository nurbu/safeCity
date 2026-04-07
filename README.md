# SafeCity

> Navigate smarter. Stay safer.

SafeCity is a web application built at the **Kean University Hackathon** that helps users find safer walking or travel routes by analyzing real crime data. Instead of finding the *shortest* path, SafeCity finds the *safest* one — routing you away from areas with higher reported crime activity.

---

## Features

- **Safe Route Generation** — Calculates routes that avoid high-crime areas based on real crime data points
- **Interactive Map** — Visualizes crime hotspots and your suggested safe path
- **Crime Data Integration** — Uses crime incident data to score and weight route options
- **Real-time Navigation** — Fast, responsive UI built with Next.js

---

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Framework | [Next.js](https://nextjs.org/) (App Router) |
| Language | TypeScript |
| Styling | CSS / PostCSS |
| Linting | ESLint |

---

## Getting Started

### Prerequisites

- Node.js `v18+`
- npm, yarn, pnpm, or bun

### Installation

```bash
git clone https://github.com/nurbu/safeCity.git
cd safeCity
npm install
```

### Running the Development Server

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser to see the app.

---

## Project Structure

```
safeCity/
├── public/           # Static assets
├── src/
│   └── app/          # Next.js App Router pages & components
├── next.config.ts    # Next.js configuration
├── tsconfig.json     # TypeScript configuration
└── package.json      # Dependencies & scripts
```

---

## How It Works

1. User inputs a start and destination point on the map.
2. Crime data points are loaded and mapped geographically.
3. The routing algorithm penalizes paths that pass near crime hotspots.
4. The app returns the optimal safe route — balancing distance with safety score.

---

## Built At

**Kean University Hackathon**
A time-limited hackathon challenge focused on building practical solutions for community safety.

---

## Contributing

Pull requests are welcome. If you'd like to improve the routing algorithm, add new data sources, or enhance the UI, feel free to fork the repo and open a PR.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/my-feature`)
3. Commit your changes (`git commit -m 'Add my feature'`)
4. Push to the branch (`git push origin feature/my-feature`)
5. Open a Pull Request

---

## License

This project is open source. See the repository for details.

---

## Acknowledgements

- Crime data sourced from public datasets
- Built with [Next.js](https://nextjs.org/) by Vercel
- Inspired by the goal of making cities safer for everyone
