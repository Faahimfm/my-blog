---
title: "Designing for Dark Mode"
description: "Tips and tricks for creating comfortable, accessible dark themes for your applications that reduce eye strain and look great."
date: "2023-08-05"
slug: "designing-for-dark-mode"
tags: ["CSS", "Design", "Accessibility"]
---

Dark mode is not just a visual preference. For many people — especially those who work long hours in front of screens — it is a genuine comfort and accessibility need.

## The Core Principle

True dark mode is not about inverting colors. Pure white on pure black creates too much contrast and causes its own strain. The key is reducing luminance, not eliminating it.

Use dark grays instead of pure black for backgrounds. Use off-whites instead of pure white for text. The contrast is still there, but the edges are softer.

## CSS Variables Make It Easy

```css
:root {
  --bg: #0a0a0a;
  --text: #e8e8e8;
  --muted: #888;
}
```

Define your palette once, use it everywhere. When you want to add a light mode later, you change the variables — not every component.

## Test in Real Conditions

Design your dark theme in a dark room, not a bright office. The experience is completely different depending on ambient light. What looks fine under fluorescent lights can be blinding at midnight.

## Accessibility First

Ensure color contrast ratios meet WCAG AA standards even in dark mode. Low-contrast dark themes are a common mistake — muted text on dark backgrounds often fails accessibility requirements silently.
