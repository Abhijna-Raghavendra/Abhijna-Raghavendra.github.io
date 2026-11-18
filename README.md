# abhijna-raghavendra.github.io

Personal academic website of Abhijna Raghavendra: research in post-quantum cryptography, proof systems and coding theory.

Live at **https://abhijna-raghavendra.github.io/**

Built with [Astro](https://astro.build) and deployed to GitHub Pages by the workflow in `.github/workflows/deploy.yml` on every push to `main`.

## Structure

```text
/
├── public/
│   ├── papers/               # Thesis, course report, slides, notes (PDF)
│   ├── cv.pdf
│   └── abhijna-raghavendra.jpeg
├── src/
│   ├── components/           # Theme toggle
│   ├── layouts/              # Base page layout, projects page layout
│   └── pages/
│       ├── index.astro       # Main page: publications, research, projects, background
│       ├── projects.md       # Software projects page
│       └── projects/*.md     # One file per software project
└── package.json
```

Content for the main page lives at the top of `src/pages/index.astro`: the `research` and `projects` arrays hold the cards.

A link to a local PDF only appears if the file exists in `public/`. The build prints a warning for any linked file it cannot find.

## Commands

| Command           | Action                                          |
| :---------------- | :---------------------------------------------- |
| `npm install`     | Install dependencies                            |
| `npm run dev`     | Start the dev server at `localhost:4321`        |
| `npm run build`   | Type-check, then build the site into `./dist/`  |
| `npm run preview` | Preview the built site locally                  |

## Licence

Source code is MIT-licensed. Papers, notes, slides, photographs and written content are not; see [LICENSE](LICENSE).
