name: Deploy website
on:
  workflow_dispatch:
  push:
    branches:
      - main


jobs:
  deploy:
    runs-on: ubuntu-latest
    permissions:
      contents: write  # To push a branch 
      pages: write  # To push to a GitHub Pages site
      id-token: write # To update the deployment status
    steps:
      - uses: actions/checkout@v4
        with:
          fetch-depth: 0
      - uses: dtolnay/rust-toolchain@stable
      - uses: Swatinem/rust-cache@v2
      - name: Install latest mdbook
        run: |
          cargo install mdbook
      - name: Install preprocessors
        run: |
          cargo install --locked mdbook-callouts
          cargo install --locked mdbook-emojicodes
      - name: Build Book
        run: |
          # This assumes your book is in the root of your repository.
          # Just add a `cd` here if you need to change to another directory.
          mdbook build
      - name: Setup Pages
        uses: actions/configure-pages@v5
      - name: Upload artifact
        uses: actions/upload-pages-artifact@v3
        with:
          # Upload entire repository
          path: 'book'
      - name: Deploy to GitHub Pages
        id: deployment
        uses: actions/deploy-pages@v4

