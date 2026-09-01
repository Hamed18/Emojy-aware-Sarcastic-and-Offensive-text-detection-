# EmoMTL: Emoji-Aware Multitask Learning for Code-Mixed Low-Resource Language

Author: Mohammod Hamed Hasan

Tech: Python, Jupyter, Pandas, NumPy, Scikit-learn, PyTorch, Transformers models, Matplotlib, Seaborn 

---

## Project overview
EmoMTL is an emoji-aware multitask learning pipeline designed for classifying code-mixed (Bengali–English) social media comments in low-resource settings. The project focuses on leveraging emoji context and shared representations (cross-stitch networks) to improve performance on multiple related tasks (e.g., sarcasm, offensiveness, sentiment) when labeled data is scarce.

## Key contributions
- Built a multi-label, code-mixed Bengali social media dataset annotated for relevant downstream tasks and prepared emoji-aware preprocessing pipelines.
- Implemented a multitask learning architecture using cross-stitch units to share representations between tasks while allowing task-specific specialization.
- Evaluated 10+ baselines across traditional ML, sequence models, and transformers:
  - Classical ML: SVM, Random Forest (RF), etc.
  - Sequence models: BiLSTM
  - Transformer-based: mBERT, RoBERTa, BanglaBERT
- Performed thorough error analysis and applied explainable AI techniques (feature importances, attention inspection) to interpret model behavior.
- Validated results with stratified multi-fold cross-validation and statistical significance testing.

## Challenges & solutions
- Challenge: Low-resource code-mixing (Bengali–English) and emoji context degrade standard transformer performance — noisy tokens, out-of-vocabulary words, and semantics encoded by emojis.
- Solution: Introduced emoji-aware encoding (emoji normalization/presence features and embedding strategies) and cross-stitch sharing to better leverage correlated signals across tasks. Used class-weighting and sampling to mitigate label imbalance. Applied significance testing to ensure reported improvements are robust.

## Results & evaluation
- Comparative evaluation across 10+ baselines demonstrates that emoji-aware multitask learning with cross-stitch sharing consistently improves recall and F1 for under-represented labels compared to single-task transformer baselines.
- Results are reported using multi-fold cross-validation and accompanied by error analysis and interpretability artifacts (confusion matrices, attention/feature visualizations).

## How to cite
If you use this work in research, please ask for permission to the Author and cite the repository or any associated publication/paper. (Add citation details or DOI here if available.)

## Contact
Mohammod Hamed Hasan — (GitHub: @Hamed18)  
For dataset questions, reproduction help, or collaboration, open an issue or send a pull request.

## License — IMPORTANT
All Rights Reserved — No Use Without Permission.
Copyright (c) 2026 Hamed18
All Rights Reserved — No Use Without Prior Written Permission

1. Ownership
   The copyright holder (\"Copyright Holder\") of this repository and its contents is:
   Hamed18 (GitHub: https://github.com/Hamed18)
   Effective date: 2026-09-01

   The term "Materials" in this License means all repository contents including, but not limited to:
   - source code, scripts, Jupyter notebooks, models, configuration files;
   - datasets, annotations, and any derived data;
   - documentation, experiments, and analysis results;
   - any other files, media, or digital assets distributed with or referenced by this repository.

2. Permission and Prohibited Uses
   Except as expressly authorized in a separate, written license agreement signed by the Copyright Holder,
   you are strictly prohibited from doing any of the following with the Materials:

   a. Copying, reproducing, distributing, publishing, displaying, or publicly performing the Materials;
   b. Creating derivative works, modifications, adaptations, translations, compilations, or other
      works based upon the Materials;
   c. Licensing, sublicensing, selling, renting, leasing, lending, or otherwise transferring rights to
      the Materials to any third party;
   d. Using the Materials in whole or in part to train, fine-tune, evaluate, or produce machine learning
      or generative models that are redistributed or offered as a service, without prior written permission;
   e. Sharing, publishing, or otherwise making available the proprietary dataset(s) used in this repository,
      in whole or in part, to any third party;
   f. Using the Materials for any commercial purpose, including internal commercial use, without prior
      written permission.

3. Permitted Use by Permission Only
   Any use of the Materials is permitted only if and to the extent a written license or permission
   (\"Permission\") is granted by the Copyright Holder. Permission, if granted, may be subject to
   additional terms and conditions, including limitations on purpose, duration, distribution, attribution,
   confidentiality, indemnity, and financial compensation.

4. Requesting Permission
   To request Permission, provide the Copyright Holder with:
   - Your full name and affiliation;
   - Contact information (email and phone, if available);
   - A clear description of which Materials you wish to use;
   - The intended purpose and scope of use (research, educational, commercial, derivative works, etc.);
   - Whether you intend to redistribute, publish, or otherwise make the Materials (or derivatives) public;
   - Any proposed terms or agreements (e.g., collaboration, licensing fee, attribution).
   Contact:
   - GitHub: https://github.com/Hamed18
   - Email: hamedhasan.dev@gmail.com

5. Attribution and Notices
   If Permission is granted, the Copyright Holder may require:
   - Preservation of copyright and other proprietary notices in the Materials;
   - Clear attribution in derivative works or publications, as specified in the agreement.

6. Termination
   Any unauthorized use of the Materials is a material breach of this License and any granted Permission.
   The Copyright Holder may immediately terminate any Permission for breach, and may pursue available
   legal and equitable remedies, including injunctive relief and damages.

7. No Warranty
   The Materials are provided \"AS IS\" and without warranty of any kind, express or implied, including but
   not limited to warranties of merchantability, fitness for a particular purpose, non-infringement, or
   accuracy. The Copyright Holder disclaims all liability for damages arising from use or inability to use
   the Materials.

8. Limitation of Liability
   To the fullest extent permitted by applicable law, in no event shall the Copyright Holder be liable for
   any direct, indirect, incidental, special, consequential, or exemplary damages arising out of or in
   connection with access to, use of, or inability to use the Materials.

9. Governing Law
   This License and any disputes arising out of or related to it shall be governed by the laws of the
   jurisdiction where the Copyright Holder resides (unless otherwise agreed in writing), without regard to
   its conflict of laws rules. The Copyright Holder may elect to pursue enforcement in any competent forum.

10. DMCA and Enforcement
    If you believe someone has used the Materials in violation of this License, contact the Copyright Holder
    with details of the alleged infringement. The Copyright Holder may pursue removal, takedown, or other
    enforcement actions as appropriate.

11. Miscellaneous
    - This License does not grant any patent or trademark rights except as explicitly stated in a separate
      written agreement.
    - No waiver of any provision of this License shall be effective unless in writing signed by the Copyright Holder.

© 2026 Hamed18 — All Rights Reserved

