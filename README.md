1) Where would you fit your automated tests in your Recipe project development pipeline? Select one of the following and explain why.  
Option 1. Within a Github action that runs whenever code is pushed. It catches bugs before they reach main, runs automatically, and doesn't rely on developers remembering to test.

2) Would you use an end to end test to check if a function is returning the correct output?  
No. E2E tests simulate user workflows. Unit tests are for checking function return values.

3) What is the difference between navigation and snapshot mode?  
Navigation mode analyzes a page as it loads from start to finish (measures load performance, timing metrics, and resource fetching). Snapshot mode analyzes the page in its current state at a single point in time without reloading. It can find accessibility and best practice issues but cannot measure loading performance or JavaScript execution timing.

4) Name three things we could do to improve the CSE 110 shop site based on the Lighthouse results.  
Based on the Lighthouse results, here are the 3 things I would improve: 
First, the CSS file (main.css) is blocking the page from rendering right away, so it could be loaded in a way that doesn't hold up the rest of the page. 
Second, the site's static files like images, scripts, and stylesheets have short cache lifetimes (only 10 minutes), so setting longer cache times would help the page load faster for returning visitors. 
Third, the site has a long chain of files that depend on each other to load (the HTML loads storage.js, which then loads product-item.js, then main.js), so reducing this chain or preloading some of these files would help the page load quicker overall





