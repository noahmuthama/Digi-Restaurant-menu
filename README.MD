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

## Data (localStorage)
 
All data lives in the browser's localStorage.
 
| Key | What it holds |
| --- | --- |
| `restaurant` | Restaurant name typed on the home page index.html |
| `table` | Table number typed on the home page |
| `order` | The current order: `name`, `price`, `image`, `category`, `restaurant`, `table`, `time`, `endTime` |
| `receipts` | List of all paid orders, each with a `paidAt` time |

## Project structure
 
```
index.html
menu.html
order.html
waiter.html
receipt.html
kitchen-menu.png        (home page hero image)
menu/                   (meal photos used by menu.html)
```

## Run it

**Try it online:** https://noahmuthama.github.io/Digi-Restaurant-menu/

**Or run it on your computer:**

1. Clone the repo:
   ```bash
   git clone https://github.com/noahmuthama/Digi-Restaurant-menu.git
   cd Digi-Restaurant-menu
   ```
2. Open the folder in VS Code and start **Live Server** on `index.html`.
3. Open every page in the **same browser**, because localStorage is not shared between browsers or devices.
 
 ## Known limitations
 
- Customer and waiter must use the same browser on the same device, since there is no server. For real use on separate phones, the orders need a backend or a service like Firebase.
- Only one active order at a time. A new order replaces the previous one.
- Pay is a confirmation only. There is no real payment such as M-Pesa yet.
- The **Notify** button is not connected to anything yet.


## Ideas for later
 
- Optional feedback after payment
- Order code shown to the customer
- Multiple orders per table
- M-Pesa payment
- Backend so waiter and customer can use different devices

 

