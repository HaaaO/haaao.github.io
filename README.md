# Hi, I'm Zhonghao

I am a human-centered AI researcher and engineer, and this is my personal website.

## Local Development

### Prerequisites
- Ruby 2.6+ (comes pre-installed on macOS)
- Bundler gem

### Installation

1. Install dependencies:
   ```bash
   bundle install
   ```

2. If you encounter an error installing the `ffi` gem (common on newer macOS with Apple Silicon), the `Gemfile` already includes a fix. Just run:
   ```bash
   bundle update ffi
   ```

### Serving the Website Locally

Run the Jekyll development server:
```bash
bundle exec jekyll serve
```

The site will be available at `http://127.0.0.1:4000/`

Press `Ctrl+C` to stop the server.

---

This website is developed based on the design and open-sourced code from [Fred Hohman](https://github.com/fredhohman/fredhohman.github.io).
