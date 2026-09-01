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
If you use this work in research, please cite the repository or any associated publication/paper. (Add citation details or DOI here if available.)

## Contact
Mohammod Hamed Hasan — (GitHub: @Hamed18)  
For dataset questions, reproduction help, or collaboration, open an issue or send a pull request.

## License
Add an explicit license (e.g., MIT) to clarify reuse permissions. If no license is present, the repository is not open-source by default.
