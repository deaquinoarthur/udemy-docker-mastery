# Docker Mastery

## Assignment: Bind Mounts

- Use a Jekyll "Static Site Generator" to start a local web server
- Don't have to be a web developer: this is an example of bridging the gap
  between local file access and apps running in containers
- source code is in the course repo under `bindmount-sample-1`
- We edit files with editor on our host using native tools
- Container detects changes with host files and updates web server
- start container with `docker run -p 80:4000 -v $(pwd):/site bretfisher/jekyll-serve`
- Refresh our browser to see changes
- Change the file in `_posts/` and refresh the browser to see changes
