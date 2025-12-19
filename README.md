# Surrey-AML-Assignment
AML Assignment
**Applied Machine Learning EEEM076 Assignment - 6926172**
**Vision Transformer (ViT) on Place2_simp dataset - Comparative Analysis**

## Files
* 'EEEM076_6926172_Assignment (Ver A).ipynb': The main training and evaluation code.
* 'results/': TensorBoard logs, Plots and confusion matrices.
* 'model_weights/': Fine-Tuned ViT model weights.

## How to run
1. Open the notebook (`EEEM076_6926172_Assignment (Ver A).ipynb`) in Google Colab
2. Require GPU (T4 GPU) setting
3. Run the cells in order
4. Training Loops take up to hours.  Previous Outputs and Results are already in the notebook.
5. Part 0 is the necessary imports and setups.  Training loops cells could be skipped if not necessary.
6. Results, eg. TensorBoard logs, plots and confusion matrices are saved automatically in 'results' in this repository.
7. Fine-tuned ViT model weights are automatically saved in 'model_weights' in this respository.

## Outline of EEEM076_6926172_Assignment (Ver A).ipynb --
Part 1 - Compare ViT (vit-base-patch64-224) and CNN (ResNET50)
A. Setup of ViT (FlexibleViT) and CNN/ResNet50 (FlexibleCNN)
B. Compare FlxibleViT and FlexibleCNN for val accuracy

Part 2 - Fine-tuning of ViT hyperparameters
A. Learning Rate - 1e-5, 5e-4, 1e-4
B. Batch Size - 16, 64
C. Weight decays - 0.0, 0.1
D. Long run - 15 epochs
E. Re-run Fine-tuned ViT and test on Custom Test Set (my_custom_testset)

Part 3 - Zero Shot recognition
A. CLIP (Standard Prompt)
B. CLIP (Ensemble Prompting)
C. CLIP (Natural Language Prompting - GPT generated)

Part 4 - Few Shots recognition
A. CLIP with CoOp (Context Optimization)

## Note:
Datasets (code will upload the zip files automatically from Google Drive and unzip in Colab):
1. Places2_simp.zip
2. my_custom_testset.zip
3. testset.zip (just for reference)

## Outputs
Output results, eg. tensorboard logs, plots & etc will be saved in 'results/' in this repository
