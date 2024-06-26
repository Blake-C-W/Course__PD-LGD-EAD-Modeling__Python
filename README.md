# Course__PD-LGD-EAD-Modeling__Python
Modeling Probability of Default, Loss Given Default, and Exposure at Default

## Models
* PD: Binomial Logistic Regression
* LGD: Beta Regression
* EAD: Beta Regression

## Expected loss(EL) and its components: PD, LGD, and EAD
### Types of factors for expected loss
* Borrower Specific
* Economic Environment
  
### Established credit risk modeling defines expected loss as PD x LGD x EAD
* PD = Probability of Default
* LGD = Loss Given Default (Min Loss)
* EAD = Exposure at Default (Max Loss)

### Example
* Borrower wants to buy house for $500,000
* Lender funds 80% (LTV)
* Loan Amount = $500,000 x .8 = $400,000
* Borrower paid $40,000 so far (outstanding balance = $360,000)
* If borrower defaults EAD will be $360,000
* Assuming imperical evidence that 1 in 4 homeowners default (PD = 1/4 or 25%)
* If borrwer defaults and bank can sell the house for $342,000 immediately then EAD will equal $360,000 - $342,000 = $18,000
* LGD = $18,000 / $360,000 = 5%
* EL = 25% (PD) x 5% (LGD) x $360,000 (EAD) = $4,500

## Capital adequacy, regulations, and the Basel II accord
### Basel II Accord
- Minimum capital Requirements:
  1. Credit Risk
     * Standardized Approach (SA)
     * Internal Ratings Based (IRB) Approaches
         1. Foundation Internal Ratings Based (F-IRB) Approach
         2. Advanced Internal Ratings Based (A-IRB) Approach
  3. Operational Risk
  4. Market Risk

## Basel II approaches: SA, F-IRB, and A-IRB
- SA (PD: External, LGD: External, EAD: External)
  - lending to countries:
    - Risk Weights
      * AAA to AA-: 0%
      * A+ to A-: 20%
      * BBB+ to BBB-: 50%
      * BB+ to B-: 100%
      * Below BB-: 150%
      * Unrated: 100%
  - lending to firms:
    - Risk Weights
      * AAA to AA-: 20%
      * A+ to A-: 50%
      * BBB+ to BB-: 100%
      * Below BB-: 150%
      * Unrated: 100%
  - Retail Risk Weight: %75
  - Retail Risk Weight: %35
- F-IRB (PD: Internal, LGD: External, EAD: External)
- F-IRB (PD: Internal, LGD: Internal, EAD: Internal)

