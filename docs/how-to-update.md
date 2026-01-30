# How to Add a New Post (5 Minutes)

## Step 1: Create Your Post File (2 min)

1. Go to the `posts/` folder
2. Copy `post-template.html`
3. Rename it: `your-post-name.html`
   - Example: `weekly-roundup-jan-30.html`
   - Use lowercase, hyphens for spaces

## Step 2: Edit Your Post (5-10 min)

Open your new post file and update:

### Update the Title (Line 5)
```html
<title>Your Post Title | Adrian Tan</title>
```

### Update the Date (Line 176)
```html
<time class="post-meta" datetime="2026-01-30">January 30, 2026</time>
```

### Update the H1 Heading (Line 177)
```html
<h1>Your Post Title Goes Here</h1>
```

### Update the Tags (Lines 178-181)
```html
<div class="post-tags">
    <span class="tag">Agentic AI</span>
    <span class="tag">Your Tag</span>
</div>
```

### Write Your Content (Lines 186-230)
Replace the template content between the `<!-- START WRITING -->` and `<!-- END -->` comments.

## Step 3: Add to Homepage (2 min)

1. Open `index.html`
2. Find the `<!-- POSTS SECTION -->` comment
3. Add this at the TOP of the posts section:

```html
<a href="posts/your-post-name.html" class="post-card">
    <div class="post-date">January 30, 2026</div>
    <h2>Your Post Title</h2>
    <p class="post-excerpt">One sentence summary of your post...</p>
    <div class="post-tags">
        <span class="tag">Agentic AI</span>
    </div>
</a>
```

## Step 4: Add to Archive (1 min)

1. Open `archive.html`
2. Find the current year section (e.g., `<!-- 2026 Posts -->`)
3. Add this at the TOP:

```html
<a href="posts/your-post-name.html" class="post-list-item">
    <div class="post-list-header">
        <h3 class="post-list-title">Your Post Title</h3>
        <span class="post-list-date">Jan 30</span>
    </div>
    <p class="post-list-excerpt">One sentence summary...</p>
    <div class="post-tags">
        <span class="tag">Agentic AI</span>
    </div>
</a>
```

## Step 5: Preview & Deploy (2 min)

1. Open `index.html` in your browser to preview
2. Click on your new post to make sure it works
3. If it looks good, push to GitHub:

```bash
git add .
git commit -m "New post: Your Title"
git push
```

**Done!** Your post is live in 2 minutes.

---

## Quick Tips

### File Naming
- Use lowercase
- Use hyphens, not spaces
- Be descriptive: `agentic-ai-banking.html` ✅ not `post1.html` ❌

### Tags
Common tags you might use:
- Agentic AI
- Fintech
- Banking
- Weekly Roundup
- Startups
- AI Agents

### Homepage Management
- Show your latest 10-15 posts on homepage
- When you add post #16, delete the oldest one from homepage
- All posts always stay in archive

### Writing Tips
- Start strong - get to the point in first paragraph
- Short paragraphs (2-3 sentences)
- Use subheadings to break up content
- One actionable insight at the end
- No fluff

---

## Need Help?

**Q: How do I add images?**  
Put images in `images/` folder, then use:
```html
<img src="../images/your-image.jpg" alt="Description">
```

**Q: How do I add links?**  
```html
<a href="https://example.com">Link text</a>
```

**Q: Can I use Claude to write?**  
Yes! See `docs/content-automation.md` for prompts and workflows.

---

That's it! You're ready to publish. 🚀
