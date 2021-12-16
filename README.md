# DEP-training

## DOM Task

Task: Create web-application for load and search info about YouTube videos using user's request.

Use-case:

1. User opens the application and see search input
2. User types the topic inside of search input. For example javascript
3. Application makes call to YouTube REST API and shows results as thumbnails in horizontal list
4. List is scrolled through click on the page. Video count on the page depends on screen size.
5. Load 15 records, the rest if the records that doesn't in the screen will go into pagination. The page numbers will be below the thumbnails.

Requirements:

1. Chrome support and one mobile platform
2. HTML creates using JS. Required code inside index.html.
3. No jquery or other frameworks. You can use only lodash.
4. JS code should be splitted to different files depending on architecture.
5. Minimal info about video is title with link on youtube, preview, description, author, published date, count of views.
6. Data from youtube could be received using:

- https://www.googleapis.com/youtube/v3/search?key=[YOUR_API_KEY]&type=video&part=snippet&maxResults=15&q=[SEARCH_STRING]
- https://www.googleapis.com/youtube/v3/videos?key=[YOUR_API_KEY]&id=[VIDEO_IDS]&part=snippet,statistics
- how too receive API key - https://www.youtube.com/watch?v=[VIDEO_ID]
- full documentation - https://developers.google.com/youtube/v3/

7. Design should be not ugly
