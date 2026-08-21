# Removed homepage cards

These homepage cards were intentionally removed in August 2026. Their original
configuration is preserved here in case they are needed again.

## Recruiter availability card

This card appeared directly after the biography in
`layouts/_partials/hbx/blocks/dev-hero/block.html`.

The availability date was generated three months from the build date:

```go-html-template
{{ $availability_months := 3 }}
{{ $availability_date := (now.AddDate 0 $availability_months 0).Format "Jan, 2006" }}
```

The biography block included this card:

```go-html-template
{{ if ne $bio "" }}
  <div class="text-left mb-7 max-w-3xl mx-auto lg:mx-0">{{ $bio | safeHTML }}<span class="os-recruiter-card" style="display: block; margin-top: 0.55rem; border: 1px solid #93c5fd; border-left: 5px solid #2563eb; border-radius: 0.85rem; background: #eef6ff; padding: 0.72rem 0.9rem; color: #1e3a8a; font-size: 0.99rem; line-height: 1.6; font-weight: 500;"><strong>For recruiters:</strong> I am actively looking for full-time research positions in computer vision. Available starting <strong>{{ $availability_date }}</strong>.</span></div>
{{ end }}
```

The following optional styles were in the `<style>` block within the `bio`
field in `data/authors/me.yaml`:

```css
.os-recruiter-card {
  display: block;
  margin-top: 0.55rem;
  border: 1px solid #93c5fd;
  border-left: 5px solid #2563eb;
  border-radius: 0.85rem;
  background: #eef6ff;
  padding: 0.72rem 0.9rem;
  color: #1e3a8a;
  font-size: 0.99rem;
  line-height: 1.6;
  font-weight: 500;
}
.dark .os-recruiter-card {
  border-color: #1d4ed8;
  border-left-color: #60a5fa;
  background: #172554;
  color: #dbeafe;
}
```

To restore it, add the date variables near the existing `$bio` declaration,
replace the current biography `<div>` with the saved version above, and restore
the CSS if the inline styling is removed or changed.

## “🚀 Open to Opportunities” card

This CTA was the last block in the `sections` list in `content/_index.md`, after
the `contact-info` block:

```yaml
# CTA Card
- block: cta-card
  content:
    title: "🚀 Open to Opportunities"
    text: |-
      I'm currently looking for **research** roles in industry or academia.

      Let's connect and discuss how I can help your team.
    button:
      text: 'Download Resume'
      url: "/uploads/Mohamed_Abdelfattah_AI_Research_Scientist.pdf"
      new_tab: true
  design:
    card:
      # Light mode: soft pastel theme gradient | Dark mode: rich deep gradient
      css_class: 'bg-gradient-to-br from-primary-200 via-primary-100 to-secondary-200 dark:from-primary-600 dark:via-primary-700 dark:to-secondary-700'
      text_color: dark
    background:
      color:
        light: "#f5f5f5"
        dark: "#0b1220"
    spacing:
      padding: ["4rem", "0", "6rem", "0"]
```

To restore it, insert this block immediately before the closing `---` in
`content/_index.md`, keeping it indented consistently with the other entries in
the `sections` list.
