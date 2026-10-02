# local-bouncing-DVD-logo
A locally runnable version of [bouncingdvdlogo.com](https://bouncingdvdlogo.com) with some tweaks.

- All of the logic and styling is in `bouncingdvd.html`.
- You can add or remove items in "logos" and the page will dynamically adjust to the new items after a reload (just make sure you keep the same naming scheme).
- On each page reload, the starting size and vector will be different, within a range depending on viewport size.

---

### Setup

Just make sure you have the `logos/` folder in the same directory as `bouncingdvd.html`. It should look like this:
```
.
├── bouncingdvd.html
└── logos
    ├── dvdlogo-01.svg
    ├── dvdlogo-02.svg
    ├── dvdlogo-03.svg
    └── dvdlogo-...
```

Display it either by:
- Opening `bouncingdvd.html` in your browser directly (making sure to keep the file hierarchy above) and it will display animated, or...
- Run a web server in the same directory as `bouncingdvd.html` and access it via the HTTP server's address (e.g.. if python3 is installed on your system, run `python -m http.server 8080`, and open `localhost:8080/bouncingdvd.html`; if you want it to open directly at `localhost:8080`, feel free to rename `bouncingdvd.html` to `index.html`).
