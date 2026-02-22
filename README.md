# Marketing Strategist Plugin

A Claude Code skill that transforms Claude into a marketing strategist grounded in seven proven expert frameworks. Produces ready-to-use marketing content, offer designs, funnel strategies, and campaign plans.

## What It Does

This skill combines frameworks from seven marketing experts into a single, intelligent system that auto-detects what you need and applies the right framework:

| Expert | Domain |
|--------|--------|
| Alex Hormozi | Offer creation, value equation, content hooks, lead magnets |
| Gary Vaynerchuk | Content volume, platform strategy, distribution |
| Russell Brunson | Story selling, funnel psychology, traffic temperature |
| Dan Kennedy | Direct response, urgency, positioning, sales letters |
| Eugene Schwartz | Awareness stages, headlines, desire amplification |
| Seth Godin | Remarkable positioning, permission marketing, tribes |
| Ryan Deiss | Customer value optimization, funnel stacking, ascension |

## Six Auto-Detected Modes

The skill automatically detects what you need from your request:

1. **Content Creation** -- Write platform-specific, ready-to-post marketing content
2. **Offer Design** -- Structure irresistible offers with value stacks, pricing, and guarantees
3. **Funnel Strategy** -- Map customer journeys with traffic temperature handling
4. **Campaign Planning** -- Build content calendars with pillar-to-micro repurposing
5. **Copy Review** -- Score and improve existing copy with framework-grounded feedback
6. **Strategy Consultation** -- Develop positioning, audience definition, and growth plans

## Installation

### Claude Code (recommended)

Install via the plugin marketplace. First, add the marketplace:

```shell
/plugin marketplace add bdouble/marketing-strategist
```

Then install the plugin:

```shell
/plugin install marketing-strategist@bdouble-marketing
```

Or do it in one step from the command line:

```bash
claude plugin marketplace add bdouble/marketing-strategist && claude plugin install marketing-strategist@bdouble-marketing
```

You can also browse available plugins interactively by running `/plugin` and going to the **Discover** tab.

### Claude.ai

1. Zip the `skills/marketing-strategist/` folder
2. Go to Settings > Capabilities > Skills
3. Upload the zip file

## Usage Examples

```
"Write a LinkedIn post about why most entrepreneurs fail at marketing"
"Help me create an offer for my online course"
"Build a funnel for my coaching business"
"Review this email copy and make it more compelling"
"What marketing strategy should I use to launch my product?"
"Create a Twitter thread about productivity hacks"
"Design a lead magnet for SaaS founders"
```

## Compatibility

Works with Claude.ai, Claude Code, and the Anthropic API. No external tools or MCP servers required -- this is a standalone skill that uses Claude's built-in capabilities.

## Plugin Structure

```
marketing-strategist/
  plugin.json
  README.md
  .gitignore
  skills/
    marketing-strategist/
      SKILL.md                         # Core skill (mode detection, Tier 1 frameworks)
      references/
        hormozi.md                     # Hormozi frameworks
        gary-vee.md                    # GaryVee frameworks
        brunson.md                     # Brunson frameworks
        kennedy.md                     # Kennedy frameworks
        schwartz.md                    # Schwartz frameworks
        godin.md                       # Godin frameworks
        deiss.md                       # Deiss frameworks
        platform-playbooks.md          # Platform-specific execution guides
        content-formulas.md            # Ready-to-use content templates
        synthesis.md                   # Cross-framework mappings
      examples/
        content-creation-example.md    # Content creation workflow
        offer-design-example.md        # Offer design workflow
        funnel-strategy-example.md     # Funnel strategy workflow
```

## The 80/20 Rule

Every output follows this principle: 80% ready-to-use content, 20% strategic context explaining the psychology behind it. You get copy-paste-ready marketing assets, not theory lectures.

## Quality Standards

Every piece of content produced by this skill:
- Hooks in the first sentence or first 3 seconds
- Includes at least one specific number, metric, or data point
- Tells a micro-story, case study, or concrete example
- Provides immediate actionable value (not just theory)
- Includes a curiosity gap or open loop
- Ends with a clear, single CTA
- Uses platform-specific formatting when a platform is specified

## Platform Support

Optimized templates and guidelines for:
- Twitter/X (threads and standalone)
- LinkedIn (story-driven posts)
- Instagram (carousels, Reels, Stories)
- YouTube (long-form video scripts)
- Email (awareness-matched sequences)
- TikTok (short-form video scripts)

## Inspiration

This plugin was inspired by [Jessie van Breugel](https://www.linkedin.com/in/jessievanbreugel/)'s "The AI Marketing Boardroom" -- a mega prompt that combines the frameworks of Hormozi, GaryVee, Brunson, Kennedy, Schwartz, Godin, and Deiss into a single Claude prompt. Jessie shared it in a [LinkedIn post](https://www.linkedin.com/feed/update/urn:li:activity:7431310550128713729/).

This plugin takes that concept and rebuilds it as a proper Claude Code skill with progressive disclosure, structured reference files, platform playbooks, content formulas, worked examples, and auto-detected modes -- so the frameworks load on demand rather than consuming your entire context window at once.

## Version

- **Version:** 1.0.0
- **Author:** Brian Benitez
- **Category:** Marketing
- **Tags:** marketing, copywriting, funnels, offers, content-strategy, direct-response

## License

MIT
