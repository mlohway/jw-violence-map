# Violence and persecution against Jehovah’s Witnesses, 1935–1950

Milo Hathaway · History 4245: Nazi Germany and the Holocaust

Interactive map of 188 incidents compiled from:
- "Mass violence against Jehovah's Witnesses, 1940–1942" (Cambridge, 2015)
- ACLU, *The Persecution of Jehovah's Witnesses* (1941)
- Shawn Francis Peters, *Judging Jehovah's Witnesses* (2000)
- Rebekah Huss Fox, "Johnson v. State," in *First Amendment Studies in Arkansas* (2016)

## Files
- `index.html`: the map (D3 + TopoJSON, loaded from public CDNs)
- `data.json`: the incidents
- `states.json`: US state outlines (us-atlas, ISC license)

## Publish on GitHub Pages
1. Create a new public repository and upload these three files to its root.
2. Settings → Pages → Source: "Deploy from a branch", branch `main`, folder `/ (root)`.
3. After a minute the map is live at `https://<username>.github.io/<repo>/`.

The page loads its data with `fetch()`, so it must be served over http(s). Opening `index.html`
directly from your disk will show "The map data couldn't load."

## Embed elsewhere
```html
<iframe src="https://<username>.github.io/<repo>/" width="100%" height="700" style="border:0"></iframe>
```

## Updating
Replace `data.json` with a new export. Columns match the spreadsheet; the fields starting with `_`
are the filter categories.
