# DeepGrounding Website

Static landing page for DeepGrounding, an independent research organization
focused on recursive self-improvement, long-horizon AI systems, and grounded
evaluation.

## Local Preview

Open `index.html` in a browser, or serve the directory locally:

```bash
python3 -m http.server 8000
```

Then visit <http://localhost:8000>.

## GitHub Pages Deployment

This directory is intended to be the root of the public repository:

```text
deepgrounding/deepgrounding.github.io
```

Required repository files:

- `index.html`
- `styles.css`
- `CNAME`
- `README.md`

In GitHub repository settings:

1. Go to **Settings -> Pages**.
2. Set **Build and deployment** to **Deploy from a branch**.
3. Select the default branch and the root folder.
4. Set the custom domain to `deepgrounding.org`.
5. Enable **Enforce HTTPS** after DNS verification completes.

## DNS Records

Configure these records in Alibaba Cloud DNS for `deepgrounding.org`:

```text
@    A      185.199.108.153
@    A      185.199.109.153
@    A      185.199.110.153
@    A      185.199.111.153
www  CNAME  deepgrounding.github.io
```

After DNS propagates, GitHub Pages should serve:

- `https://deepgrounding.org`
- `https://www.deepgrounding.org`

## Future Content

Research project pages can be added once materials are cleared for public
release. Suggested future routes:

- `/research/recursive-self-improvement/`
- `/research/calibration-floor/`
- `/notes/`
