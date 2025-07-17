 (cd "$(git rev-parse --show-toplevel)" && git apply --3way <<'EOF' 
diff --git a/README.md b/README.md
index afdade0400b5cfcc2ab16484946ce99e44be225b..0db99c8625278ee7482925154e9ae369e04f91d1 100644
--- a/README.md
+++ b/README.md
@@ -1,17 +1,24 @@
-# Digits_recognizer_Neuralnetwork
-Recognize hand written digits classifier from 0 to 9.
+# Digits Recognizer Neural Network
 
-# Used Package
-Numpy, Matplotlib, Tensorflow(Keras/Sequential Model and Dense Layer)
+This repository contains a Jupyter notebook demonstrating a simple neural network that classifies handwritten digits.
+It is based on the practice labs from a machine learning course, and some utility modules referenced in the notebook are not included here.
 
-# Approach
-Binary Classification 
---> Use ReLU, Softmax Function.
+## Requirements
 
-# Progress
-Variable check & Visualize
---> Model Representation
---> Model Implementation
---> Softmax Placement
+- Python 3
+- numpy
+- matplotlib
+- tensorflow
 
-Epoch: 100 times
+A `requirements.txt` file is provided for convenience.
+
+## Usage
+
+1. Install the dependencies:
+   ```bash
+   pip install -r requirements.txt
+   ```
+2. Launch Jupyter and open `Digits_recognizer.ipynb` to run the notebook.
+
+The dataset and helper functions (`autils`, `public_tests`, `lab_utils_softmax`, etc.) used in the original course material are not part of this repository.
+You may need to modify the notebook to load your own data or provide alternative implementations for these helpers.
 
EOF
)
