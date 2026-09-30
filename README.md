
Your project is ready for real business data. Start in this order:

1. **Sign in:** Use the email and password for a user you created in your Supabase project’s **Authentication → Users**. The app doesn’t have a default password.
2. **Add products:** Go to **Inventory → Add product**. Only **Name** is required. For example:
   - Name: `Notebook`
   - SKU: `NOTE-A5`
   - Category: `Stationery`
   - Unit: `pcs`
   - Cost price: `40`
   - Sell price: `60`
   - Stock quantity: `25`
   - Low stock alert at: `5`
3. **Add customers:** Go to **Customers → Add customer**. **Name** is required; phone, email, and notes are optional. Example: `Asha Kumar`, `9876543210`, `asha@example.com`, `Monthly customer`.
4. **Create a bill:** Go to **Billing**, search for a product and add it to the cart. Set quantities and prices, select a customer or leave it as **Walk-in customer**, and adjust discount or tax if needed. Tax starts at **5%**. Saving the invoice automatically reduces stock.
5. **Review invoices and reports:** Invoices can be marked paid; dashboard and reports summarize sales and stock.

Your Customers page currently shows **0 customers** and a notice that there are no products. You can enter them manually as above, or use the `SEED DATA` section of `schema.sql` to load demo records. The project displays money in rupees (₹).



Yes. Right now your app runs **locally** on your laptop, so after shutting down, the web server stops. To use it again:

1. Open the project folder in VS Code.
2. Open the terminal in that folder.
3. Run `npm.cmd run dev`.
4. Open `http://localhost:3000`.

Leave that terminal running while you use the app. You don’t need to run the command every time you open another browser tab, only when the server has stopped, such as after shutting down or restarting your laptop.

If you want to open the app without starting it yourself, you’d need to deploy it to a hosting service such as Vercel and connect it to Supabase.
