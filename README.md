# Personal site

## Workflow

Local serving workflow
```sh
    $ bundle exec jekyll serve --lsi --drafts
```

Create draft
```sh
    $ bundle exec jekyll draft "My new draft"
```

Create post
```sh
    $ bundle exec jekyll post "My New Post"
```

Publish/unpublish post
```sh
    $ bundle exec jekyll publish _drafts/my-new-draft.md
    $ bundle exec jekyll unpublish _posts/2014-01-24-my-new-draft.md
```

Create page
```sh
    $ bundle exec jekyll compose "My new Page" --collection "pages"
```

## Features
- [x] Post page, date and category styles
- [x] Update nav footer content
- [x] Social icon support on external aux links, include icons as `_includes`.

- [ ] Post list page and RSS streams
- [ ] Post page, ChatGPT integration
- [ ] Archive page layout and style update, no need for `<table>`
- [ ] Jupyter notebook styles

Integration
- [x] Disqus comment
- [x] Google Analytics integration

- [ ] Spotify listening list
- [ ] Good reads integration list
      - Static export as JSON

Writing
- [ ] Home page, introduction