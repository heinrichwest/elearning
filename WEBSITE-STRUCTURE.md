# eLearning South Africa - Website Structure

## Overview
This eLearning website has been created based on your sitemap.xml.txt file. The site includes a homepage, main navigation pages, course category pages, and individual course pages.

## Completed Pages

### Main Pages (6 pages)
1. **index.html** - Homepage with hero slider, course categories, and key features
2. **tap-edge.html** - TAP Edge program page for individual learners
3. **tap-business.html** - TAP Business corporate training solutions
4. **why-us.html** - About page highlighting benefits and values
5. **short-courses.html** - Complete course catalog with 24+ courses listed
6. **newsletter.html** - Contact form, newsletter signup, and FAQs

### Category Pages (1 created, 2 remaining)
1. **hr-courses.html** - HR & Management courses category ✓
2. **project-management-courses.html** - TO BE CREATED
3. **computer-courses.html** - TO BE CREATED

### Individual Course Pages (1 template created, 29+ remaining)
1. **first-aid-training.html** - Complete course template with:
   - Course overview and learning outcomes
   - Detailed module breakdown
   - Prerequisites and assessment info
   - Pricing and enrollment CTA
   - Related courses section

## Remaining Pages to Create

Based on your sitemap, the following individual course pages still need to be created:

### Health & Safety Courses
- occupational-health-safety.html
- fire-fighting.html

### Computer & IT Courses
- basic-microsoft-excel.html
- advanced-microsoft-excel.html
- basic-excel-assessment.html
- advanced-microsoft-excel-assessment.html
- power-bi-course.html
- speed-typing-test-assessment.html
- solving-problems-with-data-and-probability.html

### HR & Management Courses
- emotional-intelligence.html
- leadership-skills.html
- managing-workplace-conflicts.html
- train-the-trainer.html
- assessor-conduct-outcome-based-assessments.html
- moderator-course.html

### Project Management Courses
- project-management-fundamentals.html

### Professional Development Courses
- effective-time-management.html
- stress-management.html
- personal-development-plan.html
- how-to-deal-with-depression.html
- business-communication.html
- effective-sales-masterclass.html

### Compliance Courses
- financial-intelligence-centre-act-fica.html
- paia-act-online-course.html
- cybercrime-and-business-emails.html

### Business Courses
- learn-to-start-your-own-business.html

## Website Structure

```
eLearning/
├── index.html (Homepage)
├── tap-edge.html (Individual program)
├── tap-business.html (Corporate program)
├── why-us.html (About/Benefits)
├── short-courses.html (Course catalog)
├── newsletter.html (Contact & Newsletter)
│
├── Category Pages/
│   ├── hr-courses.html ✓
│   ├── project-management-courses.html (to create)
│   └── computer-courses.html (to create)
│
└── Course Pages/
    ├── first-aid-training.html ✓ (Template)
    └── [29+ more course pages to create]
```

## Key Features Implemented

### Navigation
- Consistent main navigation across all pages
- Breadcrumbs on content pages
- Mobile-responsive hamburger menu

### Homepage
- 3-slide hero carousel with eLearning messaging
- Feature icons highlighting key benefits
- Course category showcase (3 main categories)
- "Why Choose Us" section
- Call-to-action banner
- Newsletter signup

### Course Pages Structure
Each course page includes:
- Breadcrumb navigation
- Course badge (category indicator)
- Course stats (duration, level, certificate, language)
- Detailed overview and learning outcomes
- Expandable module accordion
- Who should take this course section
- Prerequisites
- Assessment & certification info
- Sticky sidebar with pricing and enrollment CTA
- Related courses section

### Footer
- Newsletter signup form
- Quick links menu
- Social media links
- Copyright information

## Navigation Links

All pages include the following main navigation:
- Home → index.html
- TAP Edge → tap-edge.html
- TAP Business → tap-business.html
- Short Courses → short-courses.html
- Why Us → why-us.html
- Newsletter → newsletter.html

## Template Usage

The **first-aid-training.html** file serves as a template for all other course pages. To create a new course page:

1. Copy first-aid-training.html
2. Rename to match sitemap URL (e.g., leadership-skills.html)
3. Update the following:
   - Page title
   - Course badge color/category
   - Course name and description
   - Duration, level, and pricing
   - Learning outcomes
   - Module content
   - Prerequisites
   - Related courses links
4. Ensure breadcrumb links are correct
5. Update meta tags as needed

## Pricing Structure (Examples Used)

- Basic courses: R 850 - R 950
- Intermediate courses: R 1,200 - R 1,500
- Advanced courses: R 1,500 - R 1,800
- Corporate pricing: Contact for quote

## Badge Colors by Category

- **Health & Safety**: Red (`bg-danger`)
- **Computer Skills**: Blue (`bg-primary`)
- **HR & Management**: Green (`bg-success`)
- **Project Management**: Cyan (`bg-info`)
- **Professional Development**: Yellow (`bg-warning`)
- **Compliance**: Gray (`bg-secondary`)

## Next Steps

To complete the website:

1. Create remaining 2 category pages:
   - project-management-courses.html
   - computer-courses.html

2. Create remaining 29+ individual course pages using the template

3. Customize course-specific content:
   - Learning outcomes
   - Module breakdowns
   - Duration and pricing
   - Prerequisites

4. Optional enhancements:
   - Replace logo image (currently using KJ styles.jpeg)
   - Add actual course images
   - Implement form submission functionality
   - Add backend for newsletter signups
   - Configure email contact forms

## Contact Information Used

- Phone: +27 10 123 4567
- Email: info@elearning.co.za
- Social: LinkedIn, Twitter, Facebook

## Technology Stack

- HTML5
- Bootstrap 5
- Font Awesome icons
- Swiper.js (slider)
- GSAP (animations)
- Custom theme CSS

All pages are responsive and mobile-friendly.
