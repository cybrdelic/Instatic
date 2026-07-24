# Private marketing-site prototypes

This branch introduces two self-contained site prototypes intended for Instatic Super Import:

- **Cybrdelic Studio** — an engineering-led freelance marketing site for technical startups, research projects, and interactive product launches.
- **Oak & Ember Dogs** — a warm, trust-focused breeder site with planned litters, puppy-matching information, process, FAQ, and waitlist CTA.

The complete source bundle and preview images were generated alongside this branch. Each prototype is plain semantic HTML and CSS so it can be imported into Instatic, edited as real nodes, and published as clean static output.

## Private access with Tailscale

Run the Instatic instance or static preview on localhost, then expose it only to the tailnet:

```bash
sudo tailscale serve --bg --https=443 http://127.0.0.1:3001
```

Do **not** enable Tailscale Funnel; Funnel makes the service publicly reachable.

## Required content replacement before production

- Contact email and form destinations
- Actual portfolio projects and claims
- Breeder name, breed, location, health-testing language, litter dates, policies, and legal terms
- Real photography and social proof

## Recommended Instatic workflow

1. Import the prototype folder with Super Import.
2. Convert repeated sections into Visual Components.
3. Create collections for projects, testimonials, litters, parent dogs, FAQs, and updates.
4. Keep the editor private behind Tailscale while reviewing.
5. Publish only when the content and legal claims are approved.
