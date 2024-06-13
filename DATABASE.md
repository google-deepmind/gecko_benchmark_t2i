
# Gecko Benchmark

There are three aspects to the Gecko benchmark:
- A prompt set
- Generated images
- Human annotations

## Prompt set

The prompts are located within the CSV `./prompts.csv`.
There are five types of columns:

- `prompt_id`: the ID.
- `prompt_type`: Whether it came from Gecko(R) or Gecko(S).
- `dataset_id`: The dataset id. For Gecko(R) prompts, the original dataset it
 was sampled from and a numeric identifier. For Gecko(S) prompts, the type of
 prompt.
- `prompt`: The prompt.
- `max_disagreement_less_X%`: Whether the prompt is reliable if we use X% as
 the threshold. In the paper we used `50%`. There are two versions: v1 and v2.
 v1 is where we used the standard deviation for Likert ratings and v2 is the case where we use variance (as described in the paper). v1 is more conservative than v2.

Note that this prompt set is a subset of those used in the tech report as we
 have done additional filtering before release.

## Images and Human annotation
Working on.
