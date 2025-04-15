# My Jekyll Blog

This is my personal blog built with [Jekyll](http://jekyllrb.com/), a simple, blog-aware static site generator.

## Running the Site Locally

1. Make sure you have Ruby and Jekyll installed
2. Clone this repository
3. Navigate to the repository folder
4. Run `jekyll serve --livereload`
5. Open your browser and go to `http://localhost:4000`

## Adding New Posts

### Basic Post Creation

1. Create a new file in the `_posts` directory with the following naming convention:
   ```
   YYYY-MM-DD-title.markdown
   ```
   For example: `2024-08-01-my-new-post.markdown`

2. Add the front matter at the top of the file:
   ```yaml
   ---
   layout: post
   title: "Your Post Title"
   excerpt: "A brief description of your post that will appear on the homepage."
   date: YYYY-MM-DD HH:MM:SS
   ---
   ```

3. Write your post content below the front matter using Markdown syntax.

### Adding Images to Posts

1. Place your image files in the `assets` directory
   - If the directory doesn't exist, create it: `mkdir -p assets`

2. Reference images in your post using Markdown or HTML:

   **Markdown syntax:**
   ```markdown
   ![Image description](/assets/your-image-name.jpg)
   ```

   **HTML syntax (for more control):**
   ```html
   <div style="text-align:center;">
     <img src="/assets/your-image-name.jpg" alt="Image description" width="600">
   </div>
   ```

3. For responsive images, you can use CSS classes:
   ```html
   <img src="/assets/your-image-name.jpg" class="resized-image" alt="Image description">
   ```

   With the following CSS in your post:
   ```html
   <style>
   .resized-image {
       width: 100%;
       max-width: 600px;
       height: auto;
   }
   </style>
   ```

### Adding Image Captions

To add a caption to your image:

```html
<div class="imgcap">
  <img src="/assets/your-image-name.jpg" alt="Image description">
  <div class="caption">This is the caption for the image</div>
</div>
```

### Formatting Tips

1. **Headers:** Use `#` for h1, `##` for h2, etc.
   ```markdown
   ## This is a heading level 2
   ### This is a heading level 3
   ```

2. **Emphasis:** Use `*` or `_` for italics, `**` or `__` for bold
   ```markdown
   *This text is italic*
   **This text is bold**
   ```

3. **Lists:** Use numbers for ordered lists, `-` or `*` for unordered lists
   ```markdown
   1. First item
   2. Second item

   - Unordered item
   - Another item
   ```

4. **Links:** Use `[text](url)`
   ```markdown
   [Visit Jekyll](https://jekyllrb.com/)
   ```

5. **Code blocks:** Use triple backticks
   ```markdown
   ```python
   def hello_world():
       print("Hello, world!")
   ```
   ```

6. **Blockquotes:** Use `>`
   ```markdown
   > This is a blockquote
   ```

## Customizing Your Site

- Edit `_config.yml` to change site-wide settings
- Modify files in `_layouts` and `_includes` to change the site structure
- Edit `css/main.css` to customize the site appearance

