QAShares will have a marketplace for users to ask questions and receive expert answers. This will marketplace will work according to the following logic: -

1.	A user, herein known as the questioner, puts forward a question and assigns a value in QAS and a timeframe.

2.	Other users, herein known as the answerers, can then answer the question to the best of their knowledge.

3.	At the end of the timeframe, if there are no answers then the questioners QAS are refunded.

4.	If there are answers: -

a.	By default, the QAS is split between answers according to their reputation

b.	The questioner has <DefaultMinsToAllocate> minutes to modify the allocation. They can also choose to retain some QAS - which will trigger a review by one reviewer. They can also opt to pay <StandardReviewQAS> for each additional reviewer (up to a maximum of <MaxReviewers>). This is paid into the user fund.

c.	 If the questioner fails to allocate QAS then a review with three reviewers is triggered and the questioner’s reputation is decreased by <NonAllocationRepPercentageDecrease>%.

d. 	Following this the answerers have <DefaultMinsRequestReview> minutes to request a review and specify the amount they believe they should be given and the number of reviewers they would like to review (up to a maximum of <MaxReviewers>). They must then pay <StandardReviewQAS> * (Reviewers-1) QAS back into the user fund.

e.	If there is no review then QAS is allocated as per the average of the user allocation and the reputation split.

f. 	If review is in action then the maximum of the number of reviewers, requested by the questioner or answerers, is allocated to review the question and answers. Reviewers will come from the top 10% of users by reputation and must not have reviewed the same questioner’s questions or answerers answers in the last <NoOfDaysSincePrevReview> days. They look at the questions and answers and independently assign what they think is a correct allocation of the QAS – including whether any QAS should be retained. The average (mean) of the reviewers’ allocations together with questioner’s allocations (As long as she allocated) are calculated and this forms the new allocation. 

g. 	In the event of a review panel of three or more, and one reviewer being out of line with their fellow reviewers, then another reviewer will be called in to provide a further review. If the replacement reviewer is well aligned to the other reviewers, then they replace the out of sync reviewer. If the replacement reviewer is also not well aligned with the other reviewers, then the whole review process is annulled and restarted.

h.	Once the review is complete the QAS is allocated through a combination of questioner allocation and reviewer allocations. If a pay-out to an answerer is smaller than <MinPayoutPercentage>% then the questioner is returned that value and the answerer does not receive any payout.

i. 	Reviewers receive QAS from the user fund.

j.	Questioner allocations and reviewers decisions also affect questioner and answerer reputations. This will use an ELOi adjustment formula of ((expected amount based on percentage of total answerer reputation) – (Percentage of actual amount allocated))/10. 

5.	On a random basis, reviewers’ decisions are assessed by other reviewers who can vote on their performance. This will also act as a reputation adjustment. 
