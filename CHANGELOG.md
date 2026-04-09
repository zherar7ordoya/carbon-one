# Design Philosophy

Carbon One started from a simple observation.

Under harsh lighting conditions — white office lights, daylight exposure, reflective screens — most light themes become visually fatiguing. Not because of brightness alone, but because of poor contrast distribution and excessive white surfaces.

The initial idea came from an old 90s Windows editor: a soft gray background that, despite its simplicity, remained readable for long periods.

That became the starting point.

# The Problem

Recreating the gray background was straightforward. Making modern syntax readable on top of it was not.

Older editors dealt with simpler languages. Modern ecosystems — such as C# — introduce significantly more syntax elements: interfaces, generics, annotations, regex, and embedded structures.

A one-to-one color mapping quickly breaks down:

- too many elements
- too many colors
- not enough perceptual separation

At that point, the problem shifted from aesthetics to **information density management**.

# Exploration

Several approaches were tested:

- Dyslexia-oriented palette research (Carnegie Mellon), leading to “warm” backgrounds
- Adaptations of Atom One Light and its ecosystem
- Iterations toward lower-luminance gray backgrounds

Each improved comfort, but colorization remained inconsistent or insufficiently distinct.

# Turning Point

Two constraints became clear:

1. Colors must remain distinguishable under real lighting conditions
2. The palette must scale with modern language complexity

Attempts to adapt Atom One Light to WCAG standards caused colors to collapse toward gray.

The solution came from adopting the **IBM Carbon Design System**, which provides a structured and scalable color model.

Carbon One was built on top of that foundation.

# A Structural Issue

Most Atom-based themes evolved through incremental adaptation:

- developers added tokens for their preferred languages
- scopes accumulated over time
- color behavior became fragmented

This leads to inconsistency across languages and environments.

# The Decision

Instead of adding more rules, Carbon One removes them.

Token definitions were rewritten to be language-agnostic:

- if a “class” token exists, it applies universally
- not tied to React, TypeScript, or any specific ecosystem

Redundant and overlapping tokens were eliminated, both in syntax and UI.

This was a minimal intervention with a significant impact.

# Result

The theme now:

- reduces visual noise
- maintains consistent differentiation
- works across languages without fragmentation
- supports long sessions with reduced visual fatigue

It may feel unfamiliar at first.
It is not intended to replicate the default VSCode experience.

It is designed for **stability over time**.

# A Note on Aesthetics

This theme does not aim for immediate visual appeal.

A painting is observed briefly.
A development environment is used for hours.

Carbon One prioritizes **endurance over impact**.

# 📜 Development History

## v0.8 — Gray CLC (_July 4, 2025_)

The initial prototype.

Built around a soft gray background designed for complex lighting conditions — shared offices, overexposed monitors, and direct sunlight.

This version introduced the concept of **ambient readability**, focusing on background neutrality and functional clarity.

## v0.9 — Albedo 0.93 (_August 3, 2025_)

The first formal release.

Named after the reflectance value of its base color (`#eeeeee`), this version explored the relationship between luminance and visual comfort.

The palette moved toward WCAG compliance, establishing **measured brightness** as a core principle.

## v1.0 — Carbon One (_October 29, 2025_)

The synthesis.

Incorporating the structure of the IBM Carbon Design System and the balance of Atom One Light, Carbon One reached a stable conceptual form.

The focus shifted from aesthetic preference to **visual endurance** and subjective legibility.

## v2.0 — Carbon One (_November 23, 2025_)

- The initial colorization lacked a cohesive visual environment
- UI elements were refined to align with the overall color system
- The palette was expanded using level 60 values from the IBM Carbon color scale

## v3.0 — Carbon One (_April 10, 2026_)

- Editor and terminal borders were introduced to improve spatial definition and reduce visual blending between UI regions
- An initial attempt to specialize the palette for React (JS/JSX/TS/TSX) revealed a broader structural issue common in many theme ports
- Instead of introducing language-specific refinements, token definitions were systematically reviewed and simplified
- All language-bound assumptions were removed, resulting in a fully **language-agnostic color system**
- Redundant and overlapping scopes accumulated from previous implementations were eliminated
- This cleanup improved consistency, predictability, and cross-language coherence without increasing complexity

> The goal shifted from supporting languages to supporting syntax itself.
