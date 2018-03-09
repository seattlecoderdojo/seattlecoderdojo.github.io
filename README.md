## Hackers - the hacker room website

### Contributing
1. Clone this repository
2. Install ruby (if you somehow don't have it)
3. Set up Jekyll:
```bash
gem install jekyll bundler
```
4. Run `jekyll serve` for a development server!

### To add a Tutorial
1. Create a new markdown file in `_tutorials`
2. At the head of the file, be sure to populate the following information:
```yaml
---
title: Your fancy title here
difficulty: intermediate
language: javascript
estimate: '1 hour'
---
```
... be sure to only pick 1 difficulty and language. The site indexes by these
two tags. Estimate is optional, but why not.
