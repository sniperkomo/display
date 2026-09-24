# NFL Spread Model Display

A small, dependency-free NFL dashboard that displays one detailed card for every game in the weekly slate.

## What it shows

- Day grouping and kickoff time
- Stadium and stadium location
- Away and home team rows
- Sportsbook market line
- Model projected line
- One highlighted model pick per game
- No score projections or team filter

The current data was transcribed from the supplied model screenshot. The site is a display layer only; it does not contain or recreate the underlying prediction algorithm. The model pick favors the home spread when the model is more favorable to the home team; otherwise it selects the away spread with the sign flipped. Score projections are intentionally omitted.

## Publish with GitHub Pages

1. Open the repository's Settings.
2. Open Pages.
3. Set the source to GitHub Actions.
4. Pushes to the main branch will run .github/workflows/deploy-pages.yml.
5. GitHub will show the published site URL in the workflow run and Pages settings.

Because this repository is private, whether the published site can be publicly viewed depends on the GitHub account or organization plan and Pages settings.

## Updating the weekly slate

Edit the games array near the bottom of index.html. Each item contains kickoff, game, line, model, lineValue, and modelValue fields.

Then commit the change to main. The Pages workflow will redeploy the site.

This is for informational purposes only. Model projections are not guarantees of results.