# schelling-games

## Playing Schelling games with UChicago students!

This project imports data from a Google Form where participants play "Schelling games" designed to demonstrate the ability to coordinate in the absence of communication in order to "win" cooperative (vs zero-sum) games.

Importantly, this is by no means intended to present reliable, rigorous data or to make any contribution to any literature whatsoever. Instead, this is intended to be an interactive exercise for two contexts:

1. Introducing students to concepts around non-verbal communication, cooperative interaction, tacit coordination, etc.
2. Offering an example repository to students getting started with R and/or GitHub.

For anyone falling into the second category who is using this repo as a reference, you should also note that R Markdown in this repo outputs to html and it build into GitHub pages. There are some important differences between a pages repo (like this) and a repo designed to organize a publishable manuscript (like with papaja). For example, a pages repo includes most YAML info in a dedicated `_site.yml` file, while a manuscript outputting to PDF or .docx will usually include a YAML header at the top of the R Notebook. Still, there is considerable overlap between the two. Poke around a little and you should be able to figure out what's what.

Finally, because this repo is intended to be a learning tool, the .Rmd and .R files contained within include many comments in both the markdown and code. Some comments are very over-explain-y and others are questions or challenges to prompt you to think about why some things are the way they are and what better alternatives might be. In other words, *don't* use these files as an example of how (or how much) to use informative comments effectively in your own work, but *do* take the time to read them properly and not just skim past them.

## Repo contents


```
-- [top level]
    -- _site.yml (define site-wide YAML parameters)    
    -- .gitignore
    -- README.md
    -- custom.css (define select style elements to override bootstrap)
    //top-level .Rmd files build to .html files in the docs folder//
    -- index.Rmd
    -- about.Rmd
    -- ma.Rmd (variant of index; uses data filtered to current MA students only)
-- data
    -- responses_raw.csv (static dataset snapshotted from google form data in Fall 2023)
-- source
    -- functions.R (required custom functions, sourced in index)
    -- setup.R (basic preparation of response data, defining aesthetic preferences, etc.) 
-- docs
    -- /site_libs
        -- //everything that builds a the html site on the backend, powered by bootstrap/bootswatch
    //html output and related files rendered from top-level docs//
    -- /index_files
    -- /ma_files
    -- /data
    -- /source
    -- index.html
    -- ma.html
```
