

PROJECT ASSIGNMENT

DATABASE:
	USERS (uid, first name, last name, email , dob, hometown , gender , password)
	
	FRIENDS (uid , uid)

	ALBUMS(aid, name, uid, doc)

	PHOTOS(pid, aid, caption, data)

	TAGS(hashtag)

	TAGGED (pid, hashtag)

	LIKE (uid, pid,doc)

	COMMENTS(cid, content, uid,pid, doc)



需求
	Users：
		REGISTER	非注册用户不能上传图片； 
					fname\lname\email\dob\password    required
					email unique
		FRIENDS		ADD A NEW FRIEND FROM FRIEND LIST
					LIST FRIENDS
					SEARCH FRIENDS
		USER ACTIVITY	
					list top 10 users with the largest contribution on the website. contribution=number of photos uploaded + number of comments left for others' photos

		LOGOUT 

	Album and photo:
		BROWSING	browse photos (visitors/registered users)
		CREATE
		DELETE
	
	TAG:
		VIEWING YOUR PHOTOS BY TAG 			PRESENT TAGS AS HYPERLINKS
		VIEWING ALL PHOTOS BY TAG 		add switch VIEW ALL PHOTOS/VIEW MY PHOTOS 
		PHOTO SEARCH						visitors/registered users
											could be conjunctive queries 'AND'

	COMMENTS:
		LEAVE comments 						visitors/registered users
											cannot comment on their own photos
		LIKE  					  show  the number of likes/ users liked this photo

		SEARCH
								specify a text query (one or more words) and the system should find the users that have created comments  that exactly match the query text. The system should return these users ordered by the number of comments that match the query for each such user in descending order. 

	RECOMMENDATIONS:
		FRIENDS					RECOMMEND POSSIBLE NEW FRIENDS
		YOU-MAY-ALSO-LIKE			
								Take the five most commonly used tags among the user's photos. Perform a disjunctive search through all the photos for these five tags. A photo that contains all five tags should be ranked higher than one that contained four of the tags and so on. Between two photos that contain the same number of matched tags prefer the one that is more concise, i.e., the one that has fewer tags over all. 



PAGES:
	LOGIN
	REGISTER
	PROFILE (INFORMATION    FRIENDS   RECOMMEND FRIENDS)

	HOMEPAGE (SEARCH TAG/COMMENTS/PEOPLE) (TOP 10 USERS)(RECOMMEND PHOTOS)
	PHOTO PAGE (INFORMATION  COMMENT LIKE DELETE)
	UPLOAD


EXTENSION FUNCTION:
	EXPLORE
	FORGET PASSWORD
	RECOMMEND SEARCHING
	PIN FUNCTION


























































