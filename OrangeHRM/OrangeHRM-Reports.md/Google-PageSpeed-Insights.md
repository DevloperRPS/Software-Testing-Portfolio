# Google PageSpeed Insights Report

This report presents the results of the performance and quality assessment conducted on the OrangeHRM Demo application using[ **Google PageSpeed Insights**](https://pagespeed.web.dev/). 

The evaluation focuses on page performance, Core Web Vitals, accessibility, best practices, and SEO to identify potential areas for improvement.


## Objective

The objective of this assessment is to evaluate the application's overall performance and user experience, identify performance bottlenecks, and document optimization opportunities using Lighthouse-based analysis.


## Tool Overview

Google PageSpeed Insights is a web performance analysis tool developed by Google. 

It uses Lighthouse to measure page performance, Core Web Vitals, accessibility, best practices, and SEO while providing recommendations to improve the overall quality of a web application.

## Key Takeaways

- The application **failed the Core Web Vitals Assessment**.
- Multiple performance issues affecting page loading were identified.
- Large image resources contributed to slower loading times.
- Several render-blocking requests delayed the initial page rendering.
- Opportunities for improving resource loading and optimization were detected.
- The accessibility audit indicated that the accessibility tree is not properly structured, which may impact users relying on assistive technologies.
- Additional Lighthouse recommendations were provided to improve overall application performance and user experience.

## Report Screenshots

A [complete PageSpeed Insights report](https://pagespeed.web.dev/analysis/https-opensource-demo-orangehrmlive-com-web-index-php-dashboard-index/hx05v59mw4?form_factor=mobile), including performance metrics, audit results, diagnostics, and optimization opportunities, can be accessed using the report link.

### Core Vitals Web Assesment
<img width="1036" height="643" alt="core-vital-web-assesment-google-pagespeed-insights-report-for-orangehrm-web-application" src="https://github.com/user-attachments/assets/38dc7b01-91a9-49ed-94fe-530c1a5d1e82" />

### Performance Issues

<img width="1036" height="879" alt="diagonise-performance-issues-report-for-orangehrm-web-application-by-google-pagespeed-insights" src="https://github.com/user-attachments/assets/39b240fc-f3f0-4c62-84f6-872f9c71a947" />

## Recommendations

- Optimize and compress image assets to reduce loading time.
- Eliminate or defer render-blocking resources where possible.
- Improve resource loading through efficient caching and code optimization.
- Resolve accessibility issues to create a properly structured accessibility tree.
- Review Lighthouse recommendations and implement the suggested optimizations.
- Perform regular performance audits after application updates to monitor improvements.

## Conclusion

The PageSpeed Insights assessment identified several performance and accessibility improvements for the OrangeHRM application. 

Although the application remains functional, the failed Core Web Vitals assessment and the presence of render-blocking resources, image optimization opportunities, and accessibility issues indicate areas that should be addressed to enhance performance, usability, and overall user experience.
