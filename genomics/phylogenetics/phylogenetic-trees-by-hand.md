# Phylogenetic trees by hand

1\) Start with aligned sequences:

![Aligned sequences A-F](../../.gitbook/assets/image%20%284%29.png)

2\) Build a table of all of the differences between two sequences. For example, sequences A and B have 9 differences

![Just an example showing there are 9 differences between A and B](../../.gitbook/assets/image.png)

![The actual table we&apos;ve made of all the differences. Try it yourself!](../../.gitbook/assets/image%20%2815%29.png)

3\) Find a pair of sequences that has the fewest differences. In this case, there's a tie--\(B and E\) and \(A and C\) each only have 2 differences. Draw branches to connect those pairs.

![We connected \(A and C\) and \(B and E\)](../../.gitbook/assets/image%20%283%29.png)

4\) Re-do the table \(from step 2\) but with A-C and B-E as one group. To find the number of differences between a group \(like \(A and C\)\) and a single sequence \(like D\) just take the average. For example, D has 4 differences with A and 5 differences with C, so it has 4.5 differences with \(A and C\). 

![Our first table with combined sequences!](../../.gitbook/assets/image%20%2811%29.png)

Now we just keep repeating steps 3 and 4, like so:

\(3 again\) The two sequences that have the fewest differences are \(A and C\) and D. So let's combine those. 

![Making progress!](../../.gitbook/assets/image%20%281%29.png)

\(4 again\) make the new table

![More tables!](../../.gitbook/assets/image%20%288%29.png)

\(3 again\) The sequences with the fewest differences are \(A and C and D\) and \(B and E\). Combine those

![This is starting to look legit](../../.gitbook/assets/image%20%2814%29.png)

At this point, we don't need to make another table because we only have 1 sequence left \(poor F\). So let's just throw that on the end:

![That&apos;s our tree!](../../.gitbook/assets/image%20%2819%29.png)

{% embed url="https://www.youtube.com/watch?v=09eD4A\_HxVQ" %}



