# Digital Restaurant Menu
A simple table-ordering web platform , the customer types the name and table number, opens that restaurants menu , orders preferred meal , they see waiting waiter then a countdown then a receipt appears , click pay and customer is directed to pay , customer pays and receipt stored.

## How it works
1. **Home (`index.html`):** the customer types the restaurant name and their sitting table number.
2. **Menu (`menu.html`):** they browse by category (Breakfast, Drinks, Lunch, Dinner) and tap **Order** on a meal.
3. **Waiter (`waiter.html`):** the order appears here. The waiter types the minutes by  which the meal should be ready and taps **Start timer**.
4. **Order (`order.html`):** the customer sees their meal and the countdown. When it reaches zero, the meal disappears and the receipt shows with a **Pay** button.
5. **Receipt (`receipt.html`):** the customer taps **Pay**. The payment is saved and appears in the payment history.

## Pages

| File | Purpose |
| --- | --- |
| `index.html` | Landing page, collects restaurant name and Sitting table number |
| `menu.html` | Meal list with a category dropdown and Order buttons |
| `waiter.html` | Shows the current order, waiter sets the wait time |
| `order.html` | Customer view: live countdown, then receipt and Pay |
| `receipt.html` | customer Pays the bill and view the payment history |
 

