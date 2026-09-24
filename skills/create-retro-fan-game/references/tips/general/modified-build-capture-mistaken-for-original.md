# A capture from a modified build was mistaken for an original reference

- **Search terms:** reference provenance, runtime capture, original pose, earlier project output, style reference, withdrawn candidate
- **Misleading observation:** A runtime capture or work-folder image looks like the host's original sprite, pose, or sound, and a candidate is described as original-based.
- **Other interpretation:** The capture came from a build in which the project had already replaced that slot. Resemblance and location do not establish origin.
- **Distinguishing check:** Trace the reference to the input identity that produced it, such as the build receipt and the asset binding of that build. If it was modified, withdraw dependent candidates and recover the original.
- **Transfer limit:** Captures from the untouched original remain valid references once that identity is recorded.
- **Related criteria:** `references/strategy/creative-review.md` §Reference Identity, `references/conventions/artifact-states.md` §Authored Or Generated Asset Provenance, `references/conventions/observation-records.md` §Raw Result.
