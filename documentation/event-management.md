# Event Management Guide

## Table of Contents
1. [Overview](#overview)
2. [Adding New Events](#adding-new-events)
3. [Event Detail Pages](#event-detail-pages)
4. [Image Guidelines](#image-guidelines)
5. [Event Categories](#event-categories)
6. [Best Practices](#best-practices)

## Overview
This guide provides instructions for managing events on the Revival Palace Community Church website. The event system consists of:
- Event listings page (`events.html`)
- Individual event detail pages (`event-detail.html`)

## Adding New Events

### Step 1: Prepare Event Content
Before adding a new event, gather the following information:
- Event title
- Event date and time
- Location
- Event description
- Event image
- Event category (e.g., Conference, Outreach, Youth & Family)
- Registration link (if applicable)
- Contact information

### Step 2: Add to Event Listings
To add a new event to the listings page (`events.html`):

1. Locate the event grid section:
```html
<div class="row">
    <!-- Event items here -->
</div>
```

2. Add a new event item using this template:
```html
<div class="col-lg-4 col-12 mb-3">
    <div class="product-thumb">
        <a href="event-detail.html">
            <img src="images/events/[image-name].jpg" class="img-fluid product-image" alt="[Event Title]">
        </a>

        <div class="product-top d-flex">
            <span class="product-alert me-auto">[Event Status]</span>
            <a href="#" class="bi-heart-fill product-icon"></a>
        </div>

        <div class="product-info d-flex">
            <div>
                <h5 class="product-title mb-0">
                    <a href="event-detail.html" class="event-title-link">[Event Title]</a>
                </h5>
                <p class="product-p">[Event Description]</p>
            </div>
            <small class="product-price text-muted ms-auto mt-auto mb-5">[Event Type]</small>
        </div>
    </div>
</div>
```

## Event Detail Pages

### Creating a New Event Detail Page
1. Create a new HTML file named `event-detail-[identifier].html`
2. Use the existing `event-detail.html` as a template
3. Update the following sections:

```html
<!-- Hero Section -->
<section class="hero-section">
    <div class="section-overlay"></div>
    <div class="container">
        <div class="row">
            <div class="col-12">
                <h1 class="text-white mb-4">[Event Title]</h1>
                <p class="text-white">[Event Description]</p>
            </div>
        </div>
    </div>
</section>

<!-- Event Content -->
<section class="event-content section-padding">
    <div class="container">
        <div class="row">
            <div class="col-lg-8 col-12">
                <!-- Event Image -->
                <div class="event-image mb-4">
                    <img src="images/events/[image-name].jpg" class="img-fluid" alt="[Event Title]">
                </div>

                <!-- Event Details -->
                <div class="event-details">
                    <h2>[Event Title]</h2>
                    <div class="event-meta mb-4">
                        <span class="event-date"><i class="bi-calendar-check me-2"></i>[Date]</span>
                        <span class="event-time ms-3"><i class="bi-clock me-2"></i>[Time]</span>
                        <span class="event-location ms-3"><i class="bi-geo-alt me-2"></i>[Location]</span>
                    </div>
                    <div class="event-description">
                        [Full Event Description]
                    </div>
                    
                    <!-- Registration Section -->
                    <div class="event-registration mt-4">
                        <a href="[Registration Link]" class="btn custom-btn">Register Now</a>
                    </div>
                </div>
            </div>

            <!-- Event Info Sidebar -->
            <div class="col-lg-4 col-12">
                <div class="event-info">
                    <h3>Event Information</h3>
                    <ul class="list-unstyled">
                        <li><i class="bi-calendar me-2"></i>Date: [Date]</li>
                        <li><i class="bi-clock me-2"></i>Time: [Time]</li>
                        <li><i class="bi-geo-alt me-2"></i>Location: [Location]</li>
                        <li><i class="bi-person me-2"></i>Contact: [Contact Person]</li>
                        <li><i class="bi-telephone me-2"></i>Phone: [Phone Number]</li>
                        <li><i class="bi-envelope me-2"></i>Email: [Email Address]</li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</section>
```

## Image Guidelines

### Event Images
- Size: 16:9 aspect ratio recommended
- Resolution: Minimum 1200x675 pixels
- Format: JPG or WebP
- Location: `images/events/` directory
- Naming: Use descriptive names (e.g., `conference-2024.jpg`)

### Image Optimization
- Compress images before uploading
- Use descriptive alt text
- Maintain consistent aspect ratios
- Ensure good lighting and quality

## Event Categories
Current event categories include:
1. Conference
   - Annual Revival Conference
   - Healing Conference
   - Leadership Conference

2. Outreach
   - Community Outreach Day
   - Mission Trips
   - Charity Events

3. Youth & Family
   - Youth Sunday
   - Family Day
   - Children's Programs

4. Regular Services
   - Sunday Services
   - Wednesday Prayer
   - Friday Home Cells

## Best Practices
1. Keep event titles clear and descriptive
2. Use consistent date and time formatting
3. Include all necessary event details
4. Optimize images before uploading
5. Update event status regularly
6. Remove past events or mark them as completed
7. Test registration links
8. Keep contact information up to date
9. Use appropriate event categories
10. Regularly backup content

## Support
For technical support or questions about managing events, contact:
- Website Administrator: [Contact Information]
- Technical Support: [Contact Information] 