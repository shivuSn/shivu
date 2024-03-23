**GoldBuying Contract**

**Overview:**
The GoldBuying contract is designed to facilitate the purchase of gold by users. It includes functionalities for checking the availability of gold carats, buying gold, and purchasing gold in grams. The contract enforces certain conditions such as a minimum amount of gold to buy and a threshold for free membership.

**Instructions for Use:**
1. **CaratsAvailability Function:**
   - This function checks the availability of gold carats within the range of 18 to 22 carats.
   - Input: `carrot` - an integer representing the carat value.
   - Output: None.
   - Behavior: Throws an assertion error if the carat value is not within the specified range.

2. **buyGold Function:**
   - This function is used to buy gold.
   - Input: `amount` - an integer representing the amount of gold to buy in grams.
   - Output: None.
   - Behavior: Requires that the amount of gold to buy is greater than or equal to the minimum gold amount specified (6000 grams). Throws an error if the requirement is not met.

3. **goldgram Function:**
   - This function is used to check if a user qualifies for free membership based on the amount of gold purchased.
   - Input: `gram` - an integer representing the amount of gold purchased in grams.
   - Output: None.
   - Behavior: If the amount of gold purchased is greater than or equal to the free membership threshold (100 grams), it reverts with an error message indicating that free membership is provided.

4. **purchaseGold Function:**
   - This function is used to purchase gold in grams.
   - Input: `grams` - an integer representing the amount of gold to purchase in grams.
   - Output: A string message indicating the success of the purchase.
   - Behavior: Calls the `buyGold` function to ensure the purchase meets the minimum requirements and then returns a success message.

**License:**
This contract is licensed under the MIT License, as indicated by the SPDX-License-Identifier tag at the beginning of the code.

**Author** 

Shivaraj 

shivun12890@gmail.com
