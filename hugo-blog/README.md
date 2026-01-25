# Yongkang's Blog - Hugo with PaperMod Theme

This is Yongkang Yang's research blog, built with Hugo and the PaperMod theme.

![Hugo Blog Homepage](https://github.com/user-attachments/assets/9368c2a8-52f2-4b8c-8a76-2e2b0f68100e)

## Prerequisites

- Hugo Extended v0.146.0 or higher (required for PaperMod theme)

## Installation

### Install Hugo

On Linux:
```bash
wget https://github.com/gohugoio/hugo/releases/download/v0.146.0/hugo_extended_0.146.0_Linux-64bit.tar.gz
tar -xzf hugo_extended_0.146.0_Linux-64bit.tar.gz
sudo mv hugo /usr/local/bin/
```

On macOS with Homebrew:
```bash
brew install hugo
```

### Clone the Repository

```bash
git clone https://github.com/yongkang-yang/source_blog.git
cd source_blog/hugo-blog
git submodule update --init --recursive
```

## Running Locally

To run the Hugo server locally:

```bash
hugo server
```

The site will be available at http://localhost:1313

To build the static site:

```bash
hugo --minify
```

The built site will be in the `public/` directory.

## Running in GitHub Codespaces

### Quick Start

1. Open this repository in GitHub Codespaces
2. In the terminal, navigate to the hugo-blog directory:
   ```bash
   cd hugo-blog
   ```
3. Run the convenience script:
   ```bash
   ./start-server.sh
   ```
4. Codespaces will automatically forward port 1313 and prompt you to open the site in your browser

### Manual Setup (if Hugo not installed)

If Hugo is not already installed in your Codespace:

1. Install Hugo:
   ```bash
   wget https://github.com/gohugoio/hugo/releases/download/v0.146.0/hugo_extended_0.146.0_Linux-64bit.tar.gz
   tar -xzf hugo_extended_0.146.0_Linux-64bit.tar.gz
   sudo mv hugo /usr/local/bin/
   ```
2. Start the Hugo server:
   ```bash
   hugo server --bind 0.0.0.0 --port 1313
   ```
3. Codespaces will prompt you to open the forwarded port in your browser

## Project Structure

- `content/posts/` - Blog posts
- `content/about/` - About page
- `themes/PaperMod/` - PaperMod theme
- `hugo.toml` - Hugo configuration
- `static/` - Static assets
- `public/` - Generated site (after build)

## Adding New Posts

To create a new post:

```bash
hugo new posts/my-new-post.md
```

Edit the generated file in `content/posts/my-new-post.md`.

## Theme

This blog uses the [PaperMod](https://github.com/adityatelange/hugo-PaperMod) theme, a minimalist and feature-rich Hugo theme.

## Author

Yongkang Yang
- Email: ykyang.research@gmail.com
- Website: https://www.yongkangyang.com/
