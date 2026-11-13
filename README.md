# JBHI submission files

Everything needed to submit the manuscript to *IEEE Journal of Biomedical and Health Informatics* through ScholarOne. Each folder matches one section of the upload page.

**Title:** Driver Vigilance Estimation From EEG and Forehead EOG Under Deployment Constraints: Real-Time Features, Unseen Subjects, and Interpretable Kolmogorov–Arnold Networks
**Manuscript type:** Regular paper (13 pages)

## Required uploads

| # | Upload section | File | Notes |
|---|---|---|---|
| 1 | Main Manuscript | `1_Main_Manuscript/JBHI_ShyakaAlainChristian_LaTeX_Source.zip` | LaTeX source in one archive: `main.tex`, `main.bbl`, `refs.bib`, 7 figures, 1 table, `ieeecolor.cls`, `generic.sty`, logo files. Tested: compiles on its own to 13 pages with no errors. The PDF in the same folder is the compiled version, for reference or if a PDF is also requested. |
| 2 | Conflict of Interest | none | Tick the box stating that none of the authors have a conflict of interest. No file is needed. |
| 3 | Author Consent Form | `3_Author_Consent_Form/JBHI_ShyakaAlainChristian_ConsentForm.pdf` | Signed by all three authors, dated 2026-11-13. |
| 4 | Graphical Abstract | `4_Graphical_Abstract/JBHI_ShyakaAlainChristian_GraphicalAbstract.png` | 1980 × 885 px (aspect ratio 660:295). Built from the paper's results. |
| 5 | Graphical Abstract Text | `5_Graphical_Abstract_Text/JBHI_ShyakaAlainChristian_GraphicalAbstract_Text.txt` | 2 sentences, 40 words (limit 50). |

## Optional uploads that apply

| Upload section | File | Notes |
|---|---|---|
| Cover Letter | `6_Cover_Letter/JBHI_ShyakaAlainChristian_CoverLetter.pdf` | Paste `..._CoverLetter_PasteText.txt` into the text box, or upload the PDF. Seen by the editor only. |
| Previously Published Statement | `7_Previously_Published_Statement/..._Statement.txt` | Explains how this paper differs from the authors' CAIT 2024 conference paper, which it cites. Upload the CAIT 2024 PDF here as well (download it from IEEE Xplore, doi:10.1109/CAIT64506.2024.10963136). |

Not needed: tracked-changes manuscript (first submission), separate figure files (figures are in the LaTeX archive), supplementary material (code is public and linked in the paper), LaTeX supplementary files (all inside the archive).

## Form fields

**Authors** (enter in this order):

| # | First name | Last name | E-mail | ORCID | Affiliation |
|---|---|---|---|---|---|
| 1 (corresponding) | Shyaka Alain | Christian | alainchristian@nuaa.edu.cn | 0009-0004-0374-6331 | College of Computer Science and Technology, Nanjing University of Aeronautics and Astronautics, Nanjing 211106, China |
| 2 | Zhe | Chen | zhechen@nuaa.edu.cn | 0000-0002-4707-2402 | College of Computer Science and Technology, Nanjing University of Aeronautics and Astronautics, Nanjing 211106, China |
| 3 | Dawit Abdisa | Jebessa | davidabdisa40@mail.ustc.edu.cn | 0009-0007-5807-2364 | School of Software Engineering, University of Science and Technology of China, Suzhou 215123, China |

**Keywords:** Driver drowsiness; electroencephalography; electrooculography; evaluation protocol; interpretable machine learning; Kolmogorov–Arnold network; vigilance estimation

**Funding:** none. The work did not receive support from any funding organization.

**Data:** SEED-VIG (Shanghai Jiao Tong University, available under license). Code: https://github.com/Helloworldceo/Alain_DDD-dataset

**Abstract** (250 words, as in the manuscript):

Drowsy driving is a major cause of road crashes, and electroencephalography and electrooculography can track the preceding loss of vigilance. An in-vehicle vigilance monitor must work in real time and for drivers it has never seen, whereas many SEED-VIG results rely on features smoothed over whole sessions, which require future samples, and on test subjects seen during training. This study measures how much these shortcuts inflate reported performance and develops an estimator that satisfies both constraints. Recordings of 21 subjects are cleaned automatically, and 19 physiologically motivated features are computed from past and current samples only, with every session-level parameter estimated from an unlabeled two-minute warm-up. With identical models, random window splitting raises the correlation with the percentage of eyelid closure by 0.12 to 0.27 over leave-one-subject-out evaluation, and session-smoothed features raise it by a further 0.05 to 0.13; strictly real-time processing lowers it by at most 0.03. On unseen subjects without labeled calibration data, a Kolmogorov–Arnold network on the 19 features reaches a correlation of 0.724 and the lowest root-mean-square error of all models, 0.169. It matches a long short-term memory network (0.728 and 0.183) with 25 times fewer parameters and significantly outperforms a convolutional–recurrent network on raw signals, cleaned or not. Its learned functions recover established physiology: predicted drowsiness rises with the ratio of slow to fast posterior brain rhythms and, above a threshold, with slow eye movements, and falls with saccade rate. The result is an accurate, interpretable, and lightweight estimator, evaluated as it would be deployed.
