**redditList.py**

class RedditList(builtins.object) Class that handles Reddit API

**Methods defined here:**

**init**(self)
 Initialize the reddit object with api token

**addCommentsToPost**(self)
 Adds comments to its respective post

**emptyCommentList**(self)
 Empty the comment list

**emptyPostList**(self)
 Empty the post list

**getComments**(self)
 Gets a list of comments for each post in postList

**getHotPosts**(self)
 Adds hot posts to postList

**getNewPosts**(self)
 Adds new posts to postList

**getNumComments**(self)
 Return number of comments

**getNumPosts**(self)
 Returns total number of posts

**getOAuthToken**(self)
 Returns OAuth token from Reddit API

**getPostList**(self)
 Returns the post list

**getTopPosts**(self)
 Adds top posts to list

**initCommentList**(self)
 Add Comments to the commentList

**initPostList**(self)
 Adds posts to postList

**postExists**(self, post_id)
 Returns true if post exists in postList

**splitPostID**(self, post_id)
 Splits post_id field from comment to return only the post id

**writeToFile**(self, filename)
 Writes redditList to a JSON file

**writeToJSON**(self)
 Returns a JSON object of redditList



Data and other attributes defined here:

**Comment** = <class 'redditList.RedditList.Comment'> Class that represents a a comment

**Post** = <class 'redditList.RedditList.Post'> Class that represents a post