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

### References
Use [https://citation.crosscite.org/], apa formatting, to generate the reference from doi, and use Zenodo DOI badge generator:

```[![DOI:{DOI}](https://zenodo.org/badge/DOI/{DOI}.svg)](https://doi.org/{DOI})```

e.g.

```[![DOI:10.48550/ARXIV.2208.06102](https://zenodo.org/badge/DOI/10.48550/ARXIV.2208.06102.svg)](https://doi.org/10.48550/ARXIV.2208.06102)```
