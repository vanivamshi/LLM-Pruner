# LLM-Pruner

Simple LLM pruner designed using GPT-2. It includes,
1) Gradual pruning: Incrementally removes weights from the model over multiple training iterations
2) Layer-wise pruning: Prunes specific layers of a neural network
3) Mixed Precision Training: Utilize PyTorch’s AMP (Automatic Mixed Precision) to reduce memory usage and speed up training and inference without significant loss in accuracy.
4) Post-Training Quantization: Reduce the model size and computational requirements.
5) Distillation Post-Pruning: Applied after pruning to recover lost accuracy due to pruning by aligning the outputs of the pruned model with those of the original.
6) Memory Mapping: Avoids loading the entire dataset into memory, reducing the memory footprint.
7) Perplexity: Measures how well a probabilistic model predicts a text sample
