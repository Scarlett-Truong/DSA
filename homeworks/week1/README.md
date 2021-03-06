------------------------------------
Highlights
------------------------------------
+ Verify for yourself (and be ready to explain to interviewer) if your algorithm can termniate.
+ Proactively write unit tests. Sometime interviewers will ask you to do so, sometime they will just expect you to know that (just like they expect you to discuss space/time complexity and tradeoffs without being prompted).

------------------------------------
Bugs
------------------------------------
+ Don't have to write half of page of explanation on your approach. For a 30 minutes code interview, if you need to, your solution may be too complicated.

+ Wrong observation
	First observations in an interview is very important. It is important that interviewee get the question right 5 minutes in. In our class, we will practice more of that.

+ using mid causes ArrayOutOfBound exception. mid - 1 and mid + 1 are within [0, length)
	try various edge cases for your algorithm: e.g., empty, null, size = 1
  
+ not using while(true) if you can
	because you may run into infinite loop per your comment (it is safer/ easier to control if you you something like while (start < end). Interviewer may ask, can you prove that your code does not run into infinite loop
      
+ setting array boundaries to values instead of indexes. Instead of "left = array[0], right = array[array.length-1];" should be "left = 0, right = array.length - 1;"

nit:

+ left + (right - left)/2
	mid = (left + right) / 2 is a cleaner way to compute mid. However, this calculation could overflow (example: right = MAX_INT and left = MAX_INT/2)
  
+ indentation
	java code style
