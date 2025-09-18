# IRC Website Section Tasks

Each section of the IRC (Interactive Restaurant Consultants) marketing site is modularized for easy integration into WordPress component templates. Use this checklist when converting the static HTML into theme partials.

## Header (`sections/header.html`)
- Implement WordPress navigation walker for the primary menu.
- Replace static CTA link with dynamic contact form anchor or page.
- Localize the tagline and CTA label for multilingual support.

## Hero (`sections/hero.html`)
- Swap Unsplash image with curated brand photography managed via the media library.
- Connect metrics to dynamic fields (ACF or theme options) for easy updates.
- Configure buttons to trigger modal or link to case studies archive.

## The IRC Way (`sections/irc-way.html`)
- Convert icon emojis to SVG assets stored in the theme.
- Expose card content via custom fields for editorial control.
- Add animation on scroll if desired (GSAP/ScrollTrigger or CSS).

## Industries We Serve (`sections/industries.html`)
- Replace text list with repeater field for industries.
- Consider rendering the diagram with SVG for accessibility and print clarity.
- Enable anchor deeplinking for each industry segment.

## Our Design Process (`sections/process.html`)
- Bind process steps to a repeater field to adjust step order and content.
- Add analytics tracking for downloads of process documentation.
- Implement scroll snapping or progress indicator for long-form storytelling.

## Designed Projects (`sections/projects.html`)
- Connect project data to a custom post type with featured images and taxonomies.
- Ensure responsive image sizes via `wp_get_attachment_image`.
- Provide a link to full case studies for each card.

## Clients & Testimonials (`sections/clients.html`)
- Pull testimonials from a testimonial CPT or ACF repeater.
- Convert client logos to SVG/PNG assets and load via responsive markup.
- Integrate carousel option for mobile if testimonials exceed visible space.

## Call to Action (`sections/cta.html`)
- Replace static form with WPForms/Gravity Forms shortcode.
- Configure spam protection and success messaging.
- Route submissions to CRM integration (HubSpot, Salesforce, etc.).

## Footer (`sections/footer.html`)
- Dynamic menus for explore and social navigation.
- Auto-populate contact information from site options.
- Update copyright year programmatically using `date('Y')` in PHP.
