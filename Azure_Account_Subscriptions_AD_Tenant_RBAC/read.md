Back in the day when I started learning Azure, I used to get confused about different components and services in Azure (well..it's not like I am an expert right now!). Of all the topics, the most difficult one to grasp in Azure was around Azure accounts, subscriptions, active directory, tenant and role based access control since you don't get to play around with these. But with time I got the opportunity to work with them and learn more. Most of the articles around these topics take a real life example and compare it with the actual situation in Azure. So I will also use the same method and try to describe about these topics.

Let's begin....

- [Azure Account](#heading)
- [Azure Subscription](#heading)
- [Azure Active Directory and Tenant](#heading)
<!-- toc -->
## Azure Account
An account in Azure is like any other account which you create.... like in Gmail, Facebook, etc. Once an account is created you can start using the product. Similarly in Azure, you sign up and create an account. But to start using Azure just creating an account won't do any good. Consider renting a house, you can relate to creation of an account to just registering your name so that you can start living in the house. But to live in a house you need to pay RENT!!! Same is the case in azure.... Just by creating an account, Microsoft doesn't allow you to start using the services in Azure. You need to pay some rent to Microsoft........ which brings us to creating/buying an Azure subscription.

## Azure Subscription
Once an account is created in azure, Microsoft offers different plans with which you create a Subscription. Even if you don't want to create a subscription, a 7-days free trial is offered to you after which you can decide whether you want to buy the subscription or not. An Azure subscription comes with its own terms and conditions. For different types of subscriptions, the conditions vary. Comparing it with our example of renting a house, the Owner of the house has different types of rental agreements. By choosing one of the rental agreements, you can start living in the house.

Just like with the same Owner, you can enter into multiple agreements for different houses.... with Azure, you can do the same. For the same Azure account you can create multiple subscriptions. By why will you do such a thing??? Well... it depends on what you want to use the house for. You might use a subscription for a particular thing and another for another thing. The point is, Microsoft doesn't restrict you to be limited to only one subscription. You can have multiple subscriptions belonging to a single Azure Account.

## Azure Active Directory and Tenant
Consider a situation where you want someone else to access your house. You might share a duplicate of your own key of the house to that person. What happens when you want one more person to access your house? You create one more copy of your key and share it. This is all fine when there are less number of people but as more and more people are allowed access to the house the sharing of keys becomes a tedious task. 

Similarly in case of Azure, if access to an Azure subscription is required by multiple people, you can't keep sharing your account credentials with them. Because once an account credential is shared, you loose the ablity to uniquely identify the operations performed by others. This can lead to situations of undesired modifications to resources in your Subscription and since the same credential is being used there will be no way of keeping track of who performed which operations because all operations will be registered to performed under YOUR NAME!!!

To prevent such scenarios, Microsoft has a cloud offering of Active directory which is Azure Active Directory(AAD). Relating this to our example of house, you acquire a machine which can identify different people to whom you want to give the access of your house installed on the front door and open the door.  