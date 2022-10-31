# TO-DO

## Required before site can go live
- [X] Figure out youtube shortcode
- [X] Create archtypes
  - [X] For "link" posts
  - [X] For "video" posts
  - [X] For regular posts
- [X] Add in post footer
- [X] Get figure shortcode working
- [ ] Copy other single pages from Jekyll version of site
  - [X] CIDR
  - [X] keybase.txt
  - [X] robots.txt
  - [X] Copy htaccess file
    - [X] Redirect not required - using permalink configuration setting to match old URLs
- [X] Setup 404 error page
- [X] Complete scripts partial with
  - [X] Mint
  - [X] Matomo
- [X] Setup RSS feed

## Go Live Steps
- [X] Final conversion of Jekyll posts
- [X] Remove test posts from content/posts, content/videos, content/links
- [X] Put htaccess redirect into place
- [X] Delete and recreate public_html/blog directory on web host (rsync --delete?)
- [X] rsync -azr --delete public/* public_html/blog


## Optional - can happen after going live
- [ ] Create GitHub Action that rsyncs public to Pair on commit to main branch
- [ ] Get Tags page setup and working
- [ ] Get a dark mode working
- [ ] Get cat JavaScript working

## Ancillary - need to do elsewhere as a result of this project
- [X] Create new subdomain for password page

