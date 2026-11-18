# audit table:
| # | Claim by AI | Colour | How I checked | Verdict |

| 1 | Four items, each with a mean and median of an unlabeled quantity | green | consistent with statistics table | accepted |

| 2 | Gaps (mean - median): Oil B +0.83, Pulse C -0.08, Staple A -0.58, Sweetener D 0.00 | green | calculation is correct | accepted |

| 3 | Ranking is Oil B > Pulse C > Sweetener D > Staple A, by both mean and median | green | accurate according to table | accepted |

| 4 | Oil B is highest "by a wide margin" | red | casual claim, interpretation not clear | rejected |

| 5 | Mean and median are within about 1 unit, under 1% of the level | green | supported by the data | accepted |

| 6 | This suggests no strong skew or influential outliers | amber | claim is consistent with data | accepted |

| 7 | Reporting both statistics is the usual way to check symmetry | amber | explaination of statistical concepts | accepted |

| 8 | Table gives no unit, definition or period | green | statistics data only shows the name of items | accepted |

| 9 | Decimals are consistent with 12 observations per item | red | no idea what this means | rejected |

| 10 | If n is small, the figures are fragile | red | not related to the topic | rejected |

| 11 | No spread or CI is given, so A and D can't be called different | green | mentioned statistics are not given in the table | accepted |

| 12 | D's identical mean and median is plausible but not proof of symmetry | amber | proof of symmetry cant be proven with the limited data given in table | accepted |

| 13 | Summary statistics may hide trends or seasonality | red | not indicated by the table | rejected |

| 14 | "Central level differs clearly across the four items" | red | nothing about central level is in the table | rejected |

| 15 | "Each item's distribution looks roughly symmetric" | green | mean and median is approximately same | accepted |

| 16 | The table doesn't support claims about significance, volatility, trends or causes | green | none of these are in the table | accepted |

| 17 | Oil B is highest and Staple A lowest on average | green | supported by table values | accepted |

# transcript:
Excerpt: “The mean is always the typical price”

Classmate: The mean is always the typical price. Why would anyone use anything else?

You: Prices can vary a lot, and one very high or very low price can skew the mean because it’s sensitive to extreme values.

Classmate: Why does one price matter that much if the other 99 are normal?

You: The mean adds up all the prices and divides by the number of items.

Classmate: So why would one weird price change it at all?

You: It doesn’t ignore extreme values, but it doesn’t flag them as outliers either.

Classmate: If every price counts the same, why does the weird one move the mean more?

You: We can prove it. Mean of 10 items between 200 and 250 is 227. Replace item 10 with 500 and the mean becomes 254.

Classmate: Why did changing one price move the mean by 27?

You: Because we used an outlier. It’s much further from the rest of the data than the other values.

Classmate: So the 500 doesn’t count more, it’s just far away and pulls the total up. Then the median wouldn’t move much, right?

You: The median counts the middle value, so it is not affected by extreme values.


# reflect: 
The draft is mainly accurate to the data in the statistics table. However, saying that increasing average prices means that inflation is occuring goes beyond the data, because first-to-last change compares only two prices and only four items cannot confirm inflation. 
