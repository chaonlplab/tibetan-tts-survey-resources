# Tibetan TTS Resource Collection

Companion repository for the survey:

> **Recent Advances in Tibetan Speech Synthesis: A Survey**
> Chao Wang, Yuqing Cai, Renzeng Duojie, Yulei Zhu, Yutong Liu, Jinying Xiao, Lhamao Kyi, Pengbo Zhang, Tashi Nyima
> Submitted to IEEE Transactions on Audio, Speech, and Language Processing (TASLP)

This repository provides machine-readable versions of the resource inventories, study
characteristics, and evidence-tier codings used in the survey, together with links to
every retained Tibetan speech resource where a public identifier exists.

## Scope and Evidence Window

The survey's narrative evidence window is **frozen on 27 August 2026**. The frozen
window guarantees that every claim in the paper maps to a fixed, traceable record set.
This repository extends beyond the frozen window: new Tibetan TTS resources, benchmarks,
and replications are added as they become available, with an `added_after_freeze` date
so that post-freeze records are always distinguishable from the records underlying the
paper's tables.

## Contents

| File | Corresponds to | Description |
|---|---|---|
| `data/resources.csv` | Tables II & VIII | All 13 retained Tibetan speech resources (R01–R13) with dialect, speakers, size, annotation, access status, FAIR screen, and source identifiers |
| `data/studies.csv` | Table V | Tibetan TTS studies (2011–2025) with technical route, front-end report, evaluation, and verification status |
| `data/evidence_tiers.csv` | Table VII | Descriptive evidence-tier coding by technical route |

## Column Definitions (`data/resources.csv`)

- `resource_id` — R01–R13, identical to the identifiers used in the paper
- `resource_name` — name as reported by the source
- `dialect` — dialect / language coverage (Ü-Tsang, Amdo, Kham, etc.)
- `speakers`, `size`, `sampling_rate` — as reported; `NR` = not reported by the source
- `annotation` — annotation types reported
- `access_status`, `license` — source-reported access and license terms
- `paper_title`, `authors`, `venue`, `year`, `doi` — bibliographic identity
- `paper_url` — link to the describing paper (DOI resolver); `NR` if no public identifier
- `dataset_url` — direct link to the released data, or `not publicly released`
- `fair_f/​fair_a/​fair_i/​fair_r` — source-reported FAIR-readiness screen (F/A/I/R)
- `tts_relevant` — whether the resource is TTS-oriented or recognition-adjacent
- `added_after_freeze` — empty for records inside the paper's frozen window

R13 (TibetanVoice) is the only retained resource with a public download interface
(Hugging Face). Its claimed arXiv companion paper could not be verified during the
survey's audit, so it is cited as a dataset record rather than as an arXiv preprint.

## Access Notes

Many Tibetan speech resources are reported in the literature but not publicly released.
`NR` (not reported) values are inherited directly from the source papers; the survey
does not infer missing metadata. If you maintain one of these resources and can offer
a public locator, license, or corrected metadata, please open an issue or pull request.

## Citation

If you use this collection, please cite the survey (BibTeX will be added upon
publication) and this repository:

```bibtex
@misc{tibetan_tts_survey_resources,
  title  = {Tibetan TTS Resource Collection},
  author = {Wang, Chao and Cai, Yuqing and Duojie, Renzeng and Zhu, Yulei and Liu, Yutong and Xiao, Jinying and Kyi, Lhamao and Zhang, Pengbo and Nyima, Tashi},
  year   = {2026},
  note   = {Companion repository for "Recent Advances in Tibetan Speech Synthesis: A Survey". Zenodo DOI to be assigned}
}
```

## License

Data files in this repository are released under the CC BY 4.0 License (to be confirmed
before publication).
