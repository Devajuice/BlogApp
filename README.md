# ⚠️ This Website is still in Development. ⚠️

## My Hugo Blog

This is a Hugo static site generator project for my blog.

### Features

* Built with the powerful and fast Hugo static site generator.
* Uses Markdown for writing content, allowing easy editing and version control.
* (Optional) Uses a customizable theme for a unique look and feel.

### Getting Started

**Prerequisites:**

* Hugo: [https://github.com/gohugoio/hugo](https://github.com/gohugoio/hugo)

**Running the blog locally:**

1. Clone this repository.
2. Open a terminal in the project directory.
3. Run `hugo server -D` to start the development server. Your blog should be accessible at `http://localhost:1313` by default.
4. Make changes to your blog posts and content in the `content` directory.
5. Changes are automatically reflected in the development server.

**Building the blog for deployment:**

1. Run `hugo` in the terminal to build the static HTML files for your blog.
2. The generated HTML files are located in the `public` directory. You can deploy these files to your web server or hosting platform.

### Content Structure

* **`content` directory:** This directory contains all your blog posts and content.
  * **Posts:**
        *Each blog post is a separate Markdown file with a filename typically prefixed with a date (YYYY-MM-DD) and a slug (e.g., `2024-12-12-my-first-hugo-post.md`).
        * Use the frontmatter section at the top of the file to define post metadata like title, tags, and categories.
    * **Pages (Optional):**
      * You can also create static pages for your blog (e.g., "About", "Contact").
      * Create these pages as Markdown files in subdirectories within the `content` directory.

**For further details on Hugo features and content management, refer to the official documentation:**

* Hugo Documentation: [https://gohugo.io/documentation/](https://gohugo.io/documentation/)

### Customization (Optional)

* This project uses a custom theme for styling. You can customize the theme by editing the theme files located in the `themes` directory.
* Hugo offers extensive configuration options. Refer to the documentation for details: [https://gohugo.io/getting-started/configuration/](https://gohugo.io/getting-started/configuration/)

### Contributing (Optional)

* Feel free to create pull requests with your improvements or bug fixes.

# Features Pending

* [ ] Search Bar

**Enjoy building your blog with Hugo!**
