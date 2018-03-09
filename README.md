## Hackers - the hacker room website

### Contributing
If you want to run the develoment server locally:
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
languages: javascript ruby python
estimate: '1 hour'
---
```
You can pick 1 difficulty, but any number of languages (sepearted by spaces.)
Estimate is optional, but why not.
