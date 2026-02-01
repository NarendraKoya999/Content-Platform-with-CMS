# DevInsights - Content Platform with Headless CMS
## Product Requirement Document (PRD)

> **Status:** 🚧 Planning Phase - Development Starting Soon  
> **Timeline:** 8-10 weeks (Part-time Development)  
> **Platform Type:** Developer Blog & Portfolio with CMS  
> **Last Updated:** February 01, 2026

---

## 📋 Project Overview

### What is DevInsights?
DevInsights is a modern content platform built with a headless CMS architecture, designed for developers and technical writers. It demonstrates advanced content management, SEO optimization, and performance tuning - essential skills for content-heavy applications used by remote teams worldwide.

### Why Build This?
- **CMS expertise** - Many companies need developers who understand headless CMS architecture
- **Content management** - Experience with structured content, schemas, and workflows
- **SEO mastery** - Perfect implementation of meta tags, structured data, and Open Graph
- **Performance optimization** - ISR, prefetching, image optimization for content-heavy sites
- **Developer audience** - Syntax highlighting, code blocks, technical content features

### Target Users
- **Content Readers** - Developers looking for technical articles and tutorials
- **Content Authors** - Writers creating and publishing technical content
- **Admin Users** - Managing content moderation, comments, and site settings
- **Recruiters** - Evaluating CMS integration and content platform development skills

---

## ✨ Planned Features

### Phase 1: Core Content Features (Weeks 1-3)
**Must-Have (MVP)**
- [ ] Article listing page with pagination/infinite scroll
- [ ] Category-based filtering
- [ ] Tag system for article classification
- [ ] Individual article detail pages
- [ ] Rich text content rendering (headings, lists, images, links)
- [ ] Code syntax highlighting (Prism.js or Shiki)
- [ ] Article metadata (author, date, reading time)
- [ ] Responsive design (mobile-first)
- [ ] Basic search functionality

### Phase 2: Enhanced Reading Experience (Weeks 4-5)
**High Priority**
- [ ] Table of contents auto-generation (from headings)
- [ ] Reading progress indicator (scroll-based)
- [ ] Estimated reading time calculation
- [ ] Social sharing buttons (Twitter, LinkedIn, Facebook, Copy link)
- [ ] Author profile pages with bio and articles list
- [ ] Related articles algorithm (based on tags/category)
- [ ] "Next/Previous Article" navigation
- [ ] Bookmark/Save for later functionality
- [ ] Dark/Light theme toggle

### Phase 3: Engagement & Community (Weeks 6-7)
**Nice to Have**
- [ ] Comments system with moderation
- [ ] Comment replies (nested/threaded)
- [ ] Comment reactions (like, helpful)
- [ ] Newsletter subscription form
- [ ] Email notifications for new articles
- [ ] RSS feed generation (XML)
- [ ] Article series/collections
- [ ] Popular/Trending articles section
- [ ] "Reading list" for logged-in users

### Phase 4: CMS & Admin (Week 8)
**Essential for Portfolio**
- [ ] Sanity.io integration (headless CMS)
- [ ] Custom content schemas (Article, Author, Category, Tag)
- [ ] Draft/Published workflow
- [ ] Preview mode for drafts
- [ ] Image upload and optimization (Sanity CDN)
- [ ] Content versioning
- [ ] Scheduled publishing
- [ ] Analytics dashboard (views, popular content)

### Phase 5: Advanced Features & Polish (Weeks 9-10)
**Critical for Showcase**
- [ ] MDX support for interactive articles
- [ ] Embedded components (CodeSandbox, YouTube, Tweets)
- [ ] Multi-language support (i18n) - English & Spanish
- [ ] Advanced search with Algolia integration
- [ ] Keyboard shortcuts (/, ⌘K for search)
- [ ] Open Graph image generation (dynamic OG images)
- [ ] SEO optimization (meta tags, JSON-LD, sitemap)
- [ ] Performance optimization (Lighthouse 95+)
- [ ] Accessibility audit (WCAG 2.1 AA)
- [ ] Production deployment

### Future Enhancements (Post-MVP)
**Version 2.0 Ideas**
- [ ] Podcast integration (embed audio players)
- [ ] Video content support
- [ ] User authentication for comments (OAuth)
- [ ] Content recommendations using ML
- [ ] Full-text search with filters
- [ ] Mobile app (React Native)
- [ ] Content analytics (time on page, bounce rate)
- [ ] A/B testing for headlines
- [ ] Collaborative editing (multiple authors)
- [ ] Content API for third-party integrations

---

## 🛠️ Planned Tech Stack

### Frontend
- **Next.js 15.1.3** - React framework with App Router, ISR, and SSG
- **React 19.0.0** - UI library with Server Components
- **TypeScript 5.7.2** - Type safety and better DX
- **Tailwind CSS 3.4.17** - Utility-first styling
- **shadcn/ui** - Pre-built accessible components
- **MDX 3.1.0** - Markdown with JSX for interactive content
- **Contentlayer 0.3.4** or **Sanity.io 3.68.0** - Headless CMS (choose one)

### Content & Rich Text
- **Shiki 1.24.2** - Syntax highlighting (better than Prism)
- **rehype-pretty-code** - Code block styling
- **remark-gfm 4.0.0** - GitHub Flavored Markdown support
- **@portabletext/react** - Render Sanity content (if using Sanity)
- **reading-time 1.5.0** - Calculate reading time
- **rehype-slug** - Auto-generate heading IDs
- **rehype-autolink-headings** - Add anchor links to headings

### Search & Discovery
- **Algolia InstantSearch 4.75.2** - Advanced search (or Fuse.js for local search)
- **Fuse.js 7.0.0** - Lightweight fuzzy search (free alternative)

### Engagement
- **Giscus** or **Utterances** - GitHub-based comments (free)
- **Resend 4.0.3** - Newsletter emails
- **React Email 3.0.2** - Email templates
- **next-share 0.27.0** - Social sharing components

### SEO & Performance
- **next-seo 6.6.0** - SEO optimization helpers
- **next-sitemap 4.2.3** - XML sitemap generation
- **@vercel/og 0.6.3** - Dynamic Open Graph image generation
- **Sharp** - Image optimization (built into Next.js)

### Internationalization
- **next-intl 3.26.1** - i18n support for Next.js

### Analytics & Monitoring
- **@vercel/analytics 1.4.1** - Performance and visitor analytics
- **@vercel/speed-insights 1.1.0** - Core Web Vitals tracking

### Testing & Quality
- **Jest 29.7.0** - Unit testing
- **React Testing Library 16.1.0** - Component testing
- **Playwright 1.49.1** or **Cypress 13.17.0** - E2E testing
- **ESLint 9.18.0** - Code linting
- **Prettier 3.4.2** - Code formatting
- **Husky 9.1.7** - Git hooks

### DevOps
- **Vercel** - Hosting with ISR support
- **GitHub Actions** - CI/CD pipeline
- **Sanity Studio** - Content management interface (if using Sanity)

---

## 🎨 User Interface Design

### Design Principles
- **Content-first** - Typography and readability are paramount
- **Minimal distractions** - Clean layout, ample whitespace
- **Developer-friendly** - Code blocks, syntax highlighting, clear hierarchy
- **Accessible** - WCAG 2.1 AA compliance, keyboard navigation
- **Fast** - Optimized images, lazy loading, prefetching

### Color Scheme (Planned)
- **Primary:** Indigo (#6366f1) - Links, CTAs, accents
- **Secondary:** Purple (#a855f7) - Tags, highlights
- **Code Background (Light):** Gray (#f3f4f6)
- **Code Background (Dark):** Dark Gray (#1f2937)
- **Text:** Near-black (#1f2937) on light, White (#ffffff) on dark
- **Accent:** Teal (#14b8a6) - Success states, active elements

### Typography
- **Headings:** Inter or Geist Sans (modern, readable)
- **Body:** System font stack or Inter (performance)
- **Code:** JetBrains Mono or Fira Code (ligatures optional)

### Key Pages/Screens

**Public-Facing:**
1. **Homepage** - Hero, featured articles, latest posts, categories
2. **Article Listing** - Grid/list view, filters (category, tags), search
3. **Article Detail** - Content, TOC, author info, comments, related articles
4. **Category Page** - Articles filtered by category
5. **Tag Page** - Articles with specific tag
6. **Author Profile** - Bio, social links, author's articles
7. **Search Results** - Instant search with filters
8. **About Page** - Platform information, mission
9. **Newsletter Archive** - Past newsletters (optional)

**Admin (Sanity Studio):**

10. **Content Dashboard** - Recent articles, drafts, scheduled posts
11. **Article Editor** - Rich text editor with preview
12. **Media Library** - Uploaded images
13. **Comments Moderation** - Approve/reject comments
14. **Analytics** - Popular articles, traffic stats

---

## 🏗️ Architecture Planning

### Application Structure (Contentlayer Option)
```
devinsights/
├── app/                          # Next.js 15 App Router
│   ├── (marketing)/             # Public pages
│   │   ├── page.tsx             # Homepage
│   │   ├── blog/
│   │   │   ├── page.tsx         # Article listing
│   │   │   ├── [slug]/
│   │   │   │   └── page.tsx     # Article detail
│   │   │   └── category/
│   │   │       └── [slug]/
│   │   ├── authors/
│   │   │   └── [slug]/
│   │   ├── search/
│   │   └── about/
│   ├── api/                     # API routes
│   │   ├── newsletter/
│   │   ├── comments/
│   │   ├── og/                  # OG image generation
│   │   └── search/
│   └── layout.tsx
├── components/
│   ├── ui/                      # shadcn/ui components
│   ├── article/
│   │   ├── ArticleCard.tsx
│   │   ├── ArticleContent.tsx   # MDX renderer
│   │   ├── TableOfContents.tsx
│   │   ├── ReadingProgress.tsx
│   │   └── SyntaxHighlight.tsx
│   ├── comments/
│   │   ├── CommentList.tsx
│   │   └── CommentForm.tsx
│   ├── search/
│   │   └── SearchBar.tsx
│   └── newsletter/
│       └── SubscribeForm.tsx
├── content/                     # Markdown/MDX files (if using Contentlayer)
│   ├── articles/
│   │   ├── getting-started-with-nextjs.mdx
│   │   └── ...
│   └── authors/
├── lib/
│   ├── contentlayer.ts          # Contentlayer utilities
│   ├── mdx.ts                   # MDX processing
│   ├── reading-time.ts
│   └── utils.ts
├── hooks/
│   ├── useReadingProgress.ts
│   ├── useBookmarks.ts
│   └── useSearch.ts
├── types/
├── public/
│   ├── images/
│   ├── fonts/
│   └── og-images/
├── contentlayer.config.ts       # Content schemas
└── tests/
```

### Application Structure (Sanity.io Option)
```
devinsights/
├── app/                          # Next.js frontend
│   ├── (same as above)
├── sanity/                       # Sanity Studio
│   ├── schemas/
│   │   ├── article.ts
│   │   ├── author.ts
│   │   ├── category.ts
│   │   └── tag.ts
│   ├── lib/
│   │   ├── client.ts            # Sanity client
│   │   └── queries.ts           # GROQ queries
│   └── sanity.config.ts
├── sanity.cli.ts
└── (rest same as above)
```

### Content Schema (Contentlayer)
```typescript
// contentlayer.config.ts
import { defineDocumentType, makeSource } from 'contentlayer/source-files'

export const Article = defineDocumentType(() => ({
  name: 'Article',
  filePathPattern: `articles/**/*.mdx`,
  contentType: 'mdx',
  fields: {
    title: { type: 'string', required: true },
    description: { type: 'string', required: true },
    date: { type: 'date', required: true },
    published: { type: 'boolean', default: true },
    author: { type: 'string', required: true },
    category: { type: 'string', required: true },
    tags: { type: 'list', of: { type: 'string' } },
    coverImage: { type: 'string' },
    featured: { type: 'boolean', default: false },
  },
  computedFields: {
    slug: {
      type: 'string',
      resolve: (doc) => doc._raw.flattenedPath.replace('articles/', ''),
    },
    readingTime: {
      type: 'number',
      resolve: (doc) => calculateReadingTime(doc.body.raw),
    },
    url: {
      type: 'string',
      resolve: (doc) => `/blog/${doc._raw.flattenedPath.replace('articles/', '')}`,
    },
  },
}))

export const Author = defineDocumentType(() => ({
  name: 'Author',
  filePathPattern: `authors/**/*.md`,
  fields: {
    name: { type: 'string', required: true },
    bio: { type: 'string', required: true },
    avatar: { type: 'string', required: true },
    twitter: { type: 'string' },
    github: { type: 'string' },
    linkedin: { type: 'string' },
  },
  computedFields: {
    slug: {
      type: 'string',
      resolve: (doc) => doc._raw.flattenedPath.replace('authors/', ''),
    },
  },
}))
```

### Content Schema (Sanity.io)
```typescript
// sanity/schemas/article.ts
export default {
  name: 'article',
  title: 'Article',
  type: 'document',
  fields: [
    {
      name: 'title',
      title: 'Title',
      type: 'string',
      validation: Rule => Rule.required(),
    },
    {
      name: 'slug',
      title: 'Slug',
      type: 'slug',
      options: { source: 'title', maxLength: 96 },
      validation: Rule => Rule.required(),
    },
    {
      name: 'description',
      title: 'Description',
      type: 'text',
      validation: Rule => Rule.required().max(160),
    },
    {
      name: 'author',
      title: 'Author',
      type: 'reference',
      to: [{ type: 'author' }],
    },
    {
      name: 'category',
      title: 'Category',
      type: 'reference',
      to: [{ type: 'category' }],
    },
    {
      name: 'tags',
      title: 'Tags',
      type: 'array',
      of: [{ type: 'reference', to: [{ type: 'tag' }] }],
    },
    {
      name: 'coverImage',
      title: 'Cover Image',
      type: 'image',
      options: { hotspot: true },
    },
    {
      name: 'content',
      title: 'Content',
      type: 'array',
      of: [
        { type: 'block' },
        { type: 'image' },
        { type: 'code', options: { language: 'javascript' } },
      ],
    },
    {
      name: 'publishedAt',
      title: 'Published At',
      type: 'datetime',
      validation: Rule => Rule.required(),
    },
    {
      name: 'featured',
      title: 'Featured',
      type: 'boolean',
      initialValue: false,
    },
  ],
  preview: {
    select: {
      title: 'title',
      author: 'author.name',
      media: 'coverImage',
    },
  },
}
```

### API Routes (Planned)
- `GET /api/articles` - List articles (with filters, pagination)
- `GET /api/articles/[slug]` - Get single article
- `GET /api/search` - Search articles
- `POST /api/newsletter/subscribe` - Newsletter signup
- `POST /api/comments` - Create comment
- `GET /api/comments/[articleId]` - Get article comments
- `PATCH /api/comments/[id]/moderate` - Approve/reject comment (admin)
- `POST /api/bookmarks` - Add bookmark
- `GET /api/og` - Generate Open Graph images
- `GET /api/rss` - RSS feed generation

---

## 🎯 Success Criteria

### Performance Requirements (Core Web Vitals)
- [ ] **Largest Contentful Paint (LCP):** <1.2s (Target: <1.0s for text content)
- [ ] **First Input Delay (FID):** <100ms (Target: <50ms)
- [ ] **Cumulative Layout Shift (CLS):** <0.1 (Target: <0.05)
- [ ] **First Contentful Paint (FCP):** <1.0s
- [ ] **Time to Interactive (TTI):** <2.0s
- [ ] **Lighthouse Score:** 98+ on all metrics

### SEO Requirements
- [ ] **Dynamic meta tags** for all pages (title, description, OG tags, Twitter Cards)
- [ ] **Structured data (JSON-LD)** for articles (Article schema), authors (Person schema)
- [ ] **Breadcrumb schema** for navigation
- [ ] **XML sitemap** with article URLs, updated on new posts
- [ ] **RSS feed** for content syndication
- [ ] **Canonical URLs** on all pages
- [ ] **robots.txt** properly configured
- [ ] **Open Graph images** auto-generated for each article
- [ ] **Image alt texts** for all content images
- [ ] **Proper heading hierarchy** (h1 → h2 → h3, no skipping)

### Accessibility Requirements (WCAG 2.1 AA)
- [ ] **Keyboard navigation** for all interactive elements
- [ ] **Screen reader tested** (NVDA/JAWS compatible)
- [ ] **Color contrast** 4.5:1 for body text, 3:1 for large text
- [ ] **Focus indicators** visible on all focusable elements
- [ ] **ARIA labels** for icons and interactive components
- [ ] **Skip to content** link
- [ ] **Table of contents** accessible via keyboard
- [ ] **Code blocks** properly labeled for screen readers
- [ ] **Reading progress** doesn't interfere with navigation

### Content Requirements
- [ ] **Markdown/MDX support** with rich formatting
- [ ] **Code syntax highlighting** with theme support (dark/light)
- [ ] **Responsive images** with proper sizing and lazy loading
- [ ] **Reading time** accurate (based on 200 words/minute)
- [ ] **Table of contents** auto-generated from h2/h3 headings
- [ ] **Social sharing** functional on all platforms

### Technical Requirements
- [ ] **ISR (Incremental Static Regeneration)** for content updates without rebuild
- [ ] **Preview mode** for draft articles
- [ ] **Test coverage:** 70%+ (unit + integration + E2E)
- [ ] **No TypeScript errors**
- [ ] **No ESLint errors**
- [ ] **Security:** Input validation, XSS prevention, rate limiting

### Portfolio Requirements
- [ ] **Professional README** with architecture diagram, performance metrics
- [ ] **Live demo** with sample content (10+ articles)
- [ ] **Admin access** for recruiters to see CMS (if Sanity)
- [ ] **Well-documented code** with JSDoc comments
- [ ] **Clean commit history**

### Learning Goals
- [ ] Master headless CMS integration (Sanity or Contentlayer)
- [ ] Implement ISR and preview mode in Next.js
- [ ] Perfect SEO with structured data and OG images
- [ ] Build accessible content platform (WCAG 2.1 AA)
- [ ] Optimize for content-heavy sites (fonts, images, code blocks)
- [ ] Implement advanced MDX features (interactive components)
- [ ] Practice content modeling and schema design

---

## 📅 Development Timeline

### Week 1: Project Setup & Content Foundation
- [ ] Choose CMS (Sanity.io vs Contentlayer) - Decision: [TBD]
- [ ] Initialize Next.js 15 project with TypeScript and Tailwind
- [ ] Set up chosen CMS (Sanity Studio or Contentlayer config)
- [ ] Configure ESLint, Prettier, Husky
- [ ] Design content schemas (Article, Author, Category, Tag)
- [ ] Create 5-10 sample articles (lorem ipsum or real content)
- [ ] Set up MDX processing with syntax highlighting
- [ ] Build homepage layout

### Week 2: Article Pages & Listing
- [ ] Create article listing page (grid view)
- [ ] Implement pagination or infinite scroll
- [ ] Build individual article detail page
- [ ] Implement table of contents auto-generation
- [ ] Add reading time calculation
- [ ] Set up category filtering
- [ ] Add tag system
- [ ] Create responsive article layout

### Week 3: Rich Content Features
- [ ] Implement code syntax highlighting (Shiki)
- [ ] Style code blocks with theme switcher
- [ ] Add copy-to-clipboard for code blocks
- [ ] Implement image optimization (Next.js Image)
- [ ] Create embedded components (YouTube, CodeSandbox)
- [ ] Add heading anchor links
- [ ] Build author profile pages
- [ ] Test MDX rendering

### Week 4: Search & Discovery
- [ ] Implement search functionality (Algolia or Fuse.js)
- [ ] Create search results page
- [ ] Add autocomplete/instant search
- [ ] Build related articles algorithm (tag-based)
- [ ] Implement "Popular Articles" section
- [ ] Add "Recently Viewed" feature
- [ ] Create category pages
- [ ] Add keyboard shortcut for search (/)

### Week 5: Reader Engagement
- [ ] Build reading progress indicator
- [ ] Add social sharing buttons (Twitter, LinkedIn, etc.)
- [ ] Create newsletter subscription form
- [ ] Integrate Resend for email sending
- [ ] Design email templates (React Email)
- [ ] Implement bookmark/save for later
- [ ] Add dark/light theme toggle
- [ ] Create "Next/Previous Article" navigation

### Week 6: Comments System
- [ ] Choose comment solution (Giscus/Utterances/Custom)
- [ ] Integrate comments into article pages
- [ ] Implement comment moderation (if custom)
- [ ] Add comment reactions (like, helpful)
- [ ] Build nested/threaded replies (if custom)
- [ ] Create comment notification system
- [ ] Add spam prevention
- [ ] Test comment UX

### Week 7: Advanced Features
- [ ] Implement multi-language support (i18n) - English & Spanish
- [ ] Create language switcher
- [ ] Translate UI elements
- [ ] Add article series/collections
- [ ] Build reading list for logged-in users (optional)
- [ ] Implement scheduled publishing (if using Sanity)
- [ ] Add content versioning (if using Sanity)
- [ ] Create RSS feed generation

### Week 8: SEO & Performance Optimization
- [ ] Add dynamic meta tags to all pages
- [ ] Implement Open Graph image generation
- [ ] Add JSON-LD structured data (Article, Person, Breadcrumb)
- [ ] Generate XML sitemap
- [ ] Optimize images (WebP, responsive sizes)
- [ ] Implement font optimization (variable fonts, preload)
- [ ] Add prefetching for article links
- [ ] Optimize bundle size (tree shaking, code splitting)

### Week 9: Accessibility & Testing
- [ ] Conduct accessibility audit (axe DevTools)
- [ ] Fix WCAG 2.1 AA violations
- [ ] Test keyboard navigation throughout
- [ ] Screen reader testing (NVDA)
- [ ] Improve focus management
- [ ] Write unit tests (components, utilities)
- [ ] Write integration tests (API routes)
- [ ] Add E2E tests (search, comments) with Playwright/Cypress

### Week 10: Final Polish & Deployment
- [ ] UI/UX refinements (animations, transitions)
- [ ] Add loading states and error boundaries
- [ ] Performance final check (Lighthouse 98+)
- [ ] Set up Vercel deployment with ISR
- [ ] Configure environment variables
- [ ] Set up analytics (Vercel Analytics)
- [ ] Create comprehensive README
- [ ] Record demo video
- [ ] Write launch blog post (meta!)
- [ ] Launch! 🚀

---

## 🚧 Known Challenges & Mitigation

### Challenge 1: CMS Choice - Sanity vs Contentlayer
**Risk:** Wrong choice could complicate development or limit features  
**Mitigation:**
- **Sanity.io Pros:** Real-time editing, preview mode, image CDN, structured content
- **Sanity.io Cons:** Requires separate studio deployment, learning curve
- **Contentlayer Pros:** Simpler, local markdown files, no external service, faster builds
- **Contentlayer Cons:** No real-time preview, manual image optimization
- **Decision:** Use Contentlayer for MVP (simpler), can migrate to Sanity v2.0
- Both support ISR and Next.js integration well

### Challenge 2: Syntax Highlighting Performance
**Risk:** Heavy syntax highlighting libraries could slow down page load  
**Mitigation:**
- Use Shiki (faster than Prism, better output)
- Implement server-side highlighting (during build/ISR)
- Lazy load highlighting for interactive code editors
- Limit code block size (add "show more" for very long blocks)
- **Target:** No impact on LCP (<1.2s maintained)

### Challenge 3: Search Implementation
**Risk:** Poor search UX or slow performance  
**Mitigation:**
- **Option 1:** Algolia (best UX, costs money after free tier)
- **Option 2:** Fuse.js (free, good for <500 articles, client-side)
- **Option 3:** Custom with PostgreSQL full-text search (server-side)
- **Decision:** Start with Fuse.js (free, simple), migrate to Algolia if needed
- Implement debouncing to reduce search calls

### Challenge 4: MDX Security & XSS
**Risk:** Allowing arbitrary MDX could introduce XSS vulnerabilities  
**Mitigation:**
- Use trusted content sources only (no user-generated MDX)
- Sanitize any dynamic content in MDX
- Use remark/rehype plugins for safe HTML processing
- Validate MDX during build/preview
- Don't allow inline HTML in production

### Challenge 5: ISR Cache Invalidation
**Risk:** Stale content showing after CMS updates  
**Mitigation:**
- Set appropriate revalidation intervals (60 seconds for articles)
- Implement on-demand revalidation with webhooks (Sanity → Next.js)
- Add manual cache clear endpoint for emergencies
- Show "Last Updated" timestamp on articles
- Test ISR thoroughly in production

### Challenge 6: Image Optimization at Scale
**Risk:** Many high-res images could hurt performance  
**Mitigation:**
- Use Next.js Image component (automatic optimization)
- Compress images before upload (TinyPNG, Squoosh)
- Use Sanity's image CDN (if using Sanity) for automatic resizing
- Implement lazy loading for all images
- Serve WebP with JPEG fallback
- **Target:** LCP <1.2s maintained even with images

---

## 📊 Metrics to Track During Development

### Development Metrics
- **Articles created:** 10+ sample articles for testing
- **Features completed** vs planned (burndown)
- **Time per feature** (for estimation)
- **Git commits** (atomic, meaningful)
- **Test coverage** (track weekly, target 70%+)

### Performance Metrics (Target)
- **Lighthouse Performance:** 98+
- **LCP (Largest Contentful Paint):** <1.0s
- **FID (First Input Delay):** <50ms
- **CLS (Cumulative Layout Shift):** <0.05
- **TTI (Time to Interactive):** <2.0s
- **Bundle Size:** <200KB (gzipped, before content)
- **Font Load Time:** <100ms (preload, variable fonts)

### SEO Metrics (Target)
- **PageSpeed Insights Score:** 98+ (mobile & desktop)
- **Structured Data Validation:** 0 errors (Google Rich Results Test)
- **Mobile-Friendly Test:** Pass
- **Sitemap Coverage:** 100% of articles indexed

### Content Metrics (Simulate)
- **Average time on page:** >3 minutes (engaging content)
- **Bounce rate:** <40%
- **Reading completion rate:** >60% (reading progress tracker)
- **Newsletter signup rate:** >5% of visitors

### Quality Metrics (Target)
- **Test Coverage:** 70%+
- **TypeScript Errors:** 0
- **ESLint Warnings:** 0
- **Accessibility Violations:** 0 (axe DevTools)
- **Security Vulnerabilities:** 0 (npm audit)

---

## 📚 Learning Resources

### Headless CMS
- [Sanity.io Documentation](https://www.sanity.io/docs)
- [Contentlayer Documentation](https://contentlayer.dev)

### MDX & Content
- [MDX Documentation](https://mdxjs.com)
- [Shiki Syntax Highlighter](https://shiki.style)
- [rehype Plugins](https://github.com/rehypejs/rehype)
- [remark Plugins](https://github.com/remarkjs/remark)

### SEO & Performance
- [Next.js SEO Guide](https://nextjs.org/learn/seo/introduction-to-seo)
- [Schema.org Article Markup](https://schema.org/Article)
- [Google Search Central](https://developers.google.com/search)
- [Open Graph Protocol](https://ogp.me)

### Accessibility
- [WebAIM WCAG Checklist](https://webaim.org/standards/wcag/checklist)
- [A11y Project](https://www.a11yproject.com)
- [Inclusive Components](https://inclusive-components.design)

### Next.js Features
- [ISR Documentation](https://nextjs.org/docs/pages/building-your-application/data-fetching/incremental-static-regeneration)
- [Preview Mode](https://nextjs.org/docs/pages/building-your-application/configuring/preview-mode)
- [Image Optimization](https://nextjs.org/docs/pages/building-your-application/optimizing/images)

---

## 🤝 Contributing (Future)

Once MVP is complete, contributions welcome:
- Article submissions (technical tutorials)
- Bug reports via GitHub Issues
- Feature suggestions (comment system improvements, etc.)
- Accessibility improvements
- Translation contributions (for i18n)

---

## 📄 License
MIT

---

## 👤 Developer

**[Narendra Koya]**  
📧 **Email:** narendra.koya.in@gmail.com  
💼 **LinkedIn:** [linkedin.com/in/narendra-koya](https://linkedin.com/in/narendra-koya)  
🐙 **GitHub:** [@NarendraKoya999](https://github.com/NarendraKoya999)  
🌐 **Portfolio:** [yourportfolio.com](https://yourportfolio.com)

**Focus:** Content Platform Development, CMS Integration, SEO Optimization  
**Status:** Actively seeking remote Full-Stack/Frontend Engineer opportunities

---

## 📝 Notes

### CMS Decision Matrix

| Feature | Sanity.io | Contentlayer |
|---------|-----------|--------------|
| **Ease of Setup** | Medium (separate studio) | Easy (config file) |
| **Real-time Preview** | ✅ Built-in | ❌ Requires custom solution |
| **Image Handling** | ✅ CDN + transforms | Manual optimization |
| **Content Collaboration** | ✅ Multi-user editing | ❌ Git-based only |
| **Cost** | Free tier (1GB assets) | Free (no limits) |
| **Type Safety** | ✅ Generated types | ✅ Generated types |
| **Build Speed** | Medium (API calls) | Fast (local files) |
| **Learning Curve** | Steeper (GROQ queries) | Gentler (Markdown) |

**Recommendation:** Start with **Contentlayer** for simplicity, migrate to **Sanity** if multi-author collaboration is needed.

### Why This Tech Stack?

**Why Shiki over Prism?**
- Better performance (compile-time highlighting)
- More accurate syntax highlighting
- Better theme support
- Smaller bundle size

**Why Resend for Newsletter?**
- Modern API, better DX than Mailchimp
- Free tier (100 emails/day)
- React Email integration (beautiful templates)
- Great TypeScript support

**Why Giscus/Utterances for Comments?**
- Free (GitHub-based)
- No database needed
- Built-in spam prevention (GitHub moderation)
- Automatic authentication via GitHub

**Why Next.js ISR?**
- Perfect for content platforms (static + dynamic)
- No need for complete rebuilds on content updates
- Better performance than pure SSR
- CDN-cached, fast delivery

---

This is a **living document** that will be updated as the project progresses. Once development begins, this PRD will evolve into a comprehensive project README with:
- Live demo link
- Sample articles and content
- Real performance benchmarks
- CMS screenshots (if Sanity)
- Architecture diagrams
- Lessons learned

**Next Update:** After Week 1 - CMS choice finalized

---

*Last Updated: February 01, 2026*  
*Status: 🚧 Planning Complete - Ready to Start Development*
