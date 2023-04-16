# arc
Auto Cloud - Salesforce Actionable Relation Center


The Salesforce Actionable Relation Center (ARC) in Auto Cloud is a feature that enables users to view and act on related records within a single card. This feature is designed to improve the user experience and increase productivity by providing easy access to information and actions related to a particular record.

For example, suppose a user is viewing a customer account record in Salesforce Auto Cloud. The Actionable Relation Card will display documents such as the customer's contact information, previous orders, and support cases. The user can then take action directly from the card, such as creating a new support case or viewing details of a previous order.

This feature is handy for Sales/Service teams who need to access customer information quickly and efficiently. It improves efficiency by providing a centralized view of all relevant information.

Overall, the Salesforce Actionable Relation Card in Auto Cloud is a powerful tool that can help organizations to increase efficiency and productivity by providing easy access to related records and actions within a single card. Refer to the below URL trailhead URL



https://play.vidyard.com/426REjmHvrcsV2L2eQ5vW7?
Let's learn Auto Cloud ARC with a use case. 

Use Case: 

Universal Container(UC) is an Auto Manufacturing company that wants to show all the related Accounts and Contacts related to the Vehicle on the Vehicle detailed page for their service Advisors. The advisors should be able to create cases and manage users from the ARC layout. The Vehicle can have the following stakeholders. 

Current Owner
Previous Owner
Primary Driver
Secondary Driver
Referral Account Details
Selling Dealer
Servicing Dealer
Note: UC wants to deliver the above feature out of the box(OOTB).



Solution: 

We will use Salesforce Auto Cloud OOTB objects to implement the features. 

Use Assets and Vehicles to manage the current ownership.
Use Asset Account Participation object to showcase Previous Owner and Dealership details. 
Use Asset Contact Participation object to house Driver details. 
Use the Account Contact Relation object to capture the referral details. 
We can create a record type or Use the Salesforce OOTB Account Type field to segregate different customer types. In my example, I made two record types, Household and Dealer.
Note: I tried to make this example simple and tried to implement 100% OOTB configuration. 

Please check the video below to create an ARC according to the Use Case. 

https://www.youtube.com/watch?v=PoMPOGvctzs&ab_channel=SalesforceOutOfTheBox

Notes:

When you want to derive a relation from Child to Parent, you need to use Junction Object. 
Please add "ARC Access" permission on the user profile to use ARC. 
To use Vehicle and Asset Account and Asset Contact objects, Please ensure to add the "Automotive Foundation User" Permission set.
