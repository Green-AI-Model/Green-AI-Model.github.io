# Green Artificial Inteligence Model

This is the Github repo for the [Green AI Model (https://green-ai-model.github.io/)](https://green-ai-model.github.io/)

## How to build
- Static Website with: [hugo](https://gohugo.io/)
- (git submodule) Hugo Theme: [hugo-book](https://github.com/alex-shpak/hugo-book)

```bash
git clone git@github.com:Green-AI-Model/Green-AI-Model.github.io.git --recursive
```
If you already cloned without the submodule. You can add them with this:

```bash
git submodule init && git submodule update
```

### Usefull Hugo commands
```bash
hugo server --minify # Start server (minimal html)
hugo mod clean #Cleans cache
```

## How to edit
- Files can be found here: [/content/docs](/content/docs)
- Theme settings: [hugo.toml](hugo.toml)
