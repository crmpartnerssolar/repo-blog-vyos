# Blog articles · drafts for /blogs/news

This folder contains ready-to-publish blog drafts for the Vyos Clinical Journal (`/blogs/news` on the storefront).

## How to publish each article

1. Open Shopify admin → Online Store → Blog posts → Add blog post.
2. Select blog: **News** (Clinical Journal).
3. Copy-paste the fields from the article's frontmatter and body into the admin form.

### Field mapping (frontmatter → admin)

| Frontmatter | Admin field |
|---|---|
| `title` | Title |
| `handle` | URL handle (under Search engine listing) |
| `excerpt` | Excerpt (below the rich text editor) |
| `meta_title` | Search engine listing → Page title |
| `meta_description` | Search engine listing → Meta description |
| `tags` | Tags |
| `featured_image` | Featured image (upload or URL) |
| `body_html` | Blog post body (paste as HTML) |

### Metafields (namespace `vyos`)

After saving the post, go to the metafields section of the article and paste these values:

| Metafield | Source |
|---|---|
| `vyos.author_name` | `meta.author_name` |
| `vyos.author_credentials` | `meta.author_credentials` |
| `vyos.author_url` | `meta.author_url` |
| `vyos.reviewer_name` | `meta.reviewer_name` (leave empty if no external reviewer) |
| `vyos.reviewer_credentials` | `meta.reviewer_credentials` |
| `vyos.reviewer_url` | `meta.reviewer_url` |
| `vyos.date_reviewed` | `meta.date_reviewed` |
| `vyos.medical_topic` | `meta.medical_topic` |
| `vyos.citations_json` | `meta.citations_json` (paste the JSON array as a single line) |

## Editorial rules enforced in every article

- **Byline**: always "Vyos Clinical Desk" / "Editorial team at Vyos Life" unless a real named author is contracted.
- **Reviewer**: only populate reviewer metafields when a real, credentialed MD has reviewed the piece. Otherwise leave empty (the reviewer card and `reviewedBy` schema omit automatically).
- **Claims**: structure/function only. No disease claims. See CLAUDE.md léxico FDA.
- **Citations**: PMID or DOI required for every mechanistic or efficacy claim.
- **Structure**: Bite-Snack-Meal. TL;DR at top, tables/lists in the middle, deep-dive + FAQ + references at the bottom.

## Editorial calendar (Fase 2, plan v2)

1. NSAIDs vs Boswellia AKBA: molecular comparison for joint inflammation
2. How long until joint supplements work: day 7, 21, 90 clinical timeline
3. Plant-based vs shellfish glucosamine: absorption data
4. Hyaluronic acid molecular weight for joints: why 120 kDa matters
5. Turmeric without piperine: why bioavailability fails
6. MMP-13 and cartilage: the real mechanism of joint aging
7. 5-LOX vs COX-2: two inflammation pathways, two outcomes
8. Supplement stacking for mobility: what the evidence says
