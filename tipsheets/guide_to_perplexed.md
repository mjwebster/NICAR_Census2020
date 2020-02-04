
# Census return rates vs response rates: A guide to the perplexed

The Census Bureau uses two confusingly similar yardsticks to measure how well the public responds to a census. One is called the "response rate," (or "mail response rate" in 2010, when mailing the census form back was the main way to respond.) The other is the "return rate" (formerly "mail return rate.")

The response rate is quicker to calculate but less precise. The return rate is more precise but takes data that isn't available until late stages of the census. It helps to think about them as answers to a similar question asked from two different viewpoints:

- The response rate is from the Census Bureau's viewpoint: We sent out 100 invitations -- how many *responses* did we get?
- The return rate is from our viewpoint: 100 of us got invitations -- how many of us *returned* them?

The key difference: The return rate doesn't include invitations to respond:
- That the U.S. Postal Service returns to the Census Bureau as "undeliverable as addressed";
- That were sent to addresses that are eventually determined to be vacant;
- That were sent to addresses that are eventually deleted (because a housing unit was destroyed, converted to non-residential use, etc.)

Figuring out which addresses *not* to count for the return rate takes weeks of follow-up field work. That's why the response rate is useful. It can be calculated daily while the census is still under way. Watch for the Census Bureau to publicize this from mid-March until well into the summer.

It's useful to think of the response rate as similar to election night vote tallies -- imprecise but usually good enough to figure out the broad outline of what happened. The return rate is similar to the final certified vote tally, once absentee and provisional ballots have been counted: long in coming, but important to understand the nuance of the "who" and "where."

The return rate is a better measure of the civic response to the request (and legal obligation) to be counted. So it's heartening that it's higher than the response rate, sometimes substantially so. In 2010, the nationwide final return rate was 79 percent, while the response rate was just 67 percent.

Calculating the rates
Both rates use the same numerator -- households that have responded, whether by mail, online or by phone. (If a household responds more than once, the Census Bureau tries to catch that and count only one.)

The denominator of both rates includes addresses that got an invitation. In fact, that's the entire denominator for the response rate. The denominator for the return rate, however, starts with addresses that got an invitation but then subtracts the three categories of addresses listed above, since they couldn't return anything: undeliverables, vacants and deletes.

Like this:
```markdown
Response rate =
(Unduplicated non-blank responses  / Addresses that got invitations) x 100
```

```markdown 
Return rate =
(Unduplicated non-blank responses  / Addresses that got invitations - (undeliverable + vacant + delete) ) x 100
```

The Census Bureau says that to approximate the 2010 response rate, you can use the following variables from its 2019 Planning Database:

- For "Unduplicated non-blank responses," use "Census_Mail_Returns_CEN_2010."
It represents all housing units that returned a form.

- For "Addresses that got invitations," use "Mailback_Area_Count_CEN_2010."
It represents all housing units that were sent a form.

To calculate the 2010 return rate, you'll also need:
- Undeliverable: Use "Census_UAA_CEN_2010."
- Vacant: Use "Vacants_CEN_2010."
- Delete: Use "Deletes_CEN_2010."

<a href="https://www.census.gov/topics/research/guidance/planning-databases.html">The 2019 Planning Database can be found here</a>
