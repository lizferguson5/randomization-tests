# Shuffle the Labels: A Randomization Test Lab

**Live app:** https://lizferguson5.github.io/randomization-tests/

An interactive lab for BIOL 200 (Lecture 11b, Nonparametric & Randomization Tests). Students shuffle group labels to build a null distribution and calculate a randomization-test p-value, first one shuffle at a time and then thousands at once.

## What students do

1. **Meet the data.** Pseudoscorpion females mated with the same male twice (SM, n = 77) or with two different males (DM, n = 72). Students see the group means and the observed difference in means (SM − DM = −0.84), which becomes the threshold for the test.
2. **Shuffle the labels once.** Each female keeps her real number of broods, but her group label is randomly reassigned (without replacement, keeping group sizes at 77 and 72). Dots keep the color of their real group so students can watch the labels mix.
3. **Shuffle thousands of times.** Students add 10 to 10,000 shuffles and watch the null distribution build. Differences as extreme as ±0.84 are highlighted, and the two-tailed p-value updates live:
   `p = (left tail + right tail + 1) ÷ (N + 1)`
4. **Try other data.** Students paste in any two groups, or load a preset (tiny sample, zeros and an outlier, nearly identical groups, or the pseudoscorpion data), and run the full test.

### Analyze your own data (second tab)

A separate tab runs the same test on any two-group dataset:

1. **Load a CSV.** Either one column of group names plus one column of measurements, or one column per group. The app detects the layout, shows a preview, and reports any blank or non-numeric cells it skipped. Example files can be downloaded from the tab. Files can be up to 50 MB, with up to 100,000 values in the two groups being compared.
2. **Look at the data.** Group sizes, means, medians and SDs, a strip plot, and a one-shuffle preview.
3. **Set up and run.** Choose difference in means or medians, a two-sided or one-sided alternative, and α. Students run a 1,000-shuffle quick check first, then 10,000 shuffles for the final result.
4. **Result.** Null distribution, tail counts, p-value, a plain-language summary to copy, and a CSV of the shuffled differences.

Link straight to this tab with https://lizferguson5.github.io/randomization-tests/#your-data. Data stay in the browser; nothing is uploaded to a server.

Every run uses fresh random shuffles, so p-values vary slightly between students and runs. For the pseudoscorpion data, 10,000 shuffles typically give p ≈ 0.003–0.007.

## Data

The pseudoscorpion brood counts were reconstructed from the frequency histogram in the lecture slides. The reconstructed data reproduce the lecture's group means and difference (−0.84). The original study is Newcomer, Zeh & Zeh (1999), *PNAS* 96: 10236–10241, as presented in Whitlock & Schluter, *The Analysis of Biological Data*.

The Step 4 practice presets other than the pseudoscorpion data are made-up numbers for exploration.

## Using the app

- The app is a single self-contained file (`index.html`) with no dependencies or build step. It runs in any modern browser, on desktop or mobile, in light or dark mode.
- To run it locally, download `index.html` and open it in a browser.
- Accompanying Canvas questions (with answer key) are available from the instructor.

## License

Code is licensed under the [MIT License](LICENSE).

Instructional text and questions © 2026 Liz Ferguson, licensed under
[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). You're welcome to
reuse and adapt them for your own teaching. Please credit the original.

Created for BIOL 200.
