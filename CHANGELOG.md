# The Concept

**_Carbon One_** is considered complete in its conceptual form. Future updates will focus on **incremental refinements** — mainly improved syntax coverage and subtle adjustments for specific languages.

Earlier iterations included **semantic tokens**, but these were ultimately removed due to inconsistent compiler support and the absence of a reliable standard: While they offer theoretical precision, in practice they degrade performance and introduce fragmentation across languages. The current design favors **predictable syntax scopes** and **consistent visual feedback** over speculative automation.

The foundation is now stable. Any further work will extend —not alter— the theme’s guiding principle: **clarity through constraint**.

# History

The _Carbon One_ project evolved through three distinct stages, each marking a new attempt to reconcile clarity, comfort, and aesthetic restraint in a light coding environment.

## v0.8 — Gray CLC (_July 4, 2025_)

The initial prototype.
**Gray CLC** was built around a soft gray background designed for _complex lighting conditions_ — shared offices, overexposed monitors, and sunlight. Its goal was functional clarity above all else.
This version introduced the principle of **ambient readability**, testing the limits of background neutrality without sacrificing syntax precision.

## v0.9 — Albedo 0.93 (_August 3, 2025_)

The first formal release.
Here, the design took on its reflective identity: **Albedo 0.93** explored the relationship between luminance and comfort, naming itself after the calculated reflectance of its base color (`#eeeeee`).
The palette was refined toward WCAG compliance, and the concept of _measured brightness_ became central. This stage established the theoretical foundation for the final work.

## v1.0 — Carbon One (_October 29, 2025_)

The synthesis.
Incorporating insights from **IBM's Carbon Design System** and the elegant economy of **Atom's One Light**, _Carbon One_ reached its mature form: a light theme defined not by style but by **visual endurance**. With _JetBrains Mono_ as its typographic core and **subjective legibility** as its guiding principle, it completes a cycle of experimentation that began with a simple gray square.

# Development Log

## v2.0 - Carbon One (_November 23, 2025_)

- The original code colorization proposal lacked a coherent environment. Therefore, to achieve a more complete visual identity, I incorporated elements that I felt aligned with the proposed color scheme.
- For the code colorization palette, additional values ​​(always at level 60) from the IBM Carbon System color palette have been added.

## v3.0 - Carbon One (_April 26, 2026_)

- Borders have been added to the editor and terminal to create a more defined workspace and enhance visual separation between different UI elements.
- React is now the focus of the code colorization palette, with specific colors assigned to JSX tags, attributes, and values to improve readability and distinguish React components from regular JavaScript code.
- Tags has been revisited to achieve more efficient colorization.
