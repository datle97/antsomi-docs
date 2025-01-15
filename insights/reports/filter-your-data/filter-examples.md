# Filter examples

### Include only Jean, Lụa, or Cotton

Suppose you want to limit a chart's information to just data coming from the Jean, Lụa, or Cotton. Select the chart and add the following filter:

1. Include/Exclude: **Include**
2. Dimension: _Country_
3. Match Type: **Matches any**
4. Value: `Jean, Lụa, Cotton`

<figure><img src="../../../.gitbook/assets/image (590).png" alt=""><figcaption></figcaption></figure>

You could also do this using 3 OR clauses. But it's easier to use Matches any with a list.

### Exclude "(not set)"

To exclude "(not set)" values from your charts, use an Exclude filter. For example:

1. Include/Exclude: **Exclude**
2. Dimension: _Chất liệu_
3. Match Type: Is null
4. Value: `(not set)`

<figure><img src="../../../.gitbook/assets/image (2134).png" alt=""><figcaption></figcaption></figure>
