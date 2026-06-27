# Banking Transactions Analysis – Data Cleaning Process

## Information Before Cleaning
- Records (Rows): 2750  
- Columns (Features): 18  

---

## Steps

1. Imported data into Excel.  
2. Selected the data, inserted tables, and promoted headers.  
3. Started cleaning and transformation using Power Query Editor.  
4. Date column was in mixed format → changed datatype using Locale (Date, English-India).  
5. Transformed **Customer_Name** column into Proper Case.  
6. Transformed **Transaction_ID** column into Upper Case.  
7. Transformed **Account_Type** column into Proper Case.  
8. Replaced “-”, “N/A”, “Na”, “Null” with null and replaced “Fd” with “Fixed Deposit” in **Account_Type**.  
9. Transformed **Transaction_Type** column into Proper Case.  
10. Replaced “-”, “N/A”, “Na”, “Null” with null; “C”, “Cr” → Credit; “D”, “Dr” → Debit in **Transaction_Type**.  
11. Changed **Amount** column datatype to Text to replace values.  
12. Replaced “-”, “N/A”, “NA”, “NULL” with null; removed “₹”, “INR”, “Rs.”, “/-” in **Amount**.  
13. Changed **Amount** datatype to Decimal Number.  
14. Transformed **Currency** column into Proper Case.  
15. Replaced “Rs.”, “Rs” → INR; replaced “-”, “N/A”, “Na”, “Null” with null.  
16. Trimmed column where similar words “Inr” appeared.  
17. Replaced “-”, “N/A”, “Na”, “Null” with null in **Customer_Name**.  
18. Changed **Balance_After** datatype to Text to replace values.  
19. Replaced “-”, “N/A”, “NA”, “NULL”, “null” with null in **Balance_After**.  
20. Changed **Balance_After** datatype to Decimal Number.  
21. Transformed **Channel** column into Proper Case.  
22. Replaced “-”, “N/A”, “Na”, “Null” with null in **Channel**.  
23. Transformed **Status** column into Proper Case.  
24. Replaced “-”, “N/A”, “Na”, “Null” with null in **Status**.  
25. Transformed **Category** column into Proper Case.  
26. Replaced “-”, “N/A”, “Na”, “Null” with null in **Category**.  
27. Transformed **Merchant_Name** column into Proper Case.  
28. Replaced “-”, “N/A”, “Na”, “Null” with null in **Merchant_Name**.  
29. Replaced “-”, “N/A”, “Na”, “Null” with null in **Bank_Name**.  
30. Changed **Bank_Name** datatype to Text.  
31. Changed **Phone_Number** datatype to Text to replace values.  
32. Replaced “-” with blank and “N/A” with null in **Phone_Number**.  
33. Replaced “-”, “N/A”, “NA”, “null”, “NULL” with null in **Transaction_Ref**.  
34. Transformed **City** column into Proper Case.  
35. Replaced “-”, “N/A”, “Na”, “Null” with null in **City**.  
36. Transformed **Remarks** column into Proper Case.  
37. Replaced “-”, “N/A”, “Na”, “Null” with null in **City** (duplicate handling).  
38. Changed **Account_Number** datatype to Text to replace values.  
39. Replaced “-”, “N/A”, “NULL”, “NA” with null in **Account_Number**.  

---

## Null & Blank Values Transformation

### Delete & Remove
40. Deleted 1 row where Transaction_ID and Amount were null.  
41. Deleted 1 row where Transaction_ID and Account_Number were null.  
42. Deleted 5 rows where Transaction_ID and Balance_After were null.  
43. Deleted 6 rows where Transaction_ID and Transaction_Ref were null.  
44. Deleted 4 rows where Transaction_ID and Customer_Name were null.  
45. Removed 119 duplicate values in Transaction_ID.  
46. Removed 1 null value in Transaction_ID.  
47. Removed 57 blank values in Amount.  

### Replace
48. Replaced 68 blank values in **Customer_Name** with “Unknown”.  
49. Replaced 51 blank values in **Account_Number** with “Unknown”.  
50. Replaced 104 blank values in **Account_Type** with “Other”.  
51. Replaced 52 blank values in **Transaction_Type** with “Unknown”.  
52. Replaced 164 null values in **Balance_After** with “0”.  
53. Replaced 87 blank values in **Channel** with “Unknown”.  
54. Replaced 76 blank values in **Status** with “Unknown”.  
55. Replaced 138 blank values in **Category** with “Unknown”.  
56. Replaced 431 blank values in **Merchant_Name** with “Unknown”.  
57. Replaced 70 blank values in **Bank_Name** with “Unknown”.  
58. Replaced 499 blank values in **Phone_Number** with “Unknown”.  
59. Replaced 175 blank values in **Transaction_Ref** with “Unknown”.  
60. Replaced 90 blank values in **City** with “Other”.  
61. Replaced 646 blank values in **Remarks** with “Not Provided”.  

---

## Information After Cleaning
- Records (Rows): **2522**  
- Columns (Features): **18**  
