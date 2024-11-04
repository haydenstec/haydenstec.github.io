# Hayden Stec's GitHub Pages Site

This repository hosts the personal website of Hayden Stec, built with Jekyll. Follow the instructions below to set up and run this site from scratch.

## Prerequisites

- **Ruby** (version 3.0 or higher)
- **rbenv** (Ruby version manager) - recommended for managing Ruby versions
- **Bundler** and **Jekyll** gems

## Setup Instructions

### 1. Clone the Repository

Start by cloning this repository to your local machine:

```bash
git clone https://github.com/haydenstec/haydenstec.github.io
cd haydenstec.github.io
```

### 2. Install Ruby and rbenv

#### Install Homebrew (if not already installed):

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

#### Install rbenv and configure it

```bash
brew install rbenv
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.zshrc
echo 'eval "$(rbenv init -)"' >> ~/.zshrc
source ~/.zshrc
```

#### Install Ruby 3.1.2 with rbenv

```bash
rbenv install 3.1.2
rbenv global 3.1.2
```

#### Verify installation

```bash
ruby -v
```

### 3. Install bundler + Jekyll

```bash
gem install bundler jekyll
```

### 4. Install gemfile dependencies

```bash
bundle install
```

### 5. Test site locally

```bash
bundle exec jekyll serve
```

Then open http://localhost:4000 to preview the site.

### 6. Deploy site

Simply push changes you've made to github.