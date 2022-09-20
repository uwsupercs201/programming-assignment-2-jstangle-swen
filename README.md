# Programming Assignment 2

## Goal: 
- Learn to use conditional statements to control execution of tasks.

You work at a movie theater. They have a VERY complex pricing system, which for many of the ticket-sellers is too difficult to navigate. So, you've been tasked with writing a program that will generate the price of a patron's ticket based on 5 inputs:

- The day of the week
- The patrons age
- Whether the movie is action, comedy, or drama
- Location in the theater: front, middle, back
- If it is "happy hour" or not: 1-3pm

The pricing strategy is:

Base Price by day:

| Monday-Thursday | Friday | Saturday | Sunday |
|-----------------|--------|----------|--------|
| $10 | $12 | $14 | $13 |

By age:
- Seniors (65+) get a $2 discount every day except for Saturday
- Kids (0-12) get in free.

By move genre:
- Action has a $1 extra fee on every day except Friday.
- Comedy has no extra fee
- Drama is $2 LESS on Monday-Thursday

By Location:
- Front of theater is $2 more for Children or regular patrons (no extra charge for seniors)
- Middle is no extra charge for anyone
- Rear is $2 less, but not allowed at all for children (since they get rowdy). 

By Happy Hour:
- If it is happy hour, tickets are discounted by 50% of their final price after all other adjustments.

For example, a senior going to the movies on Wednesday for an action film at 2pm and wanting to sit in the middle will cost: $4.50

**BUT, there's more!**

Each customer gets to wager to get a free ticket. At the beginning of your program, generate a random integer from 4-40 (inclusive) and call it the magic number. The user can choose to wager as follows:

- They choose 4 numbers from 1-10 (inclusive)
- If those 4 numbers sum to the magic number, they get their ticket free. 
- If not, they pay DOUBLE of their ticket price!


### Your Assignment:

Write a Java program called `TicketPricer.java` which asks the user for the 5 variables which control price: 
- The day of the week
- The patrons age
- Whether the movie is action, comedy, or drama
- Location in the theater: front, middle, back
- If it is "happy hour" or not: 1-3pm

Based on that information, it should determine the price of their ticket. Then, it should allow them to choose whether they want to wager for a free ticket or double-price ticket.

Example:

```
What day is it? Monday
What is your age? 35
Is the movie action, comedy or drama? Comedy
Where would you like to sit (front, middle, rear)? Front
What time is the movie? 5pm

Your price is $12, would you like to wager for a free ticket? Yes.

Choose 4 integers from 1-10:
Number 1: 5
Number 2: 9
Number 3: 8
Number 4: 7

That adds to 29, which is not the magic number. Your total is $24.
```

## Submitting the Assignment

When you're done, you can upload your files to this Repo and commit the changes.

Click Add files at the top right of the Repo page.

There are two options:

A) Click "Add Files" to create new Java files in the repo manually. Create new files with name `TicketPricer.java` You can re-type or copy paste your code into those files.

B) Click "Upload Files" to just upload the `.java` files you already created. 

Once you've created the file you want, or uploaded them, navigate to the bottom of the Page and hit "Commit changes". Ensure "Commit directly to the main branch." is selected. You'll need to "Commit changes" once for each file you "Create" in GitHub, but can upload multiple files before a single Commit.


