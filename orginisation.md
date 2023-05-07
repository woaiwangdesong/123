Shuyuan Liu(sliu383, git id: 109999523) - performer.java, seat.java

Lei Zhang(lzha760, git id: 110000068) - user.java, ConcertMapperConvert.java, the changing in client and common folder

Yucheng Mu(ymou783, git id: 72597119) - booking.java, concert.java

ConcertResource.java is written by the three of us when we have an offline meeting and make () upload it.


In the process of writing, when we meet problems, we will first discuss them in a group online. If there is no consensus, we will meet offline and write together.

Our concurrency model uses a pessimistic locking strategy, which is implemented in the file "concertresource". The concept of pessimistic locking is that it assumes other users will be simultaneously modifying data. Therefore, when operating on data, the data is locked directly until the operation is completed, and the lock is released; during the locking period, others cannot modify the data. Which is reflected in the "makeBooking" function. Specifically, it is achieved by setting the lock mode to PESSIMISTIC_WRITE, locking the seat data as unavailable, and preventing other users from booking the same seats during this period. We believe that concurrency conflicts may frequently occur in this method, so before reading or modifying shared resources, we need to lock the resources first to prevent other threads from accessing and modifying them simultaneously, which can avoid concurrency problems.


Our model uses JPA mapping and is based on anemic domain models. We use anemic domain models to represent our entity classes. For the current business logic, using this approach feels very natural, and it is quick to develop and easy to understand. After discussing, we also believe that this approach is more suitable for this assignment.


Our domain model is negotiated offline and written and uploaded by one person, and  most of our work is done offline together, and what we discuss online is the final piece that is not completed offline.


The group work went very well, everyone did their part well and was very active in communicating with each other when they encountered problems, and they were on time to participate in offline writing and online discussions together. we could see that everyone was very responsible for this assignment. I hope we can get a high score, I think we did a very good job. cheers all team members.
​​



