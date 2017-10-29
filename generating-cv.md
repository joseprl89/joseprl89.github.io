# JSONResume

I use a tool found at jsonresume.org to apply a style to a CV written in json format.

# HTML CV

## Style used

The style used is found here:

https://github.com/mudassir0909/jsonresume-theme-elegant

Had to write a PR to handle properly end dates not yet present in the JSON (i.e. still working in the company).

## How it works

Download the theme repo, place the resume json file in the root of it, and run

`resume export --theme flat resume.html`

This generates an html version of the resume.

# PDF CV

## Style used

elegantprofile, as per its root repo

## How to obtain a PDF

First time I used the tool, the PDF extracter didn't work properly, so I had to tinker with the HTML using the chrome 
dev tools, then take a snapshot of it using fireshot.
