# Assignment 1: Design a Logical Model

## Question 1
Create a logical model for a small bookstore. 📚

At the minimum it should have employee, order, sales, customer, and book entities (tables). Determine sensible column and table design based on what you know about these concepts. Keep it simple, but work out sensible relationships to keep tables reasonably sized. Include a date table. There are several tools online you can use, I'd recommend [_Draw.io_](https://www.drawio.com/) or [_LucidChart_](https://www.lucidchart.com/pages/).

<img width="627" alt="Assignment_q1" src="https://github.com/AdithyaLab/sql/assets/167127254/d7f51165-0d71-4057-a41f-d0bcec0ac16c">

```
I am assuming that employees have no direct relationship with sales or orders for this database. Employees purely manage store operations.
```


## Question 2
We want to create employee shifts, splitting up the day into morning and evening. Add this to the ERD.

<img width="653" alt="Assignment_q2" src="https://github.com/AdithyaLab/sql/assets/167127254/3b13caf7-b023-40c9-a802-66832ccf2a1d">


## Question 3
The store wants to keep customer addresses. Propose two architectures for the CUSTOMER_ADDRESS table, one that will retain changes, and another that will overwrite. Which is type 1, which is type 2?

_Hint, search type 1 vs type 2 slowly changing dimensions._

<img width="519" alt="Assignment_q3" src="https://github.com/AdithyaLab/sql/assets/167127254/ce81c910-946f-4c8d-837c-724624692cf3">

Bonus: Are there privacy implications to this, why or why not?
```
Your answer...
For the type 1 architecture, the old address is overwritten by the new address and the old data is deleted. This means there are fewer privacy concerns as only one address is available at any one time. For the type 2 architecture, old addresses are stored, providing a more extensive history of a customer's address history, which could raise privacy concerns.
```

## Question 4
Review the AdventureWorks Schema [here](https://i.stack.imgur.com/LMu4W.gif)

Highlight at least two differences between it and your ERD. Would you change anything in yours?
```
Your answer...
1) The Schema centers one "mega" table for each "coloured" function such as Employee, Person, SalesOrderHeader, Product and Vendor. This simplifies the overall architecture for a large database. If i was to expand on the data collected by the book store, I would follow this "hub and spoke" model
2) The Schema uses modified dates, utilizing the type 2 slowly changing dimension architecture. This means that the old data will be retained in the database. I would consider this architecture for my ERD if there was a regulatory requirement to do so, but for the purposes of reducing privacy risks, I will keep it the same.
```

# Criteria

[Assignment Rubric](./assignment_rubric.md)

# Submission Information

🚨 **Please review our [Assignment Submission Guide](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md)** 🚨 for detailed instructions on how to format, branch, and submit your work. Following these guidelines is crucial for your submissions to be evaluated correctly.

### Submission Parameters:
* Submission Due Date: `June 1, 2024`
* The branch name for your repo should be: `model-design`
* What to submit for this assignment:
    * This markdown (design_a_logical_model.md) should be populated.
    * Two Entity-Relationship Diagrams (preferably in a pdf, jpeg, png format).
* What the pull request link should look like for this assignment: `https://github.com/<your_github_username>/sql/pull/<pr_id>`
    * Open a private window in your browser. Copy and paste the link to your pull request into the address bar. Make sure you can see your pull request properly. This helps the technical facilitator and learning support staff review your submission easily.

Checklist:
- [ ] Create a branch called `model-design`.
- [ ] Ensure that the repository is public.
- [ ] Review [the PR description guidelines](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md#guidelines-for-pull-request-descriptions) and adhere to them.
- [ ] Verify that the link is accessible in a private browser window.

If you encounter any difficulties or have questions, please don't hesitate to reach out to our team via our Slack at `#cohort-3-help`. Our Technical Facilitators and Learning Support staff are here to help you navigate any challenges.
