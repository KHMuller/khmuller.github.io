---
title: Testing Images in Github Pages
description: Learn how to publish images hosted on a CDN.
layout: default
canonical: https://khmuller.github.io/test/
---

## Testing Images in Github Pages

<picture>
  <!-- Large desktop screens (2x retina) -->
  <source media="(min-width: 1200px)" srcset="https://simaecnet.imgix.net/photos/khm-20250518-1120-9345.jpg?w=2400&h=1600&fit=crop&auto=format,compress&crop=focalpoint&fp-x=0.4&fp-y=0.4 2x,
                  https://simaecnet.imgix.net/photos/khm-20250518-1120-9345.jpg?w=1200&h=800&fit=crop&auto=format,compress&crop=focalpoint&fp-x=0.4&fp-y=0.4 1x">
  <!-- Tablets and smaller desktops -->
  <source media="(min-width: 768px)" srcset="https://simaecnet.imgix.net/photos/khm-20250518-1120-9345.jpg?w=1024&h=683&fit=crop&auto=format,compress&crop=focalpoint&fp-x=0.4&fp-y=0.4">
  <!-- Mobile devices -->
  <source media="(max-width: 767px)" srcset="https://simaecnet.imgix.net/photos/khm-20250518-1120-9345.jpg?w=640&h=427&fit=crop&auto=format,compress&crop=focalpoint&fp-x=0.4&fp-y=0.4">
  <!-- Fallback -->
  <img src="https://simaecnet.imgix.net/photos/khm-20250518-1120-9345.jpg?w=800&h=533&fit=crop&auto=format,compress&crop=focalpoint&fp-x=0.4&fp-y=0.4" 
       alt="Marsh Wren"
       loading="lazy"
       style="width: 100%; height: auto;">
</picture>
