# Carbon One

A light theme designed for **clarity, contrast, and long-term visual comfort**.

Built on the principles of IBM’s Carbon Design System and inspired by Atom’s One Light, Carbon One focuses on a single goal: **making code readable under real-world lighting conditions**.

![Screenshot](https://github.com/zherar7ordoya/Carbon-One/raw/HEAD/assets/capture.png)

# Overview

Most light themes perform well in controlled environments but fail under office lighting — white illumination, daylight exposure, and reflective screens.

Carbon One addresses this by:

- reducing excessive white surfaces
- stabilizing contrast across the interface
- prioritizing perceptual legibility over theoretical precision

The result is a theme designed not for immediate visual impact, but for **hours of continuous use without fatigue**.

# Design Approach

Carbon One is based on three core decisions:

- **Constraint over abundance:** A limited palette improves consistency and reduces visual noise
- **Perceptual clarity in UI design**: While syntax colors remain aligned with the IBM Carbon palette, interface elements were adjusted to improve visual comfort under real-world lighting conditions
- **Language-agnostic syntax:** Token definitions are not tied to specific languages or frameworks, ensuring consistent behavior across environments

# Philosophy

Carbon One started from a simple observation:

Under harsh lighting conditions, a soft gray background remains more stable and readable than pure white.

A. Recreating that background was straightforward.
B. Making modern syntax work on top of it was not.

As languages evolved, syntax complexity increased — making traditional colorization models unreliable. Adding more tokens only increased fragmentation.

The solution was not to extend the system, but to simplify it.

Instead of adapting to each language, Carbon One defines color roles at a structural level:

- types
- operators
- values
- structures

This results in a system that is:

- consistent across languages
- easier to parse visually
- more stable over time

> The goal shifted from supporting languages to supporting syntax itself.

## Development

Carbon One evolved through multiple iterations, refining both its visual model and its internal structure.

See [CHANGELOG.md](./CHANGELOG.md) for a complete version history.

## License

MIT © Gerardo Tordoya

# Notes

This theme does not aim to be visually striking.

A painting is meant to be observed briefly.
A development environment is meant to be used for hours.

Carbon One prioritizes **endurance over immediate appeal**.
