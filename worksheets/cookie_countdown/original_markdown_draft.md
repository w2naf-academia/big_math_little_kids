# The Cookie Countdown: A Rates Worksheet

Oct 31, 2026 · @Nathaniel

## The story

The bakery just baked **15,000 chocolate chip cookies**. That is a LOT of cookies!

Cookie Monster sneaks in. He eats **20 cookies every minute**. Nom nom nom.

The Count wants to count the cookies. But every time he looks up, there are fewer! "Ah ah ah! The number keeps CHANGING!"

Today we will help The Count. We will learn how to figure out how many cookies are left, even while Cookie Monster is still eating.

## Big idea: a rate is "how much changes each minute"

Cookie Monster eats at the same speed the whole time: 20 cookies, then 20 more, then 20 more. That speed is called a **rate**.

The cookie pile goes **down** by 20 every minute. Mathematicians say the cookies are *changing* at a rate of **minus 20 cookies per minute**. The minus means "getting smaller."

Try it: put 20 counters (beans, blocks, or paper cookies) in a pile. Take 20 away. That was one minute of Cookie Monster!

**Question 1.** Is the cookie pile getting bigger or smaller? \_\_\_\_\_\_\_\_\_\_\_\_

**Question 2.** How many cookies does Cookie Monster eat in 1 minute? \_\_\_\_\_\_

## Warm-up: a small plate of 100 cookies

Before the giant bakery, let's practice with one plate of **100 cookies**. Cookie Monster still eats 20 every minute. Help The Count fill in the table by counting **back** by 20s.

| Minutes gone by | Cookies eaten so far | Cookies left |
| --- | --- | --- |
| 0 | 0 | 100 |
| 1 | 20 | 80 |
| 2 |  |  |
| 3 |  |  |
| 4 |  |  |
| 5 |  |  |

**Question 3.** After how many minutes is the plate empty? \_\_\_\_\_\_ minutes

**Question 4.** Look at the "Cookies left" column. How much smaller does it get each row? \_\_\_\_\_\_

That number is the **rate**. It is the same in every row! That is the secret The Count needs.

## Related rates: the chocolate chips disappear too!

Every cookie has **10 chocolate chips**. When a cookie disappears, its 10 chips disappear with it. So the chips and the cookies are *related*: if we know one rate, we can find the other.

1 cookie eaten → 10 chips gone. 2 cookies eaten → 20 chips gone. Count by 10s!

**Question 5.** Cookie Monster eats 20 cookies in one minute. How many chips is that? Count by 10s twenty times, or use 20 groups of 10. \_\_\_\_\_\_ chips per minute

**Question 6.** Which number goes down faster each minute: cookies or chips? \_\_\_\_\_\_\_\_\_\_\_\_

This is called **related rates**: two things change together, and one changes 10 times as fast as the other.

## The big bakery: 15,000 cookies

15,000 is too many to count one at a time, even for The Count! So we use groups. From the warm-up, we know **one plate of 100 cookies lasts 5 minutes**.

**Question 7.** 10 plates make 1,000 cookies. If each plate takes 5 minutes, how long do 10 plates take? Count by 5s ten times. \_\_\_\_\_\_ minutes

**Question 8.** The bakery has 15 groups of 1,000 cookies. Each group takes the answer from Question 7. Count by 50s fifteen times: 50, 100, 150, … \_\_\_\_\_\_ minutes

**Question 9.** That is a long time! It is about 12 and a half hours. If Cookie Monster starts at breakfast (7:00 in the morning), about when does he finish? Circle one:

- Lunch time
- Dinner time
- Next week

**Draw it!** Draw a big cookie pile. Draw an arrow pointing down and write "−20 every minute" next to it.

## Grown-up corner: the calculus behind it

Let C(t) be cookies remaining and t be minutes. Cookie Monster's constant appetite is a first-order differential equation with an initial condition:

```latex
\frac{dC}{dt} = -20, \qquad C(0) = 15{,}000
```

Integrating gives the solution, and setting C = 0 gives the time the bakery is empty:

```latex
C(t) = 15{,}000 - 20t, \qquad t_{\text{empty}} = \frac{15{,}000}{20} = 750 \text{ min} = 12.5 \text{ h}
```

The chips are the related rate. With P = 10C chips, differentiating both sides gives:

```latex
\frac{dP}{dt} = 10\,\frac{dC}{dt} = -200 \text{ chips/min}
```

What the kids actually did maps onto this cleanly: the "Cookies left" table is a discrete solution of the ODE, Question 4 recovers dC/dt from the table, and Question 5 is the chain rule done by skip counting.

Optional extension for older or advanced kids: The Count counts 60 cookies per minute while Cookie Monster keeps eating. He finishes when counted = remaining, so 60t = 15,000 − 20t, giving t = 187.5 minutes. Their closing speed is 60 + 20 = 80 cookies per minute, a nice preview of the idea that rates add.

## Answer key

| Question | Answer |
| --- | --- |
| 1 | Smaller |
| 2 | 20 cookies |
| Warm-up table | Minute 2: 40 eaten, 60 left · Minute 3: 60, 40 · Minute 4: 80, 20 · Minute 5: 100, 0 |
| 3 | 5 minutes |
| 4 | 20 smaller each row (the rate) |
| 5 | 200 chips per minute |
| 6 | Chips (10 times as fast) |
| 7 | 50 minutes |
| 8 | 750 minutes |
| 9 | Dinner time (about 7:30 in the evening) |
