# core-web-vitals


# Introduction

In today's fast-paced digital world, having a high-performing website and delivering a great user experience is vital for online success. With shorter attention spans, users expect websites to load fast, work smoothly, and provide a seamless browsing experience. To assist website owners and developers in assessing their site's performance, identifying areas for enhancement, and even boosting search engine rankings, Google has introduced Web Vitals. These metrics are specifically designed to measure and improve user experience, ensuring that websites meet users' expectations in terms of speed, responsiveness, and overall satisfaction.

# What are Web Vitals?

Web Vitals can be considered as health check-ups for websites. Similar to how doctors assess our pulse, blood pressure, and temperature to evaluate our well-being, Web Vitals evaluate the health of a website. These metrics provide valuable insights into how well a website loads, responds to user interactions, and maintains visual stability during the browsing experience.

The six parameters of Web Vitals are:

1. Largest Contentful Paint (LCP)
    
2. First Input Delay (FID)
    
3. Cumulative Layout Shift (CLS)
    
4. Total Blocking Time (TBT)
    
5. Time to First Byte (TTFB)
    
6. First Contentful Paint (FCP)
    

These metrics help measure and improve website performance and user experience.

# Why do Web Vitals matter?

Web Vitals matter because they focus on the user. By understanding and optimizing these metrics, website owners and developers can create websites that offer fast, engaging, and user-friendly experiences. Not only does this lead to happier users, but it can also positively impact search engine rankings.

# Introducing Core Web Vitals

In Web Vitals, there is a subset called Core Web Vitals. Core Web Vitals are important measurements selected by Google to reflect crucial aspects of user experience based on three aspects: loading performance, interactivity and visual stability. These metrics are:

1. **Largest Contentful Paint (LCP)** - measures *loading* performance
    
2. **First Input Delay (FID)** - measures *interactivity*
    
3. **Cumulative Layout Shift (CLS)** - measures *visual stability*
    

Now, Lets understand these metrices.

### Largest Contentful Paint (LCP)

LCP measures how long it takes for the main content of a webpage to appear on the screen. It shows how quickly users can see the important information, like images or text, when they visit a website. A fast LCP means users can see what they need without waiting too long, which keeps them engaged and prevents them from leaving the site.

**Threshold:**

The recommended threshold for a good LCP score is 2.5 seconds or faster. An LCP score between 2.5 to 4 seconds is considered needs improvement, while anything above 4 seconds is considered poor and requires immediate attention.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1685366572189/74f9a70b-09db-449a-9b9f-d50287b14531.png align="center")

### First Input Delay (FID)

FID measures how responsive a webpage is when users interact with it for the first time. It tracks the time between a user's action, such as clicking a button, and when the webpage actually responds. A low FID ensures that the website reacts quickly to user input, providing a smooth and enjoyable browsing experience without any frustrating delays.

**Threshold:**

For a good FID score, the recommended threshold is 100 milliseconds or less. An FID score between 100 to 300 milliseconds is considered needs improvement, while anything above 300 milliseconds is considered poor and requires optimization.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1685366679029/dc1549ad-12a9-43e4-80ca-0b7edd15ba88.png align="center")

**Important Note:** First Input Delay (FID) will be replaced by Interaction to Next Paint (INP) as a Core Web Vital in March 2024. INP is an improvised version of FID. Read more here: [https://web.dev/inp/](https://web.dev/inp/)

### Cumulative Layout Shift (CLS)

CLS measures the stability of a webpage's layout during its loading process. It calculates how much the elements on the page move unexpectedly, causing disruptions and potentially leading to user errors. Websites with a low CLS have a consistent layout, ensuring that users don't experience sudden shifts or accidental clicks on the wrong elements while navigating or reading content.

**Threshold:**

A good CLS score should be 0.1 or less. CLS scores between 0.1 to 0.25 indicate room for improvement, while scores above 0.25 are considered poor and should be addressed to prevent frustrating user experiences.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1685366780150/b59575d3-e871-4025-a502-bdcef3a13164.png align="center")

# Measuring and Monitoring Core Web Vitals

By utilizing various tools and methods, website owners and developers can gain valuable insights into how their site performs and identify areas for improvement. Based on measuring environments, the three most important categories of core web vitals measurement tools are:

1. Lab tools and
    
2. Field tools
    
3. Measure Core Web Vitals in JavaScript
    

### Lab tools to measure core web vitals

Performing lab measurements is like testing features in a controlled environment before they are available to users. It helps developers catch any performance issues or problems early on, so they can fix them before users experience them. This way, developers can ensure that their features work smoothly and provide a good user experience. Lab measurements are a valuable tool to make sure everything runs smoothly before releasing to users.

The following tools can be used to measure the Core Web Vitals in a lab environment:

1. [Lighthouse](https://developer.chrome.com/docs/lighthouse/overview/): It is an open-source tool provided by Google that audits and analyzes web pages for performance, accessibility, and other best practices. It provides detailed reports and metrics, including Core Web Vitals, to help developers optimize their websites.
    
2. [Chrome DevTools](https://developer.chrome.com/docs/devtools/): Chrome DevTools is a built-in developer tool in the Google Chrome browser. It offers a variety of performance analysis features, including network monitoring, JavaScript profiling, and auditing. It also provides Core Web Vitals data, allowing developers to identify and address performance issues.
    

Note: Both the tools measures LCP and CLS core web vitals. But instead of FID they measure Total Blocking TIme (TBT). The Total Blocking Time (TBT) metric measures the total amount of time between [First Contentful Paint (FCP)](https://web.dev/fcp/) and [Time to Interactive (TTI)](https://web.dev/tti/) where the main thread was blocked for long enough to prevent input responsiveness. Read more here: [https://web.dev/tbt/](https://web.dev/tbt/)

### Field tools to measure core web vitals

Field tools are used to measure Core Web Vitals in real-world conditions, directly from users' devices and browsers. These tools collect data on actual user experiences, such as page load times, interactivity, and visual stability. By analyzing data from a wide range of users, developers can gain insights into how their website or application performs across different devices, networks, and geographical locations. Field tools provide valuable information for optimizing performance and improving the overall user experience.

1. [**Chrome User Experience Report (CrUX)**](https://developer.chrome.com/docs/crux/)**:** The Chrome User Experience Report is a public dataset collected from real users using the Chrome browser. It provides valuable insights into various performance metrics, including Core Web Vitals, across different devices, locations, and connection types. By analyzing CrUX data, you can understand how your website performs for a broader audience and identify patterns or trends.
    
    Here are the core web vitals of hashnode.com displayed on the CruX dashboard.
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1685369751346/6b3d2a1f-83bb-408b-8b5a-59c8c67b63cf.png align="center")
    
2. [Google's PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/): Google's PageSpeed Insights is a widely used tool to measure Core Web Vitals and assess the overall performance of a website. It provides valuable insights into how well your website performs and offers recommendations to improve Core Web Vitals metrics.
    
    Here's how you can use PageSpeed Insights to measure Core Web Vitals:
    
    1. Visit the PageSpeed Insights website: Go to the PageSpeed Insights website by entering the following URL in your browser: [**https://developers.google.com/speed/pagespeed/insights/**](https://developers.google.com/speed/pagespeed/insights/)
        
    2. Enter your website's URL: In the provided field, enter the URL of the web page you want to analyze and click on the "Analyze" button.
        
    3. Review the performance report: PageSpeed Insights will analyze your website and provide a detailed performance report. The report includes metrics related to Core Web Vitals, such as Largest Contentful Paint (LCP), First Input Delay (FID), and Cumulative Layout Shift (CLS). It will also display scores for these metrics along with recommendations for improvement.
        
    
    Here are the core web vitals of hashnode.com.
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1685370656384/47403f50-f46e-47f8-9a46-39bdc7794219.png align="center")
    
    You can visit this [link](https://pagespeed.web.dev/analysis/https-hashnode-com/cnb1fy74jo?form_factor=mobile) to view the full report of hashnode's web vitals on PageSpeed Insights.
    
3. [Google Search Console](https://support.google.com/webmasters/answer/9205520): Google Search Console provides a Core Web Vitals report that gives you an overview of your website's performance based on real user data. It shows metrics like LCP, FID, and CLS, along with their distribution across different pages. This tool helps you identify areas where improvements are needed and track the progress of your Core Web Vitals over time. You can visit the [google search console](https://support.google.com/webmasters/answer/9205520) and add your website to get the monitored core web vitals data.
    

### Measure Core Web Vitals in JavaScript

To measure Core Web Vitals in JavaScript one can use the web-vitals library. This library provides a straightforward way to measure each metric using standard web APIs. With just a single function call, you can measure all the Core Web Vitals accurately behaving the same as all of the tools listed above. A full reference of this API can be found on Google Chrome's github repository "[web-vitals](https://github.com/GoogleChrome/web-vitals)"

```javascript
import {onCLS, onFID, onLCP} from 'web-vitals';

function sendToAnalytics(metric) {
  // Replace with whatever serialization method you prefer.
  // Note: JSON.stringify will likely include more data than you need.
  const body = JSON.stringify(metric);

  // Use `navigator.sendBeacon()` if available, falling back to `fetch()`.
  (navigator.sendBeacon && navigator.sendBeacon('/analytics', body)) ||
    fetch('/analytics', {body, method: 'POST', keepalive: true});
}

onCLS(sendToAnalytics);
onFID(sendToAnalytics);
onLCP(sendToAnalytics);
```

After integrating the web-vitals library to measure and send Core Web Vitals data to your analytics endpoint, the subsequent step is to aggregate and analyze the data. By assessing the data, you can determine if your web pages meet the recommended thresholds for at least 75% of page visits. This analysis allows you to gain insights into the performance of your website and identify areas that may require optimization or improvement.

### Web Vitals Chrome Extension

You can effortlessly assess and report on each of the Core Web Vitals by utilizing the [Web Vitals Chrome Extension](https://chrome.google.com/webstore/detail/web-vitals/ahfhijdlegdabablpippeagghigmibma?hl=en), eliminating the need for coding. This extension leverages the web-vitals library to measure the metrics and presents them to users while they navigate the web. Whether it's evaluating your own websites, analyzing competitors' sites, or understanding the overall web performance, this extension proves to be a valuable tool.

# Benefits of Good Web Vitals

Optimizing Web Vitals has significant advantages for user experience and business outcomes. In this section, we will explore the positive impacts of good Web Vitals, including improved user engagement, higher search rankings, increased conversions, lower bounce rates, and enhanced user satisfaction.

**Enhanced User Experience and Engagement:**

Good Web Vitals provide a seamless and enjoyable user experience, with faster loading times, responsive interactions, and visual stability. This leads to increased engagement and keeps users on your website for longer periods.

**Higher Search Rankings:**

Websites with good Web Vitals may receive higher search rankings as search engines prioritize delivering a quality user experience. Optimizing Web Vitals is an essential part of SEO strategies.

**Increased Conversions, Lower Bounce Rates, and Improved User Satisfaction:**

Good Web Vitals contribute to higher conversion rates, lower bounce rates, and improved user satisfaction. Users are more likely to convert, stay on your site, and have a positive perception of your brand when the website is optimized for a smooth user experience.

# Summary

In this article, we have delved into the world of Web Vitals and their significance for website owners and developers. We explored the concept of Web Vitals, highlighted the specific metrics of Core Web Vitals, discussed their impact on user experience and SEO, and examined the benefits of optimizing website performance. As we conclude, let's recap the importance of Web Vitals and encourage readers to prioritize their website's performance using Core Web Vitals.

1. **The Importance of Web Vitals for Website Owners and Developers:**
    

Web Vitals provide crucial insights into how users perceive and interact with your website. By measuring key performance metrics, such as loading times, responsiveness, and visual stability, you gain a deeper understanding of user experience. This understanding enables you to identify areas for improvement and optimize your website accordingly, resulting in enhanced user engagement, increased conversions, improved search rankings, and overall customer satisfaction.

1. **Prioritizing Optimization with Core Web Vitals:**
    

With the introduction of Core Web Vitals as a subset of Web Vitals, Google has emphasized the significance of these specific metrics for website performance and user experience. As a website owner or developer, it is essential to prioritize optimizing your website using Core Web Vitals as a guide. By focusing on metrics like Largest Contentful Paint (LCP), First Input Delay (FID), and Cumulative Layout Shift (CLS), you can make tangible improvements that have a direct impact on user satisfaction and business success.

1. **Further Learning and Exploration:**
    

To continue your journey into the world of Web Vitals and website optimization, here are some additional resources you can explore:

* **Google's Web Vitals documentation**: The official documentation by Google provides in-depth information about Web Vitals, Core Web Vitals, and how to measure and improve website performance.
    
* **Google Search Console and PageSpeed Insights**: These tools offered by Google allow you to monitor your website's Core Web Vitals, receive performance reports, and gain insights into areas that need optimization.
    
* **Online communities and forums**: Engage with other website owners and developers in online communities and forums to exchange knowledge, best practices, and tips for optimizing Web Vitals.
    
* **Performance optimization guides:** Numerous online guides and tutorials are available that offer practical advice and techniques for improving website performance and meeting Core Web Vitals requirements.
    

# **Connect with me**

[**Twitter**](https://twitter.com/risesumit) [**Github**](https://github.com/SumitKcs) [**Linkedin**](https://www.linkedin.com/in/sumitssr/)
