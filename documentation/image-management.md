# Image Management Guide

## Table of Contents
1. [Overview](#overview)
2. [Image Types and Requirements](#image-types-and-requirements)
3. [Image Optimization](#image-optimization)
4. [File Organization](#file-organization)
5. [Best Practices](#best-practices)
6. [Tools and Resources](#tools-and-resources)

## Overview
This guide provides comprehensive instructions for managing images on the Revival Palace Community Church website. Proper image management is crucial for website performance, user experience, and visual consistency.

## Image Types and Requirements

### Hero Images
- **Location**: `images/hero/`
- **Dimensions**: 1920x1080 pixels
- **Format**: JPG or WebP
- **Max File Size**: 300KB
- **Usage**: Homepage and section headers
- **Requirements**:
  - High quality
  - Good contrast for text overlay
  - Church-related imagery
  - Properly lit

### Sermon Thumbnails
- **Location**: `images/sermons/`
- **Dimensions**: 800x450 pixels (16:9)
- **Format**: JPG or WebP
- **Max File Size**: 150KB
- **Usage**: Sermon listings and detail pages
- **Requirements**:
  - Clear, focused images
  - Pastor or worship-related content
  - Consistent style across all sermons

### Event Images
- **Location**: `images/events/`
- **Dimensions**: 1200x675 pixels (16:9)
- **Format**: JPG or WebP
- **Max File Size**: 200KB
- **Usage**: Event listings and detail pages
- **Requirements**:
  - Event-specific imagery
  - Good composition
  - Clear event context

### Pastor Profile Images
- **Location**: `images/pastors/`
- **Dimensions**: 400x400 pixels (1:1)
- **Format**: JPG or WebP
- **Max File Size**: 100KB
- **Usage**: Pastor profiles and team pages
- **Requirements**:
  - Professional headshots
  - Consistent style
  - Good lighting
  - Appropriate attire

### Gallery Images
- **Location**: `images/gallery/`
- **Dimensions**: 1200x800 pixels (3:2)
- **Format**: JPG or WebP
- **Max File Size**: 250KB
- **Usage**: Photo galleries and slideshows
- **Requirements**:
  - High-quality event photos
  - Church activities
  - Community events
  - Worship services

## Image Optimization

### Compression Guidelines
1. **Lossy Compression**
   - Use for photographs
   - Maintain quality while reducing size
   - Target 80-85% quality
   - Use tools like TinyPNG or ImageOptim

2. **Lossless Compression**
   - Use for graphics and logos
   - Preserve exact quality
   - Remove unnecessary metadata
   - Use tools like OptiPNG

### Format Selection
1. **JPG**
   - Use for photographs
   - Complex images with many colors
   - When transparency isn't needed

2. **PNG**
   - Use for graphics with transparency
   - Simple images with few colors
   - When exact quality is required

3. **WebP**
   - Use for all images when supported
   - Better compression than JPG/PNG
   - Maintain quality with smaller size
   - Provide fallback formats

### Responsive Images
1. **Srcset Implementation**
```html
<img src="images/sermons/sermon-small.jpg"
     srcset="images/sermons/sermon-small.jpg 400w,
             images/sermons/sermon-medium.jpg 800w,
             images/sermons/sermon-large.jpg 1200w"
     sizes="(max-width: 400px) 400px,
            (max-width: 800px) 800px,
            1200px"
     alt="Sermon Title">
```

2. **Picture Element**
```html
<picture>
    <source srcset="images/hero/hero-image.webp" type="image/webp">
    <source srcset="images/hero/hero-image.jpg" type="image/jpeg">
    <img src="images/hero/hero-image.jpg" alt="Hero Image">
</picture>
```

## File Organization

### Directory Structure
```
images/
├── hero/           # Hero section images
├── sermons/        # Sermon thumbnails
├── events/         # Event images
├── pastors/        # Pastor profile images
├── gallery/        # Photo gallery images
├── icons/          # UI icons and graphics
└── backgrounds/    # Background patterns and textures
```

### Naming Conventions
1. **General Rules**
   - Use lowercase letters
   - Use hyphens for spaces
   - Include date for time-sensitive images
   - Use descriptive names

2. **Examples**
   - `sermon-revival-2024-01.jpg`
   - `event-conference-spring-2024.jpg`
   - `pastor-john-smith-profile.jpg`
   - `gallery-youth-day-2024-02.jpg`

## Best Practices

### Image Selection
1. Choose high-quality, relevant images
2. Ensure proper permissions and licensing
3. Maintain consistent style across website
4. Use appropriate imagery for church context

### Accessibility
1. Always include alt text
2. Use descriptive file names
3. Maintain proper contrast
4. Consider color blindness

### Performance
1. Optimize all images before upload
2. Use appropriate image dimensions
3. Implement lazy loading
4. Use responsive images

### Copyright and Legal
1. Obtain proper permissions
2. Document image sources
3. Respect copyright laws
4. Maintain usage rights

## Tools and Resources

### Image Editing Tools
1. **Free Options**
   - GIMP
   - Paint.NET
   - Photopea (online)

2. **Professional**
   - Adobe Photoshop
   - Adobe Lightroom
   - Affinity Photo

### Optimization Tools
1. **Online Services**
   - TinyPNG
   - ImageOptim
   - Squoosh

2. **Desktop Applications**
   - FileOptimizer
   - ImageOptim (Mac)
   - RIOT (Windows)

### Browser Extensions
1. **Image Downloaders**
   - Image Downloader
   - Bulk Image Downloader

2. **Image Optimizers**
   - Image Optimizer
   - WebP Converter

## Support
For assistance with image management:
- Website Administrator: urumeneshaa@gmail.com
- Technical Support: urumeneshaa@gmail.com
- Graphic Designer: urumeneshaa@gmail.com
