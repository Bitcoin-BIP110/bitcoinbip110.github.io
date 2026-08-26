# Bitcoin BIP110 static site

This directory contains the rendered HTML, CSS, JavaScript, images, and data files for the Bitcoin BIP110 site. It is portable to a GitHub Pages project site, including URLs such as `https://USERNAME.github.io/REPOSITORY/`.

## Publish with GitHub Pages

1. Create a new GitHub repository.
2. Upload everything in this directory to the repository root, including `.nojekyll`.
3. Open **Settings > Pages** in the repository.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Select the `main` branch and the `/ (root)` folder, then save.

GitHub will display the Pages URL after deployment finishes.

## Local preview

Run a static file server from this directory. For example:

```sh
python3 -m http.server 8000
```

Then open `http://localhost:8000/`.

Opening `index.html` directly with a `file://` URL is not recommended because browsers may block module assets.
