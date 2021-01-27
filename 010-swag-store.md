# Swag store <!-- What do you want to call your `awesome_feature`? -->

- Implementation Owner: @Glide7
- Start Date: 26-01-2021
- Target Date: Unknown
- Appwrite Issue: None
  

## Summary

[summary]: #summary

Developer (and everyone) love swag. Appwrite is a kick-ass company, so we should have swag! In order for us to be able to continue to work on Appwrite, and still have the ability to provide swag, we should use a service ( such as Printful, Shopify) that makes swag on demand. Swag refers to anything Appwrite branded, such as shirts, hoodies, stickers, mugs and etc'. 

## Problem Statement (Step 1)

[problem-statement]: #problem-statement

**What problem are you trying to solve?**

At the current time, we do not have any scalable or easy way to produce swag both for us or the community. from my (little) expeirnce, dealing with ordering, sizes, printing, getting addresses and shipping - I've seen that it is complicated and cumbersome to do.

**What is the context or background in which this problem exists?**

Right now, when we have a hackathon or we want to be able to send swag to community members, it puts a toll on our time and efforts to send swag or even sell swag.

**Once the proposal is implemented, how will the system change?**

Once the proposal is implemented, community members and Appwrite will be able to buy swag off a dedicated service, on demand, per specific request (color, size, type)

<!-- Please avoid discussing your proposed solution. -->

## Design proposal (Step 2)

[design-proposal]: #design-proposal

<!--
This is the technical portion of the RFC. Explain the design in sufficient detail keeping in mind the following:

- Its interaction with other parts of the system is clear
- It is reasonably clear how the contribution would be implemented
- Dependencies on libraries, tools, projects or work that isn't yet complete
- New API routes that need to be created or modifications to the existing routes (if needed)
- Any breaking changes and ways in which we can ensure backward compatibility.
- Use Cases
- Goals
- Deliverables
- Changes to documentation
- Ways to scale the solution

Ensure that you include examples, code-snippets etc. to allow the community to understand the proposed solution. **It would be best if the examples use naming conventions that you intend to use during the actual implementation so that changes can be suggested early on during the development.**

Write your answer below.

-->


[prior-art]: #prior-art


### Setting up an online store
We will use Shoify for setting up the store, and use Printful as the platform that actually prints and ships the swag. These store intergrate together (stated later in this RFC) easily, and via the websites themselfes.

## Shopify
I have created a Shopify account (free 14-day trial, after that we need to pay 29$USD per month for the basic package, which is enough for us). The basic program allows for 2 Staff accounts, so 1 more person can have acces to it.

## Prinful
I have created a Prinftul account (free registration) using my Appwrite email account.

## Connectiong Shopiy + Printful
I have connected the Shopify store to the Prinful account. Entire guide that shows how to do it, is [here](https://www.youtube.com/watch?v=wqZgouaDjck).

## Designs + Products
As discussed with Eldad, we would help get help with design for the swag (which Eldad and I will create a list and publish towards the release of this RFC. Printful provides a variety of swag (from T-shirts to mugs to face masks and my personal favorite, flip flops 😅) 
After the design help has provided us with designs that we can use, I will add them to the Printful products.

## Shipping
Luckily for us, Prinful provides [automatic shipping](https://www.printful.com/shipping). All we need to do is set it up (As stated in the video above)

## Online store
We need to design our online store ([appwritetest.myshopify.com](appwritetest.myshopify.com) as of right now, but we can create a custom domain). It needs to be alligned with the Appwrite brand guidelines.

## Payment
We simply need to add a payment method 🙃

## QA
I think it would be neccesary for us to test the whole proccesss once we've set everything above. We should make sure the experience is working as best we can, meaning people (and us) can easily buy Appwrite swag.


### Unresolved questions

[unresolved-questions]: #unresolved-questions

<!-- What parts of the design do you expect to resolve through the RFC process before this gets merged? -->

<!-- Write your answer below. -->
None so far!

### Future possibilities

[future-possibilities]: #future-possibilities

<!-- This is also a good place to "dump ideas", if they are out of scope for the RFC you are writing but otherwise related. -->

<!-- Write your answer below. -->
## Reward system
In the futrure, we can possibly create a reward system for Appwrite contributors, that will reward them with currency or credit to use in the swag store. They can achieve that by contributing to the project 🏆
