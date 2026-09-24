# A capture from a modified build was mistaken for an original reference

- **Search terms:** reference provenance, runtime capture, original pose, earlier project output, style reference, withdrawn candidate
- **Observed scope:** A character hit pose redrawn for a Mega Drive host, using a battle capture taken earlier in the same project as the "original" pose reference.
- **Failure context:** The capture came from an existing project run and looked like the host's original sprite. A new candidate was generated from it and described as original-based.
- **Evidence:** After the person questioned it, the build manifest, asset recipe, and idle-PoC binding showed that the captured frame was a slot the project had already replaced. The candidate was marked as withdrawn for an invalid source; the original frame had not yet been recovered.
- **Established result:** A runtime capture identifies the build it came from, not the original release. Resemblance and a work-folder location did not establish origin.
- **Transfer limit:** Trace each reference to its producing input identity. Captures from the untouched original remain valid references once that identity is recorded.
- **Related criteria:** `references/strategy/creative-review.md` §Reference Identity, `references/conventions/artifact-states.md` §Authored Or Generated Asset Provenance, `references/conventions/observation-records.md` §Raw Result.
