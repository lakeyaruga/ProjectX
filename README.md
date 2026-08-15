Antibody–Antigen Binding Prediction with Deep Learning

Predicting antibody–antigen binding from protein sequence data by designing, benchmarking, and improving on a range of deep learning architectures. Final-year project awarded a first-class grade.

Overview

Antibody–antigen binding is central to immune response and to therapeutic antibody design. The goal of this project was to predict whether a given antibody–antigen pair binds, using representations derived from a protein language model, and to test whether a custom architecture could outperform standard sequence models on the task.

Approach
Data / features: protein sequences represented using protein-language-model embeddings (ESM-2), used as input features for binding prediction.
Models benchmarked: MLP, CNN, LSTM, GRU, and a Transformer, implemented and evaluated under a consistent pipeline for fair comparison.
Custom model: designed a novel cross-attention Transformer to better capture interactions between antibody and antigen representations.
Pipeline: built end-to-end in PyTorch, covering preprocessing, feature handling, training, and evaluation.
Results
The custom cross-attention model achieved 0.795 AUROC, outperforming all benchmarked baselines.
Demonstrated that modelling antibody–antigen interactions directly (via cross-attention) improved performance over models that processed sequences independently.
Tools & Techniques

Python · PyTorch · deep learning (MLP, CNN, LSTM, GRU, Transformer) · attention / cross-attention · protein language model embeddings (ESM-2) · model benchmarking & evaluation (AUROC)

What I learned

Building and fairly benchmarking multiple deep learning architectures under one pipeline.
Designing a custom attention-based architecture motivated by the structure of the problem.
End-to-end ML workflow: data preparation, training, evaluation, and interpreting results.
