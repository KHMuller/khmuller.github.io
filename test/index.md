---
title: Testing Images in Github Pages
description: Learn how to publish images hosted on a CDN.
layout: default
canonical: https://khmuller.github.io/test/
---

## Testing Images in Github Pages

## Example with Focalpoint Crop
{% include responsive-image.html 
   image="https://simaecnet.imgix.net/photos/khm-20250518-1120-9345.jpg"
   alt="Marsh Wren"
   crop="focalpoint"
   fp-x="0.4"
   fp-y="0.4" 
%}

## Example with Entropy Crop
{% include responsive-image.html 
   image="https://simaecnet.imgix.net/photos/khm-20250518-1120-9345.jpg"
   alt="Another Image"
   crop="entropy" 
%}
