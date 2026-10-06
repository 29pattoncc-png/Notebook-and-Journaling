# Online Journal Tool

A simple browser-based journal app for writing thoughts, actions, and notes.

## Features

- Save journal entries locally in browser storage
- Add title, tags, and body text
- Search entries by text or tag
- Edit and delete past entries
- Export entries as JSON

## Usage

1. Open `index.html` in a browser, or start a local web server from this folder:

   ```powershell
   py -m http.server 8000
   ```

   Then open <http://localhost:8000>.
2. Write a title, tags, and your journal content.
3. Click `Save Entry` to store it locally.
4. Use the search box to filter entries.
5. Click `Export JSON` to download your journal history.

## Publish with GitHub Pages

The included GitHub Actions workflow deploys the site when changes are pushed to
the `main` branch, or when the workflow is run manually.

1. Push this repository to GitHub.
2. In the repository, open **Settings → Pages** and select **GitHub Actions** as
   the build and deployment source if it is not already selected.
3. Open the **Actions** tab and wait for **Deploy to GitHub Pages** to complete.
   The workflow summary and the `github-pages` environment show the published
   site URL.

If the repository uses a default branch other than `main`, update the branch
under `push.branches` in `.github/workflows/deploy-pages.yml`.

## Notes

- Entries are stored in your browser's local storage.
- Each browser stores its own entries; publishing the site does not sync entries
  between browsers or devices.
