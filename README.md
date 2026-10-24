# The Corner Florist

Make a custom bouquet and send it to someone you love.

## Put it online (pick one)

**GitHub Pages**: create a public repo named `corner-florist`, upload everything in this folder, then Settings > Pages > Deploy from branch `main` / root. It goes live at `https://<you>.github.io/corner-florist/`.

**Netlify Drop**: drag this folder onto https://app.netlify.com/drop.

If the address isn't `https://rupam870.github.io/corner-florist/`, replace that address in the `og:` / `twitter:` / `canonical` tags at the top of `index.html` so link previews show the picture.

## Count visits (Mixpanel)

1. Create a free project at mixpanel.com and copy its Project Token.
2. In `index.html`, set `const MIXPANEL_TOKEN = 'your-token';`
3. Redeploy. Tracking stays off on localhost.

Events: Page Viewed (role: sender / recipient), Occasion Started, First Stem Picked, Wrap Started, Wrap Completed, Note Chosen, Gift Link Created, Gift Shared (method: share / copy), Preview Opened, Gift Opened, Flowers Taken, Ribbon Untied, Flower Fact Viewed, Image Saved, Make One Back Clicked. Each gift link carries a `gift_id`, so you can see how many sent gifts got opened.

## Credit

`const MAKER = {name:'Rupam', url:''}` near the top of the script. Add a URL to make the name a link.
