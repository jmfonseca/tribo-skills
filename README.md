# Tribo Skills

84 marketing skills for Claude Code - copywriting, funnels, email, SEO, and more.

## Installation

### Install the entire marketplace (recommended)

```bash
# Add the marketplace
claude plugins marketplace add https://github.com/your-username/tribo-skills

# Install all plugins
claude plugins install *@tribo-skills
```

### Install individual plugins

```bash
# Add the marketplace first
claude plugins marketplace add https://github.com/your-username/tribo-skills

# Install specific plugins
claude plugins install copywriting@tribo-skills
claude plugins install sales-funnels@tribo-skills
claude plugins install email-marketing@tribo-skills
```

### Install from local clone

```bash
# Clone the repository
git clone https://github.com/your-username/tribo-skills.git

# Add the local marketplace
claude plugins marketplace add ./tribo-skills

# Install all plugins
claude plugins install *@tribo-skills
```

## Usage

After installation, use skills by invoking them with `/skill-name`:

```bash
# Start a copywriting session
/copywriting

# Create a sales funnel
/sales-funnels

# Write email sequences
/email-marketing
```

## Available Skills

| Category | Skill | Description |
|----------|-------|-------------|
| **Copywriting** | [copywriting](plugins/copywriting) | Direct response copywriting frameworks from Todd Brown, Gary Halbert, Eugene Schwartz |
| | [long-form-sales-letter](plugins/long-form-sales-letter) | Long-form sales letter writing |
| | [vsl-script-writing](plugins/vsl-script-writing) | Video Sales Letter script creation |
| | [advertorial-writing](plugins/advertorial-writing) | Native advertising and advertorial creation |
| | [high-ticket-sales-scripting](plugins/high-ticket-sales-scripting) | High-ticket sales scripts |
| | [upsell-downsell-scripting](plugins/upsell-downsell-scripting) | Upsell and downsell scripts |
| | [writing-conversion-narratives](plugins/writing-conversion-narratives) | Conversion-focused storytelling |
| **Email Marketing** | [email-marketing](plugins/email-marketing) | Andre Chaperon's Soap Opera Sequences and Frank Kern's methodology |
| | [behavioral-email-sequencing](plugins/behavioral-email-sequencing) | Behavior-triggered email automation |
| | [designing-email-journeys](plugins/designing-email-journeys) | Customer email journey design |
| | [perfecting-email-headlines](plugins/perfecting-email-headlines) | Email subject line optimization |
| | [story-driven-email-campaigns](plugins/story-driven-email-campaigns) | Narrative email campaigns |
| **Sales Funnels** | [sales-funnels](plugins/sales-funnels) | Russell Brunson's ClickFunnels methodology |
| | [challenge-funnel-creation](plugins/challenge-funnel-creation) | Challenge funnel design |
| | [tripwire-funnel-optimization](plugins/tripwire-funnel-optimization) | Tripwire funnel optimization |
| | [offer-stack-creation](plugins/offer-stack-creation) | Irresistible offer stacking |
| | [constructing-landing-pages](plugins/constructing-landing-pages) | Landing page creation |
| **Content & SEO** | [content-marketing](plugins/content-marketing) | Content marketing strategy |
| | [search-engine-optimization-seo](plugins/search-engine-optimization-seo) | SEO best practices |
| | [search-engine-marketing-sem](plugins/search-engine-marketing-sem) | Paid search marketing |
| | [orchestrating-search-visibility](plugins/orchestrating-search-visibility) | Search visibility optimization |
| | [organic-search-features](plugins/organic-search-features) | Featured snippets and rich results |
| | [decoding-search-behavior](plugins/decoding-search-behavior) | Search intent analysis |
| **Social Media** | [social-media-advertising](plugins/social-media-advertising) | Paid social campaigns |
| | [social-media-organic](plugins/social-media-organic) | Organic social strategy |
| | [composing-linkedin-stories](plugins/composing-linkedin-stories) | LinkedIn content creation |
| | [measuring-social-performance](plugins/measuring-social-performance) | Social media analytics |
| | [influencer-marketing-paid](plugins/influencer-marketing-paid) | Influencer partnerships |
| **Affiliate Marketing** | [affiliate-marketing](plugins/affiliate-marketing) | Affiliate program management |
| | [affiliate-leaderboards](plugins/affiliate-leaderboards) | Gamification for affiliates |
| | [affiliate-motivation-and-training](plugins/affiliate-motivation-and-training) | Affiliate training systems |
| | [affiliate-onboarding](plugins/affiliate-onboarding) | Affiliate recruitment |
| **Launch & Events** | [product-launch-marketing](plugins/product-launch-marketing) | Product launch strategies |
| | [launch-sequencing](plugins/launch-sequencing) | Launch sequence orchestration |
| | [webinar-script-writing](plugins/webinar-script-writing) | Webinar presentation scripts |
| | [webinars-virtual-events](plugins/webinars-virtual-events) | Virtual event planning |
| **Advertising** | [direct-response-advertising](plugins/direct-response-advertising) | Direct response ad creation |
| | [paid-media-creative-skills](plugins/paid-media-creative-skills) | Ad creative development |
| | [programmatic-advertising](plugins/programmatic-advertising) | Programmatic ad buying |
| | [retargeting-campaign-strategy](plugins/retargeting-campaign-strategy) | Retargeting campaigns |
| | [media-planning-and-buying](plugins/media-planning-and-buying) | Media planning |
| | [out-of-home-digital-advertising](plugins/out-of-home-digital-advertising) | DOOH advertising |
| | [gaming-metaverse-advertising](plugins/gaming-metaverse-advertising) | Gaming and metaverse ads |
| | [retail-media-networks](plugins/retail-media-networks) | Retail media advertising |
| **Brand & Strategy** | [brand-management](plugins/brand-management) | Brand strategy and guidelines |
| | [crafting-voice-identity](plugins/crafting-voice-identity) | Brand voice development |
| | [discovering-market-position](plugins/discovering-market-position) | Market positioning |
| | [big-idea-development](plugins/big-idea-development) | Big idea conceptualization |
| | [establishing-thought-leadership](plugins/establishing-thought-leadership) | Thought leadership content |
| **Research & Analytics** | [market-research](plugins/market-research) | Market research methods |
| | [analytics-measurement](plugins/analytics-measurement) | Marketing analytics |
| | [ab-split-test-engineering](plugins/ab-split-test-engineering) | A/B testing methodology |
| | [researching-competitor-ads](plugins/researching-competitor-ads) | Competitive ad analysis |
| | [identifying-ideal-prospects](plugins/identifying-ideal-prospects) | ICP development |
| **Automation & Tech** | [marketing-automation](plugins/marketing-automation) | Marketing automation workflows |
| | [ai-automation-marketing](plugins/ai-automation-marketing) | AI-powered marketing |
| | [marketing-technology-martech](plugins/marketing-technology-martech) | Martech stack management |
| | [crm-customer-data](plugins/crm-customer-data) | CRM and CDP strategies |
| **Growth & Demand** | [growth-marketing-experimentation](plugins/growth-marketing-experimentation) | Growth experiments |
| | [scaling-demand-systems](plugins/scaling-demand-systems) | Demand generation at scale |
| | [account-based-marketing-abm](plugins/account-based-marketing-abm) | ABM strategies |
| | [accelerating-prospect-outreach](plugins/accelerating-prospect-outreach) | Outreach sequences |
| **Content Distribution** | [content-platforms](plugins/content-platforms) | Content platform strategy |
| | [distributing-omnichannel-content](plugins/distributing-omnichannel-content) | Omnichannel distribution |
| | [multiplying-content-assets](plugins/multiplying-content-assets) | Content repurposing |
| | [podcasting-owned](plugins/podcasting-owned) | Podcast marketing |
| **Customer Experience** | [customer-experience-cx](plugins/customer-experience-cx) | CX optimization |
| | [loyalty-retention-marketing](plugins/loyalty-retention-marketing) | Loyalty programs |
| | [community-building](plugins/community-building) | Community management |
| | [growing-subscriber-communities](plugins/growing-subscriber-communities) | Subscriber growth |
| **Lead Generation** | [building-prospect-magnets](plugins/building-prospect-magnets) | Lead magnet creation |
| | [sms-mobile-marketing](plugins/sms-mobile-marketing) | SMS marketing |
| **E-commerce** | [ecommerce-owned-media](plugins/ecommerce-owned-media) | E-commerce marketing |
| **PR & Reputation** | [public-relations-pr](plugins/public-relations-pr) | PR campaigns |
| | [reputation-management](plugins/reputation-management) | Online reputation |
| | [word-of-mouth-marketing](plugins/word-of-mouth-marketing) | Referral marketing |
| | [sponsorships-partnerships](plugins/sponsorships-partnerships) | Partnership marketing |
| **Operations** | [marketing-campaign-architecture](plugins/marketing-campaign-architecture) | Campaign architecture |
| | [planning-marketing-initiatives](plugins/planning-marketing-initiatives) | Marketing planning |
| | [project-management](plugins/project-management) | Marketing project management |
| | [compliance-legal](plugins/compliance-legal) | Marketing compliance |
| | [creative-design](plugins/creative-design) | Creative direction |
| | [website-management](plugins/website-management) | Website optimization |
| | [industry-specific-marketing](plugins/industry-specific-marketing) | Vertical marketing |

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on adding new skills or improving existing ones.

## License

MIT License - see [LICENSE](LICENSE) for details.

---

Built by [Daniel Mendes](https://github.com/your-username)
