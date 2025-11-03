# CSE 134B : Discussion 6

For Astro to run on your system, you will also need to have a compatible version of Node.js installed. 
For whatever reason Astro only supports even-numbered Node.js versions, so verify this with node -v.

https://docs.astro.build/en/tutorial/1-setup/2/ gives a very straightforward intro to creating and running your site.

See below for a list of relevant Astro commands and their effects:
| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |


## Folder structure of src

```
Project root
├─ src/                    
│  ├─ layouts/             # allows you to set up templates that can be recycled across pages
│  │  └─ MarkdownPostLayout.astro  # sample layout
│  ├─ pages/               # Top-level routes/pages
│  │  ├─ index.astro      
│  │  └─ blogs.astro       
│  ├─ components/          # For any reusable components (smaller than layouts)
│  │  └─ Navigation.astro
│  ├─ posts/               # Markdown blog posts/content. One quirk with Astro is that markdown files, as shown in pages/posts, can automatically be rendered in readable HTML, though for full credit they should be enhanced with a layout.
│  │  ├─ post-1.md
│  │  ├─ post-2.md
│  │  └─ post-3.md
│  └─ styles/              # Global and/or component styles
│     └─ global.css
```
For full credit, you are expected to go a bit beyond what has already been presented in the discussion.