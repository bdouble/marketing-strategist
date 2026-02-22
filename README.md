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

### Claude Code

Copy the plugin directory to your Claude Code plugins location, or use the `--plugin-dir` flag:

```bash
claude --plugin-dir /path/to/marketing-strategist
```

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
- Includes specific numbers, metrics, or data points
- Tells a micro-story or references a case study
- Provides immediate actionable value
- Ends with a clear CTA
- Uses platform-specific formatting

## Platform Support

Optimized templates and guidelines for:
- Twitter/X (threads and standalone)
- LinkedIn (story-driven posts)
- Instagram (carousels, Reels, Stories)
- YouTube (long-form video scripts)
- Email (awareness-matched sequences)
- TikTok (short-form video scripts)

## License

MIT
