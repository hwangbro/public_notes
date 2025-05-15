# Time analysis for cutting 2 grass tiles on Route 34

- Time lost to using Cut from menu: 4.16s

Encounter Slot | Pokemon | Timeloss
-------------- | ------- | --------
30%            | Snubbull | 13.82
30%            | Rattata | 13.42
20%            | Pidgey | 13.28
10%            | Abra | 14.1
5%            | Jigglypuff | 13.37
4%            | Ditto | 13.57
1%            | Ditto | 13.57

- Average timeloss for encounter weighted: 13.585s
- Encounter rate: 25/256
- Chance of 0 encounter: `(1 - 25/256) ^ 2` = 53361/65536 ~= 81.4224%
- Chance of 1 encounter: 12175/65536 ~= 18.5776%
- Average timeloss due to encounters: .185776 * 13.585 = 2.52376s

## Conclusion
- Cut loses 1.63624s on average.
- 81.4224% of the time, cut loses 4.16s
- 18.5776% of the time, cut saves 9.425s
