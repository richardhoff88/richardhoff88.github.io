
### Customization and Code Structure
- `_config.yml`: this is the configuration file. You have to restart the local server to reflect changes when developping locally. 
- `_data/navigation.yml`: where you customize the navigation bar. 
- `_pages/`: where I put my actual content pages, in HTML and Markdown format.
- `index.md`: this is the main landing page. 
- `assets/css/styles.css`: where I put my custom CSS.
- `docs`, `images`, `pdfs`: my data directories. 
- `_includes/footer.html`: modify the website footer info.
- `_site`: the auto-generated html files (from the md files in `_pages`)

### Local dev
```bash
bundle exec jekyll serve --livereload
JEKYLL_ENV=production bundle exec jekyll serve --livereload  # force production env to test the disqus comment functions
```

### Resources Links
Here are some resources/documentation that I've found useful when building the website:
- getting started with Jekyll: [Jekyll](https://jekyllrb.com/)
- configuring [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/docs/configuration/)
- Minimal Mistakes's [Github repo page](https://github.com/mmistakes/minimal-mistakes)
