# Calculate-Loyalty-Score
![Untitled](https://user-images.githubusercontent.com/63194399/195833916-c19489c1-1da8-4bea-b27b-0c3ddc946def.png)

This chart shows how we calculate loyalty scores at a high level. Here’s a scenario. The DAO community registered an airdrop through the ParachuteDrop platform, with 6 rounds of airdrops with 4 months round intervals.

![Untitled](https://user-images.githubusercontent.com/63194399/195834019-5b433250-c414-4fb9-b576-da2c0160a1f8.png)

The X-axis represents time, and the Y-axis represents the token amount. The white bold line represents the threshold of airdrop amount per round if the loyalty score was 100%, cumulatively.
The red bold line represents the coefficient for calculating the loyalty score.
The yellow box represents how many tokens you held during a specific round interval. The dark olive-colored area means how many tokens you sold during the period.

![Untitled](https://user-images.githubusercontent.com/63194399/195834123-a680f5f2-d897-42aa-bcbd-75886c086a3d.png)

**The loyalty score represents the area under the bold red line.**
We calculate the score by this equation. We take the minimum value of threshold amount and holding amount, multiplied by the holding period. And this logic prevents buying lots of tokens right before a new airdrop round begins // for the purpose of getting more loyalty scores.

So, the airdrop amount for round N is determined by cumulative loyalty score through round 1 ~ round (N-1)
