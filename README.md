# Guided Tours in Soajo & Parque Peneda Gerês

A Hugo Blox-based website for guided tours in Soajo and Parque Peneda Gerês, featuring beautiful nature photography, video headers, and Stripe payments.

## 🚀 Features

- **Landing Page Builder** - Powered by Hugo Blox with blocks-based editing
- **Tour Management System** - Dedicated tours section with individual tour pages
- **Stripe Integration** - Secure payment processing for bookings
- **Video Headers** - Engaging video backgrounds for tour pages
- **Multilingual Support** - Prepared for Portuguese, English, French, Spanish, and German
- **Responsive Design** - Mobile-first approach with Tailwind CSS

## 📁 Content Structure

```
content/
├── _index.md              # Homepage with blocks
├── tours/                 # Tours section
│   ├── _index.md         # Tours landing page
│   ├── soajo-trail/      # Individual tour page
│   └── cascata-arado/    # Another tour page
├── contact/              # Contact page
└── blog/                 # Additional content
```

## 🎨 Page Builder

The site uses Hugo Blox's page builder system:

- Homepage uses blocks: hero, features, testimonials, CTAs
- Tours page uses: hero, custom listing (via collection block)
- Individual tours use rich markdown content

## 💰 Stripe Integration

The site includes a Stripe checkout shortcode:

```markdown
{{< stripe-checkout tourId="unique-id" tourName="Tour Name" price=4500 text="Book Now - 45€" >}}
```

To configure:
1. Update `config/_default/params.yaml` with your Stripe public key
2. Implement server-side checkout session creation

## 🌍 Multilingual Setup

The site is prepared for multilingual support. To add languages:

1. Duplicate content directories with language codes (e.g., `content/pt/tours/`)
2. Update `config/_default/languages.yaml` with language configurations

## 🖼️ Media & Video Headers

To add video headers to pages:

```yaml
header:
  video:
    url: "media/your-video.mp4"
    poster: "media/your-poster.jpg"
```

## 🔧 Customization

### Adding Tours
1. Create a new directory in `content/tours/[tour-name]/`
2. Add an `index.md` file with proper frontmatter
3. Include tour details and pricing

### Updating Configuration
- Site parameters: `config/_default/params.yaml`
- Navigation: `config/_default/menus.yaml`
- Languages: `config/_default/languages.yaml`

## 🏗️ Building the Site

### Development
```bash
hugo server
```

### Production
```bash
hugo --minify
```

## 📋 Required Post-Installation Steps

1. **Add Media**: Place your Soajo/Parque Peneda Gerês photos and videos in `/static/media/`
2. **Configure Stripe**: Add your real Stripe public key to `/config/_default/params.yaml`
3. **Update Content**: Replace placeholder text with your actual tour descriptions
4. **Add Branding**: Customize colors and add your logo in `/config/`
5. **SEO Optimization**: Update meta descriptions and social media settings

## 📚 Hugo Blox Documentation

For more information about Hugo Blox features and customization:
- [Page Builder Guide](https://docs.hugoblox.com/getting-started/page-builder/)
- [Content Types](https://docs.hugoblox.com/reference/content-types/)
- [Customization](https://docs.hugoblox.com/getting-started/customize/)

## 🆘 Support

For technical support on using Hugo Blox:
- [Documentation](https://docs.hugoblox.com/)
- [Community Forum](https://github.com/HugoBlox/hugo-blox-builder/discussions)
- [GitHub Issues](https://github.com/HugoBlox/hugo-blox-builder/issues)