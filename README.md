# Hunter

Hunter is a free tool finder that runs in your browser. Find online games, AI tools, photo and video editors, and PDF helpers, then open them with one tap. You don't need to download or install anything.

The whole app is one HTML file. It has no frameworks, no build step and no server, so it works on any phone or computer.

## Features

- **Search** tools by name, description, category or website
- **Category filters** for Online Games, Social Media, AI Tools, Photo Tools, Video Tools and Other Tools
- **Hunt a random tool** to discover something new
- **Save favorites** with the ☆ button and view only saved tools
- **Copy link** button on every tool card
- **Add your own tools** with a name, link, category and short description
- **Dark and light theme**
- **Mobile friendly** and works offline once the file is on your device

## Included tools

| Category | Tools |
| --- | --- |
| Online Games | PlayBrain, Pogo, GameTop, PlayHop, OnlineGames.io, now.gg |
| Social Media | Facebook, Instagram, YouTube |
| AI Tools | There’s An AI For That, Google Flow, Hugging Face Spaces |
| Photo Tools | Remove.bg, Photoroom Tools, iLoveIMG Remove Background, ImgTools |
| Video Tools | Upscaler.video, ArtPlayer Upscaler, TensorPix |
| Other Tools | PDF24 Tools, Smallpdf, TinyURL, ShortURL |

## How to use

### Open it on Android

1. Download `hunter-app.html`.
2. Open it with a browser, or in Quick Edit's preview.

### Run it with ksweb

1. Put `hunter-app.html` in your ksweb `htdocs` folder and rename it to `index.html`.
2. Start the server in ksweb.
3. Open `http://localhost:8080` in your browser (use the port shown in ksweb).

### Run it with Termux

```bash
pkg install python
cd path/to/hunter
python -m http.server 8080
```

Then open `http://localhost:8080/hunter-app.html` in your browser.

### Put it online with GitHub Pages

1. Upload the file to a GitHub repository and rename it to `index.html`.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, then select `main` and `/ (root)`.
4. Save. Your site will appear at `https://YOUR-USERNAME.github.io/YOUR-REPO/` after a minute or two.

## Add more tools to the code

Open the file and find the `BASE` list in the script. Each tool is one line in this order: name, link, category, description.

```js
["Tool Name", "https://example.com/", "Photo Tools", "What this tool does."],
```

The category must match one of the names in the `CATS` list. To add a new category, add a name and a color to `CATS` as well.

Tools you add from inside the app are stored in your browser, so they stay on that device only. To share a tool with every visitor, add it to the `BASE` list instead.

## Project structure

```text
hunter/
├── index.html   (the app, or hunter-app.html before renaming)
└── README.md
```

## Built with

- HTML, CSS and plain JavaScript
- `localStorage` for saved and custom tools

## Notes

Hunter only links to third-party websites. It doesn't own or control them, and their features, prices and availability can change.

## Author

**Ebrat Hossen**

- Facebook: [facebook.com/ebrathossen](https://www.facebook.com/ebrathossen)
- Messenger: [m.me/ebrathossen](https://m.me/ebrathossen)
- Email: [ebrathossen720@gmail.com](mailto:ebrathossen720@gmail.com)

## Contributing

Ideas and new tool suggestions are welcome. Open an issue or send a pull request with the tool name, link, category and a one-line description.

## License

Add a license before sharing the project publicly. If you want others to use and change it freely, choose the [MIT License](https://choosealicense.com/licenses/mit/) when you create the file on GitHub.
