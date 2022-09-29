# Amazon_Vine_Analysis

# Purpose of this project:
To use PySpark, PostgresSQL, Pandas and AWS service to determine if the reviews for Health Personal Care category have any bias between vine (paid) program and non-vine program.

# Result
- How many Vine reviews and non-Vine reviews were there?

![Vine review](Images/vine_program_review_counts.png)

There are 497 reviews are from the Vine program.

![Non-vine review](Images/non_vine_program_review_counts.png)

There are 120,825 reviews are from the non-Vine program.

- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

![Total Review Numbers](Images/review_numbers.png)

After we filtered with reviews that has equal or greater than 20 votes of helpful_votes and the helpful_votes has equal or greater than 50% of rates, we got the following results for the counts of reviews:
Total Review: 121,322
Total Vine Review: 497
Total non-Vine Review: 120,825

- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
![Vine Percentage](Images/vine_program_percentage.png)
![Vine Percentage Chart](Images/vine_program_pie.png)

There are about 44% of five-stars review for the Vine program.

![Non-Vine Percentage](Images/non_vine_program_percentage.png)
![Non-Vine Percentage Chart](Images/non_vine_program_pie.png)

There are about 62% of five-stars review for the non-Vine program.

# Summary
From the results we can see, after we applied the filters for the reviews, total reviews for the Vine program only has 497 reviews out of 121,322 of total reviews, which is a very small number. And there are about 44% of five-stars review out of 497 reviews for the Vine program v.s. 62% of five-star review out of 120.825 reviews for the non-Vine program. The five-stars reviews from non-vine program are overwhelmingly higher than the Vine program. From the results I can't see the signs of bias reviews from the Vine program.

For furthur analysis, we can see how many of the Vine five-stars reviews are verified purchase and how many of the non-Vine five-stars reviews are verified purchase. Or if the number of helpful_votes for vine program reviews are higher than non-Vine program reviews.
