# FQX Technical Full-stack challenge

**The goal of the challenge:**

Create:
1) A responsive form where you can fill all the required fields and the rest respond as specified in the business background.
2) The contents of the fields are being stored in a small backend service.
   1) Your form should fetch the right data based on the url and therefore persist a page reload
   2) Updating the fields should trigger an update in the backend
   3) It is up to you if you want to store all the data in the backend or recalulate some of them on retrieval

As you're implementing a full-stack application you should focus on the correctness and the integration of the backend service,
more than focusing on the design and styling.

**The business background:**

We enable a corporation to define a corporate finance eNote deal. A user first inserts the financing amount
(=the amount of money desired to be borrowed) and the payment date (=the date when the investor should transfer the money).
Then, in the following, the corporation defines the eNote Due Date (=the date when the borrowing corporation has to pay the money back),
the difference is the maturity. Because the investor wants to make a certain profit, the eNote Face Value
(=the amount of money the borrowing corporation has to pay back) must be a bit higher than the purchase price.

The difference is the Agio. To help to calculate the eNote Face Value, you can insert either the **Agio %**, the **Agio in CHF** or the **APR %**
(=the annual interest rate).
Then the other fields including the Face Value are automatically calculated and updated in place.
Of course, you can also directly insert the Face Value (then the other 3 fields are calculated).

For the APR % calculation use european method days360 function.
It is up to you to use a library or implement it given the specification.


**The form:**

**There should be 8 fields that are used for calculations:**

• purchasePrice

• paymentDate

• dueDate

• maturity

• agioPercentage

• agioValue

• aprPercentage

• faceValue
 
