# Siddharth Raina

Data scientist (12 years, Berlin) working on how LLM and agent evaluations are measured: whether the
number an eval reports means what it is taken to mean.

### The angle

Most eval defects don't crash. They produce plausible numbers: a scorer that reports zero when it
measured nothing, a completion metric that counts submissions the validator rejected, a detector that
counts the same evidence twice. Accuracy metrics catch none of these. I look for them by re-deriving
what a metric was computed over, and by reading the non-matches before quoting a count.

### Work

- **Inspect (UK AISI).** Merged fix for `web_search("exa")` validation failures
  ([#4913](https://github.com/UKGovernmentBEIS/inspect_ai/pull/4913)). Metric-validity input on
  [#5352](https://github.com/UKGovernmentBEIS/inspect_ai/issues/5352): five inspect_evals metrics
  report 0.0 when nothing is scored, bisected to the change that introduced it.
- **Replications.** Apollo Research's insider-trading eval across three model generations:
  [post](https://raina-sid.github.io/posts/insider-trading-eval-saturated.html),
  [code](https://github.com/raina-sid/inspect-eval-replications).
- **Experiments.** When do agents leak restricted information, and what the scorer can't see:
  [post](https://raina-sid.github.io/posts/when-agents-leak-restricted-information.html).
- **Tools.** [inspect-scorer-probes](https://github.com/raina-sid/inspect-scorer-probes): audit diffs
  between two states of an eval, and metamorphic probes for scorer contracts.

Method: [How I evaluate evaluations](https://raina-sid.github.io/method.html) · Writing:
[raina-sid.github.io](https://raina-sid.github.io)
