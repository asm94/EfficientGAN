# About
EfficientNet with keras.  
(For only tabular data)

# Environment
-python     == 3.8.3  
-cuda       == 10.1  
-cudnn      == 7.6.5  
-tensorflow == 2.3.1

# Usage

```python
from model import EfficientGAN

iris = load_iris()
X_train, X_test, y_true = (iris['data'], iris['data'], iris['target'])

model = EfficientGAN()
model.fit(X_train, test=(X_test,y_true))
proba = model.predict(X_test)
```

# Reference
-Article  
https://arxiv.org/abs/1802.06222   
-Authors' github  
https://github.com/houssamzenati/Efficient-GAN-Anomaly-Detection
