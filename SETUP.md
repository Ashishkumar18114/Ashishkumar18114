# Ashish Kumar — GitHub profile refresh

This package contains a replacement GitHub profile README, two self-contained animated SVG banners, and a daily contribution-snake workflow.

## 1. Update the profile repository

Open **[Ashishkumar18114/Ashishkumar18114](https://github.com/Ashishkumar18114/Ashishkumar18114)**. Back up the existing `README.md` if you want to keep it.

Commit these three files from the `github-profile-refresh/` folder to the **root** of that repository on `main`:

- `README.md` — replaces the existing profile README
- `dark.svg` — dark-mode banner
- `light.svg` — light-mode banner

GitHub will automatically display the README on [your profile](https://github.com/Ashishkumar18114). The hero uses `<picture>` to display exactly one SVG based on the visitor's color-scheme preference.

## 2. Set up the contribution snake

1. Create a **public** repository named **`github-snake`** under `Ashishkumar18114` (the repository does not yet have to contain a README).
2. Add this package's `github-snake/.github/workflows/snake.yml` to **exactly** `.github/workflows/snake.yml` in the new repository's `main` branch.
3. Under **Settings → Actions → General**, ensure Actions are enabled and **Workflow permissions** allow read/write access where your repository policy requires it.
4. Open **Actions → Generate Contribution Snake → Run workflow** and wait for the action to finish successfully.
5. Confirm that the `output` branch contains `github-snake.svg` and `github-snake-dark.svg`.
6. Reload your profile. The README will now display the animated snake with automatic light/dark switching. The workflow runs daily at **00:15 UTC** and can be triggered manually.

If you publish the profile README before step 4 succeeds, the snake section may show a missing image temporarily.

## Notes

- Both hero SVGs contain the portrait as actual SVG characters derived from your public GitHub avatar, with **no external image, font, JavaScript, or CSS dependencies**.
- The SVG animation is native SVG/SMIL; GitHub and browsers may reduce or suppress animation depending on their SVG renderer or motion settings.
- All personal text, roles, technologies, projects, certifications, and contact links were taken from the public GitHub profile you supplied; no performance metrics were invented.
- The generated files are **not yet published to GitHub**. They need to be committed to your repositories, or you can connect GitHub in ChatGPT for repository updates.
