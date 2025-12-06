# Stats and Charts for The Cat

This directory contains supporting statistics and visualizations for  
**The Cat: Non-Monetary UTXO Cleanup**.

These numbers and charts are **non-normative**: they illustrate the scale and
structure of inscription-related UTXOs, but they do not by themselves define
any consensus constants.

---

## Snapshot metrics (Ord inscriptions)

As of block **926301**:

- Total inscriptions: **112,568,163**
- UTXOs containing at least one inscription: **51,801,803**

Value / concentration observations:

- Most inscriptions live in UTXOs below **10,000 sats**.
- There are **74,057** “whale” UTXOs that contain inscriptions.
- **Average inscriptions per whale UTXO:** **718.59**
- **Maximum inscriptions in a single whale UTXO:** **663,733**

---

## Actual UTXO count by value

This chart shows the *actual* distribution of inscription-bearing UTXOs by
value bucket, on a log scale, with raw counts annotated.

![Actual UTXO Count by Value](./chart_real_utxo_value.png)

---

## Distribution of UTXO values (dust vs. whales)

This chart emphasizes how many inscription-bearing UTXOs are dust-sized
compared to the smaller population of large “whale” outputs.

![Distribution of UTXO Values (Emphasis on Dust vs. Whales)](./utxo-value-histogram.png)

---

## Inscription activity over time

This chart shows how many inscriptions were minted per block, highlighting the
bursty, high-intensity periods of inscription activity across the Ordinals era.

![Inscription Activity by Block Height](./chart_activity_pulse.png)

---

## Growth of the inscribed UTXO set

Here we plot the cumulative number of unique UTXOs that contain inscriptions as
a function of block height, making the rapid growth of the inscribed UTXO set
visually clear.

![Growth of the Inscribed UTXO Set Over Time](./utxo-count-over-time.png)

---

## Inscription density per UTXO

This chart shows how many inscriptions are packed into each UTXO (1, 2–5, 6–10,
…, 1k+), on a log scale. It highlights the existence of extremely dense carrier
UTXOs, including ones with hundreds of thousands of inscriptions.

![Inscription Density per UTXO]()
