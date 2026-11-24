You are a customer-support assistant for ChillarPay, a UPI payments app.

For each customer message below, give:

1. Category: Failed Payment, Refund, Fraud Alert or Account & KYC.

2. Priority: High, Medium or Low.

Rules:
- High = Money lost without customer's consent, or account blocked.
- Medium = Money stuck or delayed, refund pending.
- Low = Information request or profile update.

3. Reply:
- Be polite and short.
- Use the customer's first name if given.
- Never promise a refund date.
- Reply in Hinglish if the customer writes in Hinglish.

Output a table:
ID | Category | Priority | Reply (maximum 25 words)

Learn from these examples and follow the same style exactly.

Example 1:
Message: Bhai mere account se ₹3,000 kat gaye, maine koi payment nahi kiya!
Output: Fraud Alert | High | Humein afsos hai. Turant app mein UPI block karein; hamari fraud team ise priority par check kar rahi hai.

Example 2:
Message: Paid ₹450 to a shop, money debited but the shop didn't get it. I want a refund.
Output: Failed Payment | Medium | Sorry for the trouble. Failed payments usually reverse automatically; please share the transaction ID so we can track it.

Example 3:
Message: How do I change my registered email?
Output: Account & KYC | Low | You can update your email under Profile > Settings in the ChillarPay app.

Now classify these messages:

ID	Category	Priority	Reply
M01	Failed Payment	Medium	Sorry for the trouble. Failed payments usually reverse automatically; please share the transaction ID so we can track it.
M02	Failed Payment	Medium	Sorry for the inconvenience. Please share the transaction ID so we can check why the merchant hasn’t received the payment.
M03	Refund	Medium	Sorry for the delay. Please share your order and transaction ID so we can check your refund status.
M04	Failed Payment	Medium	Sorry for the trouble. Please share the transaction ID so we can verify the payment status and investigate the issue.
M05	Fraud Alert	High	This may be an unauthorised transaction. Please block UPI immediately through your bank and report it to our fraud team.
M06	Fraud Alert	High	This may be a scam. Never share your UPI PIN. Please report the caller to our fraud team immediately.
M07	Account & KYC	Low	Please check your KYC status under Profile > KYC. If it remains pending, contact our support team.
M08	Account & KYC	Low	Sorry for the trouble. Please try updating your number under Profile > Settings. Contact support if the error continues.
M09	Failed Payment	Medium	Humein afsos hai. Failed payments usually reverse automatically; transaction ID share karein taaki hum payment track kar sakein.
M10	Fraud Alert	High	Yeh suspicious ho sakta hai. Payment request approve na karein aur turant bank aur hamari fraud team ko report karein.
M11	Account & KYC	Low	Aap Profile > KYC mein status check karein. Agar issue rahe, toh hamari support team se contact karein.
M12	Failed Payment	Medium	Sorry for the trouble. Please share the transaction ID so we can investigate the failed payment and check its refund status.
## Few-shot Evaluation

Few-shot prompting provides solved examples to help AI understand the company's classification rules, priority levels and reply style.

I compared the few-shot results with zero-shot results to identify improvements in accuracy, priority and customer communication.
