# Perimenoposse

A field guide for the perimenopause years. Real food. Real support. Real life.

Single static HTML page, served via GitHub Pages at [perimenoposse.net](https://perimenoposse.net).

## What's here

- `index.html` — the entire site (HTML, CSS, and signup JS in one file)
- `CNAME` — tells GitHub Pages which custom domain to serve (added in the domain step)

## Email signups

The two signup forms on the page write subscriber emails to a Supabase table called `subscribers`. Row Level Security is configured so the public anon key can insert new rows but cannot read existing ones — so the email list is never exposed in the browser, even though the anon key is.

To see new signups: log in to Supabase → Table Editor → `subscribers`.

## Editing the site

It's one file. Open `index.html`, edit, commit, push — GitHub Pages redeploys within a minute or two.
