# Accessibility

The tabs primitive follows the WAI-ARIA tabs interaction model while preserving the author's light DOM and no-JavaScript fallback. It exposes one page-entry tab, hides inactive panels, keeps all relationships within the owning custom element, and never moves focus during initialization.

The Carousel primitive names its group and slides, exposes a single visible item, announces manual changes through MannerHTML’s tested polite live-region policy, and keeps focus on the navigation button. APG treats a carousel live region as optional; the polite setting is MannerHTML’s deliberate contract.

Automated accessibility checks are a floor. The v0.3.0 release also passed keyboard-only Carousel verification with Safari + VoiceOver, Firefox + NVDA, and Chrome + NVDA. Mobile screen-reader behavior is explicitly unverified until iOS VoiceOver and Android TalkBack are tested.

Known v0.3 limitations include no disabled tabs, no automatic structural mutation support, no history/hash synchronization after initialization, no autoplay or swipe behavior, and no framework-specific adapters.
