## Stage 1

## Problem 

- The campus notification app has been running from few weeks. The feedback is recieved from users that the important notifcations get missed due to high volume of notification.


- A Priority inbox is required that will always disply the top 'n' important unread notifications first.
- Priority should be determined on the basis of the the weight i.e. (placement > result > event) and recency.

## Priority Inbox Logic

- Priority is determined by: 
  
- weight 
- recency

Formula: 

score = (weight * 1000000) + recency

# Data structure:

- MinHeap of size N
- Fast retrieval and insertion 
- Handles conitnuous upcoming notification.
- Maintain top N notification.
  
# Complexity:

- Insertion (Time Complexity) : O(logN)
- Retrieval (Time Complexity) : O(NlogN)

- space complexity: O(N)
  
# Scalability: 

- compute score to find the priority notification.
- compares with heap mininum
- Replace if high priority.

- Calculates the score of the email notification and keep the priortised notification in priorty inbox. Hence, avoids the storing of all the notification in memory.



