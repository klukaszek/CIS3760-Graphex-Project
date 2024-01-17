### Role: Developer

### Project Configuration
- Changed the backend Docker image to a Debian flavor image so that NumPy and Pandas wheels could install correctly via PIP. This was caused by Alpine not having a complete C toolchain which resulted in broken package installations.
- Configured vite.config.ts to use jest-dom so that we can test our components based on the page DOM.
- Spent too long trying to get the right Plotly package to work with the @types distribution of Plotly. The package was eventually recognized and worked properly.

### Backend Programming
- Set up sentiment analysis for posts in the backend using NLTK
- Using the sentiment analysis data, I created data frames with Pandas to create plots using Plotly.
- Created plots in the backend with Plotly and converted the data and layout into JSON data so that it could be passed to the front end via an API call.
- Refactored the data that is passed to the front end when we make an API call for a random post.
- Wrote tests for sentiment analysis, and plot generation.

### Frontend Programming
- Created a Svelte component to display a post with its content and date.
- Created a Svelte component to display a Plotly plot no matter what data is passed to it.
- Re-engineered the method of acquiring a random post and the sentiment analysis plot by using Svelte stores to share memory between the page and its components. Any update to the store is instantly reflected on the page.
- Wrote tests to make sure the components are working.