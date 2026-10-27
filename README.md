# Personal site — strict-orig version, deployed at the root domain

- HTML: strict transform from REA DOM structure, personal text blanked for the owner to fill in later.
- CSS: 17 original CSS files, in css/.
- JS: original module scripts + imported chunks, in assets/; the same files are
  also in _astro/ because the original clock worker is loaded from the absolute
  /_astro/ path, which resolves at a root domain.
- .nojekyll is required so GitHub Pages serves the underscore-prefixed _astro/ directory.
- Fonts: NOT copied into this repo (the GitHub connector cannot push binary files);
  CSS loads them from the original site's /fonts/ path, so the look is preserved.
- NOT included: inline boot scripts, structured data, and JSON data payloads
  (cup / easel sections / logo / mood feed) — those carry the author's own
  content, to be replaced by the owner with his own data/interfaces.
- Known limits until the owner supplies data/backend: backend API calls (/api/...)
  return 404; easel/painting, project dialog, blog subscribe and mood feed need
  the owner's data payloads and backend before they work fully. Theme and
  command palette work with the original JS.
