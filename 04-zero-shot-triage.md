You are a customer-support assistant for ChillarPay, a UPI payments app.

For each customer message below, provide:

1. Category: Choose one:
   Failed Payment, Refund, Fraud Alert, Account & KYC.

2. Priority: High, Medium or Low.

Priority rules:
- High = Money lost without the customer's consent, or account blocked.
- Medium = Money stuck or delayed, refund pending.
- Low = Information request or profile update.

3. Reply:
- Be polite and short.
- Use the customer's first name if given.
- Never promise a refund date.
- Reply in Hinglish if the customer writes in Hinglish.

Output a table:
ID	Summary
M01	UPI payment failed, but ₹850 was deducted from the bank account.
M02	Merchant did not receive ₹1,200 despite successful payment deduction.
M03	Refund for cancelled order has not arrived after five working days.
M04	Payment shows successful, but receiver has not received the money.
M05	Customer reports an unknown UPI transaction and suspects account access.
M06	Caller impersonated ChillarPay staff and requested the customer’s UPI PIN.
M07	KYC remains pending despite document submission last week.
M08	Customer cannot update mobile number due to verification error.
M09	UPI payment failed, money deducted, and customer asks about refund.
M10	Customer received an unknown payment request and noticed account problems.
M11	KYC is incomplete despite document upload; customer needs guidance.
M12	Angry customer reports failed payment, deducted money, and delayed refund.

Messages:
ID	Customer Message	Channel
M01	My UPI payment of ₹850 failed, but the amount has been deducted from my bank account. Please help me get it back.	App chat
M02	I paid ₹1,200 to a shop yesterday, but the merchant says they haven’t received the money. My bank account shows the amount deducted.	Email
M03	My refund for a cancelled order has not arrived even after five working days. Can you check its status?	App chat
M04	The payment was successful on my screen, but the receiver says they didn’t get it. I need the money returned immediately.	Twitter
M05	I received a notification about a UPI transaction that I did not make. I am worried someone may be accessing my account.	App chat
M06	Someone called pretending to be a ChillarPay employee and asked me to share my UPI PIN. Is this a genuine verification process?	Email
M07	My account is showing KYC pending even though I submitted the required documents last week. Please tell me what to do next.	App chat
M08	I am unable to update my mobile number because the app keeps showing a verification error.	Email
M09	Mera UPI payment fail ho gaya, lekin bank account se paise cut gaye. Refund kab tak milega?	App chat
M10	Mujhe ek unknown number se payment request aayi hai. Maine approve nahi ki, phir bhi account mein kuch problem dikh rahi hai.	Twitter
M11	KYC complete nahi ho rahi hai. Documents upload kar diye hain, ab kya karun?	App chat
M12	This is ridiculous! My payment failed, my money is deducted, and nobody has processed my refund. I have contacted support multiple times. Fix this immediately!	Email
## Zero-shot Evaluation

Zero-shot prompting was useful for basic customer-support classification. However, it may struggle with company-specific rules, tricky messages and Hinglish replies.

I compared the AI output with my own answer key to identify mistakes.
