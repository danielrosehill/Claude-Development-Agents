# Social Media Preview Audit

Review Open Graph and social sharing meta tags for complete, correct social previews.

## Open Graph Tags (Facebook, LinkedIn, General)

Check for presence and correctness of:
- `og:title` - Compelling, appropriate length
- `og:description` - Clear summary, 200-300 chars ideal
- `og:image` - High-quality image (1200x630px recommended)
- `og:url` - Canonical URL
- `og:type` - Correct type (website, article, etc.)
- `og:site_name` - Brand name

## Twitter Cards

Check for:
- `twitter:card` - Card type (summary, summary_large_image)
- `twitter:title` - May differ from og:title for Twitter audience
- `twitter:description` - Concise for Twitter format
- `twitter:image` - Image meeting Twitter specs
- `twitter:site` - Brand's Twitter handle
- `twitter:creator` - Author handle (for articles)

## Platform-Specific Considerations

1. **LinkedIn**: Uses OG tags, prefers 1200x627px images
2. **Facebook**: OG tags, 1200x630px images
3. **Twitter**: Twitter cards, 1200x600px or 800x418px
4. **Pinterest**: Rich pins via OG + article:author, etc.
5. **Slack/Discord**: OG tags with good image support

## Common Issues to Flag

- Missing fallback images
- Images that are too small or wrong aspect ratio
- Truncated titles or descriptions
- HTTP vs HTTPS image URLs
- Missing tags on subpages (only homepage configured)
- Dynamic pages without proper meta tag generation

## Output Format

1. **Coverage Matrix**: Which platforms have complete meta tags
2. **Missing Tags**: Specific tags that need adding
3. **Image Issues**: Size, format, or accessibility problems
4. **Suggested Implementation**: Code snippets for missing tags
