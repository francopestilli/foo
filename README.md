<!-- brainlife-app:begin (generated from the App manifest; edit the manifest, not this block) -->

> **Utility that copies a debiased, T1-aligned DWI (with bvals and bvecs) unchanged so the output carries the preprocessed datatype tag.**

Copies the input files unchanged to the output (no image processing is done, the main script only copies files with jq and cp). Use it to relabel a dataset with the datatype tag shown on the output when the processing it reflects was done elsewhere. Do not use it to actually process data.

| | |
|---|---|
| 📥 **Inputs** | `neuro/dwi` |
| 📤 **Outputs** | `neuro/dwi` |
| ⚙️ **Resources** | 8 CPUs · 1 h walltime |
| 🔗 **Run it** | [doi.org/10.25663/brainlife.app.846](https://doi.org/10.25663/brainlife.app.846) |

#### 📥 Inputs

| Input | Datatype | Required | Description |
|---|---|---|---|
| `dwi` | `neuro/dwi` (debiased, t1_aligned, !preprocessed) | yes | DWI image with bvals and bvecs; all three files must exist to be copied. |

#### 📤 Outputs

| Output | Datatype | Description |
|---|---|---|
| `dwi` | `neuro/dwi` | The same DWI, bvals and bvecs, copied unchanged and tagged preprocessed. |

<!-- brainlife-app:end -->

