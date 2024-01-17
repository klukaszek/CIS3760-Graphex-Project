**GitLab**
- Worked on a bit of our Sprint 5 Wiki checklist.

**Front-end**
- Added a tab that displays our database sentiment analysis bar graph. [Data Vis Components](https://gitlab.socs.uoguelph.ca/3760W23/t1/graphex/ubi/-/tree/main/frontend/src/routes/home/Components)
- Refactored our front-end components so that most could be used from anywhere in our project structure. [Components](https://gitlab.socs.uoguelph.ca/3760W23/t1/graphex/ubi/-/tree/main/frontend/src/Components)
- Designed a tab switch component to swap between data visualizations, and also to swap between our Twitter and Reddit Post datasets under the "All Posts" tab. [switch.svelte](https://gitlab.socs.uoguelph.ca/3760W23/t1/graphex/ubi/-/blob/main/frontend/src/Components/switch.svelte)

**Backend**
- Fought with Kubernetes to try and get the backend container to work on our staging site to finally work.
- Wrote a bash script to run our Flask backend and also update our database at an interval of 120 minutes with the help of Python scripts from Logan and Jonalton. [initBackend.sh](https://gitlab.socs.uoguelph.ca/3760W23/t1/graphex/ubi/-/blob/main/backend/initBackend.sh) 
- Optimized our endpoint communication by compressing all data being sent from the back end using gzip compression. [posts.py](https://gitlab.socs.uoguelph.ca/3760W23/t1/graphex/ubi/-/blob/main/backend/src/api/posts.py) [plot.py](https://gitlab.socs.uoguelph.ca/3760W23/t1/graphex/ubi/-/blob/main/backend/src/api/plot.py)
- Implemented the double bar graphs for sentiment analysis across the entire database of posts. [plot.py](https://gitlab.socs.uoguelph.ca/3760W23/t1/graphex/ubi/-/blob/main/backend/src/api/plot.py) [graphPlotter.py](https://gitlab.socs.uoguelph.ca/3760W23/t1/graphex/ubi/-/blob/main/backend/src/lib/graphPlotter.py)