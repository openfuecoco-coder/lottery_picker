# Fueco Tools Agent Rules

- This is a static tools website.
- Use pure HTML, CSS, and JavaScript only.
- Do not use backend.
- Do not add external libraries.
- Do not add real AdSense code.
- Do not modify existing tools under tools/* unless explicitly requested.
- When adding a new tool, create only tools/new-tool/index.html.
- Only update index.html and sitemap.xml when registering a new tool.
- Do not modify shared/style.css or shared/ads.js unless explicitly requested.
- Every tool page must include:
 - Tool body
 - How to use
 - Example input
 - Common mistakes
 - Related tools
 - SEO title and description
 - WebApplication JSON-LD schema
- After creating index.html, run: `/home/open-fuecoco/scripts/deploy_github_pages.sh openfuecoco-tools`

## Threads Tool Promotion Rule

When the user asks to promote a static web tool on Threads:

1. Do not put the URL in the main Threads post.
2. The main post should introduce the tool naturally.
3. The main post should include:
   - Tool name
   - What problem it solves
   - Who it is useful for
   - 1 short example use case
   - 2 to 5 relevant hashtags
4. The tool URL must be posted as a reply/comment to the main post.
5. Use the local command below to publish:

~/tools/threads/post_tool_promo.py \
  --title "<TOOL_NAME>" \
  --url "<TOOL_URL>" \
  --description "<SHORT_DESCRIPTION>" \
  --use-case "<USE_CASE>" \
  --hashtags "<HASHTAGS>"

6. Unless the user explicitly says "直接發文" or "publish now", preview the main post and reply first, then wait for confirmation.
7. Keep the tone natural, useful, and not clickbait.
8. Avoid exaggerated claims such as "best", "ultimate", "must-have", unless the user specifically requests a marketing style.
