# Sermon Creation and Management Guide

## Table of Contents
1. [Overview](#overview)
2. [Adding New Sermons](#adding-new-sermons)
3. [Sermon Detail Pages](#sermon-detail-pages)
4. [Image Guidelines](#image-guidelines)
5. [Search Functionality](#search-functionality)
6. [Load More Feature](#load-more-feature)

## Overview
This guide provides detailed instructions for managing sermons on the Revival Palace Community Church website. The sermon system consists of two main components:
- Sermon listings page (`sermons.html`)
- Individual sermon detail pages (`sermon-detail.html`)

## Adding New Sermons

### Step 1: Prepare Sermon Content
Before adding a new sermon, gather the following information:
- Sermon title
- Pastor's name
- Sermon date
- Duration
- Description (brief summary)
- Full sermon content
- Sermon image
- Video URL (if available)

### Step 2: Add to Sermon Listings
To add a new sermon to the listings page (`sermons.html`):

1. Locate the sermon grid section:
```html
<div class="row" id="sermonGrid">
    <!-- Sermon items here -->
</div>
```

2. Add a new sermon item using this template:
```html
<div class="col-lg-4 col-md-6 col-12 mb-4 sermon-item">
    <div class="sermon-thumb">
        <a href="sermon-detail.html">
            <img src="images/pastors/[image-name].jpg" class="img-fluid sermon-image" alt="[Sermon Title]">
        </a>

        <div class="sermon-info">
            <div class="sermon-date mb-2">
                <i class="bi-calendar-check me-2"></i>Uploaded on [Date]
            </div>
            <h5 class="sermon-title mb-2">
                <a href="sermon-detail.html">[Sermon Title]</a>
            </h5>
            <p class="sermon-pastor">[Pastor Name]</p>
            <p class="sermon-description">[Brief Description]</p>
            <div class="sermon-meta">
                <span class="sermon-duration"><i class="bi-clock me-2"></i>[Duration] min</span>
            </div>
        </div>
    </div>
</div>
```

3. For new sermons that should be hidden initially (using the "Load More" feature), add the `hidden-sermon` class:
```html
<div class="col-lg-4 col-md-6 col-12 mb-4 sermon-item hidden-sermon">
    <!-- Same content as above -->
</div>
```

## Sermon Detail Pages

### Creating a New Sermon Detail Page
1. Create a new HTML file named `sermon-detail-[identifier].html` (e.g., `sermon-detail-faith-purpose.html`)
2. Use the existing `sermon-detail.html` as a template
3. Update the following sections:

```html
<!-- Hero Section -->
<section class="hero-section">
    <div class="section-overlay"></div>
    <div class="container">
        <div class="row">
            <div class="col-12">
                <h1 class="text-white mb-4">[Sermon Title]</h1>
                <p class="text-white">[Brief Description]</p>
            </div>
        </div>
    </div>
</section>

<!-- Sermon Content -->
<section class="sermon-content section-padding">
    <div class="container">
        <div class="row">
            <div class="col-lg-8 col-12">
                <!-- Video Section -->
                <div class="sermon-video mb-4">
                    <div class="ratio ratio-16x9">
                        <iframe src="[Video URL]" allowfullscreen></iframe>
                    </div>
                </div>

                <!-- Sermon Details -->
                <div class="sermon-details">
                    <h2>[Sermon Title]</h2>
                    <div class="sermon-meta mb-4">
                        <span class="sermon-date"><i class="bi-calendar-check me-2"></i>[Date]</span>
                        <span class="sermon-duration ms-3"><i class="bi-clock me-2"></i>[Duration] min</span>
                    </div>
                    <div class="sermon-description">
                        [Full Sermon Content]
                    </div>
                </div>
            </div>

            <!-- Pastor Info Sidebar -->
            <div class="col-lg-4 col-12">
                <div class="pastor-info">
                    <img src="images/pastors/[pastor-image].jpg" class="img-fluid pastor-image" alt="[Pastor Name]">
                    <h3>[Pastor Name]</h3>
                    <p>[Pastor Title/Role]</p>
                </div>
            </div>
        </div>
    </div>
</section>
```

4. Update the navigation links in the new file to point to the correct sermon detail page

## Image Guidelines

### Sermon Thumbnails
- Size: 16:9 aspect ratio recommended
- Resolution: Minimum 800x450 pixels
- Format: JPG or WebP
- Location: `images/pastors/` directory
- Naming: Use descriptive names (e.g., `sermon-faith-purpose.jpg`)

### Pastor Images
- Size: Square format recommended (1:1 aspect ratio)
- Resolution: Minimum 400x400 pixels
- Format: JPG or WebP
- Location: `images/pastors/` directory
- Naming: Use pastor's name (e.g., `pastor-john-doe.jpg`)

## Search Functionality
The search feature automatically indexes:
- Sermon titles
- Pastor names
- Sermon descriptions

No additional configuration needed. The search works across all sermons, including hidden ones.

## Load More Feature
- Initially shows 3 sermons
- Clicking "Load More" reveals 3 more sermons
- New sermons should be added with the `hidden-sermon` class
- The button automatically hides when all sermons are displayed

### Adding Hidden Sermons
1. Add new sermon items with the `hidden-sermon` class
2. Place them after the visible sermons
3. The load more functionality will automatically handle them

Example:
```html
<div class="col-lg-4 col-md-6 col-12 mb-4 sermon-item hidden-sermon">
    <!-- Sermon content -->
</div>
```

## Best Practices
1. Keep sermon titles clear and descriptive
2. Use consistent formatting for dates
3. Optimize images before uploading
4. Maintain consistent sermon durations
5. Write clear, concise descriptions
6. Update sermon listings in chronological order
7. Test new pages across different devices
8. Ensure all links work correctly
9. Keep file names consistent and descriptive
10. Regularly backup content before making changes

## Support
For technical support or questions about managing sermons, contact:
- Website Administrator: urumeneshaa@gmail.com
- Technical Support: urumeneshaa@gmail.com
